# Comparing `tmp/abb_robot_client-0.3.0-py3-none-any.whl.zip` & `tmp/abb_robot_client-0.3.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 31580 bytes, number of entries: 11
+Zip file size: 31673 bytes, number of entries: 11
 -rw-rw-rw-  2.0 fat        0 b- defN 22-Nov-09 08:02 abb_robot_client/__init__.py
 -rw-rw-rw-  2.0 fat    13281 b- defN 23-Oct-18 00:09 abb_robot_client/egm.py
--rw-rw-rw-  2.0 fat    44041 b- defN 23-Oct-18 00:09 abb_robot_client/rws.py
--rw-rw-rw-  2.0 fat    37208 b- defN 22-Dec-29 01:09 abb_robot_client/rws_aio.py
+-rw-rw-rw-  2.0 fat    44686 b- defN 24-Apr-10 19:30 abb_robot_client/rws.py
+-rw-rw-rw-  2.0 fat    37879 b- defN 24-Apr-10 19:30 abb_robot_client/rws_aio.py
 -rw-rw-rw-  2.0 fat        0 b- defN 22-Nov-09 20:28 abb_robot_client/_egm_protobuf/__init__.py
 -rw-rw-rw-  2.0 fat     8345 b- defN 23-Oct-18 00:09 abb_robot_client/_egm_protobuf/egm_pb2.py
--rw-rw-rw-  2.0 fat    11601 b- defN 23-Oct-18 00:11 abb_robot_client-0.3.0.dist-info/LICENSE.txt
--rw-rw-rw-  2.0 fat     3009 b- defN 23-Oct-18 00:11 abb_robot_client-0.3.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Oct-18 00:11 abb_robot_client-0.3.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       17 b- defN 23-Oct-18 00:11 abb_robot_client-0.3.0.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      959 b- defN 23-Oct-18 00:11 abb_robot_client-0.3.0.dist-info/RECORD
-11 files, 118553 bytes uncompressed, 29938 bytes compressed:  74.7%
+-rw-rw-rw-  2.0 fat    11601 b- defN 24-Apr-10 19:31 abb_robot_client-0.3.1.dist-info/LICENSE.txt
+-rw-rw-rw-  2.0 fat     3009 b- defN 24-Apr-10 19:31 abb_robot_client-0.3.1.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-10 19:31 abb_robot_client-0.3.1.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       17 b- defN 24-Apr-10 19:31 abb_robot_client-0.3.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      959 b- defN 24-Apr-10 19:31 abb_robot_client-0.3.1.dist-info/RECORD
+11 files, 119869 bytes uncompressed, 30031 bytes compressed:  74.9%
```

## zipnote {}

```diff
@@ -12,23 +12,23 @@
 
 Filename: abb_robot_client/_egm_protobuf/__init__.py
 Comment: 
 
 Filename: abb_robot_client/_egm_protobuf/egm_pb2.py
 Comment: 
 
-Filename: abb_robot_client-0.3.0.dist-info/LICENSE.txt
+Filename: abb_robot_client-0.3.1.dist-info/LICENSE.txt
 Comment: 
 
-Filename: abb_robot_client-0.3.0.dist-info/METADATA
+Filename: abb_robot_client-0.3.1.dist-info/METADATA
 Comment: 
 
-Filename: abb_robot_client-0.3.0.dist-info/WHEEL
+Filename: abb_robot_client-0.3.1.dist-info/WHEEL
 Comment: 
 
-Filename: abb_robot_client-0.3.0.dist-info/top_level.txt
+Filename: abb_robot_client-0.3.1.dist-info/top_level.txt
 Comment: 
 
-Filename: abb_robot_client-0.3.0.dist-info/RECORD
+Filename: abb_robot_client-0.3.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## abb_robot_client/rws.py

```diff
@@ -266,15 +266,16 @@
 
         :param cycle: The cycle mode of the robot. Can be `asis`, `once`, or `forever`.
         :param tasks: One or more tasks to start.
         """
 
         rob_tasks = self.get_tasks()
         for t in tasks:
-            assert t in rob_tasks, f"Cannot start unknown task {t}"
+            if not t in rob_tasks:
+                raise Exception(f"Cannot start unknown task {t}")
 
         for rob_task in rob_tasks.values():
             if not rob_task.motiontask:
                 continue
             if rob_task.name in tasks:
                 if not rob_task.active:
                     self.activate_task(rob_task.name)
@@ -479,30 +480,32 @@
         Read a file off the controller
 
         :param filename: The filename to read
         :return: The file bytes
         """
         url="/".join([self.base_url, "fileservice", filename])
         res=self._session.get(url, auth=self.auth)
-        assert res.ok, f"File not found {filename}"
+        if not res.ok:
+            raise Exception(f"File not found {filename}")
         try:            
             return res.content
         finally:
             res.close()
 
     def upload_file(self, filename: str, contents: bytes):
         """
         Upload a file to the controller
 
         :param filename: The filename to write
         :param contents: The file content bytes
         """
         url="/".join([self.base_url, "fileservice" , filename])
         res=self._session.put(url, contents, auth=self.auth)
-        assert res.ok, res.reason
+        if not res.ok:
+            raise Exception(res.reason)
         res.close()
 
     def delete_file(self, filename: str):
         """
         Delete a file on the controller
 
         :param filename: The filename to delete
@@ -585,15 +588,16 @@
         Get the current jointtarget for specified mechunit
 
         :param mechunit: The mechanical unit to read
         :return: The current jointtarget
         """
         res_json=self._do_get("rw/motionsystem/mechunits/" + mechunit + "/jointtarget")
         state = res_json["_embedded"]["_state"][0]
-        assert state["_type"] == "ms-jointtarget"
+        if not state["_type"] == "ms-jointtarget":
+            raise Exception("Invalid jointtarget type")
         robjoint=np.array([state["rax_1"], state["rax_2"], state["rax_3"], state["rax_4"], state["rax_5"], 
             state["rax_6"]], dtype=np.float64)
         extjoint=np.array([state["eax_a"], state["eax_b"], state["eax_c"], state["eax_d"], state["eax_e"], 
             state["eax_f"]], dtype=np.float64)
      
         return JointTarget(robjoint,extjoint)
         
@@ -606,31 +610,34 @@
         :param wobj: The wobj to use to compute robtarget
         :param coordinate: The coordinate system to use to compute robtarget. Can be `Base`, `World`, `Tool`, or `Wobj`
         :return: The current robtarget
 
         """
         res_json=self._do_get(f"rw/motionsystem/mechunits/{mechunit}/robtarget?tool={tool}&wobj={wobj}&coordinate={coordinate}")
         state = res_json["_embedded"]["_state"][0]
-        assert state["_type"] == "ms-robtargets"
+        if not state["_type"] == "ms-robtargets":
+            raise Exception("Invalid robtarget type")
         trans=np.array([state["x"], state["y"], state["z"]], dtype=np.float64)
         rot=np.array([state["q1"], state["q2"], state["q3"], state["q4"]], dtype=np.float64)
         robconf=np.array([state["cf1"],state["cf4"],state["cf6"],state["cfx"]], dtype=np.float64)
         extax=np.array([state["eaxa"], state["eaxb"], state["eaxc"], state["eaxd"], state["eaxe"], 
             state["eaxf"]], dtype=np.float64)
         return RobTarget(trans,rot,robconf,extax)
     
     def _rws_value_to_jointtarget(self, val):
         v1=re.match('^\\[\\[([^\\]]+)\\],\\[([^\\]]+)\\]',val)
         robax = np.deg2rad(np.fromstring(v1.groups()[0],sep=','))
         extax = np.deg2rad(np.fromstring(v1.groups()[1],sep=','))
         return JointTarget(robax,extax)
     
     def _jointtarget_to_rws_value(self, val):
-        assert np.shape(val[0]) == (6,)
-        assert np.shape(val[1]) == (6,)
+        if not np.shape(val[0]) == (6,):
+            raise Exception("Invalid jointtarget")
+        if not np.shape(val[1]) == (6,):
+            raise Exception("Invalid jointtarget")
         robax=','.join([format(x, '.4f') for x in np.rad2deg(val[0])])
         extax=','.join([format(x, '.4f') for x in np.rad2deg(val[1])])
         rws_value="[[" + robax + "],[" + extax + "]]"
         return rws_value
     
     def get_rapid_variable_jointtarget(self, var, task: str = "T_ROB1") -> JointTarget:
         """
@@ -748,15 +755,16 @@
         
         timeout_str=""
         if timeout > 0:
             timeout_str="&timeout=" + str(timeout)
         
         res_json=self._do_get("rw/dipc/" + queue_name + "/?action=dipc-read" + timeout_str)
         for state in res_json["_embedded"]["_state"]:
-            assert state["_type"] == "dipc-read-li"
+            if not state["_type"] == "dipc-read-li":
+                raise Exception("Invalid IPC message type")
      
             o.append(IpcMessage(state["dipc-data"], state["dipc-userdef"],
                 state["dipc-msgtype"], state["dipc-cmd"], state["queue-name"]))
             
             #o.append(RAPIDEventLogEntry(msg_type,code,tstamp,args,title,desc,conseqs,causes,actions))
         return o
     
@@ -764,15 +772,16 @@
         """
         Get the current speed ratio
 
         :return: The current speed ratio between 0% - 100%
         """
         res_json=self._do_get(f"rw/panel/speedratio")
         state = res_json["_embedded"]["_state"][0]
-        assert state["_type"] == "pnl-speedratio"
+        if not state["_type"] == "pnl-speedratio":
+            raise Exception("Invalid speedratio type")
         return float(state["speedratio"])
     
     def set_speedratio(self, speedratio: float):
         """
         Set the current speed ratio
 
         :param speedratio: The new speed ratio between 0% - 100%
@@ -835,15 +844,16 @@
         """
         t1=time.time()
         self._do_post('users/rmmp?json=1', {'privilege': 'modify'})
         while time.time() - t1 < timeout:
             
             res_json=self._do_get('users/rmmp/poll?json=1')
             state = res_json["_embedded"]["_state"][0]
-            assert state["_type"] == "user-rmmp-poll"
+            if not state["_type"] == "user-rmmp-poll":
+                raise Exception("Invalid rmmp poll type")
             status = state["status"]
             if status=="GRANTED":
                 self.poll_rmmp()
                 return
             elif status!="PENDING":
                 raise Exception("User did not grant remote access")                               
             time.sleep(0.25)
@@ -879,15 +889,16 @@
                     rmmp_session.cookies.set_cookie(c)
         
         rmmp_session=self._rmmp_session        
                 
         res=rmmp_session.get(url, auth=self.auth)
         res_json=self._process_response(res)
         state = res_json["_embedded"]["_state"][0]
-        assert state["_type"] == "user-rmmp-poll"
+        if not state["_type"] == "user-rmmp-poll":
+            raise Exception("Invalid rmmp poll type")
                 
         if old_rmmp_session is not None:
             self._rmmp_session=rmmp_session
             self._rmmp_session_t=time.time()
             try:
                 old_rmmp_session.close()
             except:
@@ -963,31 +974,33 @@
                     unit = "DRV_1"
                 else:
                     signal = r.param["signal"]
                     network = r.param.get("network", "Local")
                     unit = r.param.get("unit", "DRV_1")
                 payload[f"{payload_ind}"] = f'/rw/iosystem/signals/{network}/{unit}/{signal};state'
             else:
-                assert False, "Invalid resource type"
+                raise Exception("Invalid resource type")
             payload[f"{payload_ind}-p"] = f"{r.priority.value}"
 
         payload["resources"] = [f"{i+1}" for i in range(payload_ind)]
 
                 
         url="/".join([self.base_url, "subscription"]) + "?json=1"
         res1=self._session.post(url, data=payload, auth=self.auth)
         try:
             res=self._process_response(res1)
         finally:
             res1.close()
 
-        assert res1.status_code == 201, "Subscription creation failed"
+        if not res1.status_code == 201:
+            raise Exception("Subscription creation failed")
 
         m = re.search(r'<a href="ws:\/\/.*(\/poll\/\d+)" rel="self">', res1.content.decode("ascii"))
-        assert m
+        if not m:
+            raise Exception("Invalid subscription response")
         ws_url = self.base_url.replace("http:","ws:") + m.group(1)
         
         cookie = f"ABBCX={self._session.cookies['ABBCX']}"
         header={'Cookie': cookie, 'Authorization': self.auth.build_digest_header("GET", ws_url)}
 
         return RWSSubscription(ws_url, header, handler)
```

## abb_robot_client/rws_aio.py

```diff
@@ -116,15 +116,16 @@
         Start one or more RAPID tasks
 
         :param cycle: The cycle mode of the robot. Can be `asis`, `once`, or `forever`.
         :param tasks: One or more tasks to start.
         """
         rob_tasks = await self.get_tasks()
         for t in tasks:
-            assert t in rob_tasks, f"Cannot start unknown task {t}"
+            if t not in rob_tasks
+                raise Exception(f"Cannot start unknown task {t}")
 
         for rob_task in rob_tasks.values():
             if not rob_task.motiontask:
                 continue
             if rob_task.name in tasks:
                 if not rob_task.active:
                     self.activate_task(rob_task.name)
@@ -329,30 +330,32 @@
         Read a file off the controller
 
         :param filename: The filename to read
         :return: The file bytes
         """
         url="/".join([self.base_url, "fileservice", filename])
         res=await self._session.get(url)
-        assert res.is_success, f"File not found {filename}"
+        if not res.is_success:
+            raise Exception(f"File not found {filename}")
         try:            
             return res.content
         finally:
             await res.aclose()
 
     async def upload_file(self, filename: str, contents: bytes) -> None:
         """
         Upload a file to the controller
 
         :param filename: The filename to write
         :param contents: The file content bytes
         """
         url="/".join([self.base_url, "fileservice" , filename])
         res=await self._session.put(url, content=contents)
-        assert res.is_success, res.reason_phrase
+        if not res.is_success:
+            raise Exception(res.reason_phrase)
         await res.aclose()
 
     async def delete_file(self, filename: str) -> None:
         """
         Delete a file on the controller
 
         :param filename: The filename to delete
@@ -435,15 +438,16 @@
         Get the current jointtarget for specified mechunit
 
         :param mechunit: The mechanical unit to read
         :return: The current jointtarget
         """
         res_json=await self._do_get("rw/motionsystem/mechunits/" + mechunit + "/jointtarget")
         state = res_json["_embedded"]["_state"][0]
-        assert state["_type"] == "ms-jointtarget"
+        if not state["_type"] == "ms-jointtarget":
+            raise Exception("Invalid response from controller")
         robjoint=np.array([state["rax_1"], state["rax_2"], state["rax_3"], state["rax_4"], state["rax_5"], 
             state["rax_6"]], dtype=np.float64)
         extjoint=np.array([state["eax_a"], state["eax_b"], state["eax_c"], state["eax_d"], state["eax_e"], 
             state["eax_f"]], dtype=np.float64)
      
         return JointTarget(robjoint,extjoint)
         
@@ -456,31 +460,34 @@
         :param wobj: The wobj to use to compute robtarget
         :param coordinate: The coordinate system to use to compute robtarget. Can be `Base`, `World`, `Tool`, or `Wobj`
         :return: The current robtarget
 
         """
         res_json=await self._do_get(f"rw/motionsystem/mechunits/{mechunit}/robtarget?tool={tool}&wobj={wobj}&coordinate={coordinate}")
         state = res_json["_embedded"]["_state"][0]
-        assert state["_type"] == "ms-robtargets"
+        if not state["_type"] == "ms-robtargets":
+            raise Exception("Invalid response from controller")
         trans=np.array([state["x"], state["y"], state["z"]], dtype=np.float64)
         rot=np.array([state["q1"], state["q2"], state["q3"], state["q4"]], dtype=np.float64)
         robconf=np.array([state["cf1"],state["cf4"],state["cf6"],state["cfx"]], dtype=np.float64)
         extax=np.array([state["eaxa"], state["eaxb"], state["eaxc"], state["eaxd"], state["eaxe"], 
             state["eaxf"]], dtype=np.float64)
         return RobTarget(trans,rot,robconf,extax)
     
     def _rws_value_to_jointtarget(self, val):
         v1=re.match('^\\[\\[([^\\]]+)\\],\\[([^\\]]+)\\]',val)
         robax = np.deg2rad(np.fromstring(v1.groups()[0],sep=','))
         extax = np.deg2rad(np.fromstring(v1.groups()[1],sep=','))
         return JointTarget(robax,extax)
     
     def _jointtarget_to_rws_value(self, val):
-        assert np.shape(val[0]) == (6,)
-        assert np.shape(val[1]) == (6,)
+        if not np.shape(val[0]) == (6,):
+            raise Exception("Invalid jointtarget")
+        if not np.shape(val[1]) == (6,):
+            raise Exception("Invalid jointtarget")
         robax=','.join([format(x, '.4f') for x in np.rad2deg(val[0])])
         extax=','.join([format(x, '.4f') for x in np.rad2deg(val[1])])
         rws_value="[[" + robax + "],[" + extax + "]]"
         return rws_value
     
     async def get_rapid_variable_jointtarget(self, var: str, task: str = "T_ROB1"):
         """
@@ -599,15 +606,16 @@
         
         timeout_str=""
         if timeout > 0:
             timeout_str="&timeout=" + str(timeout)
         
         res_json=await self._do_get("rw/dipc/" + queue_name + "/?action=dipc-read" + timeout_str)
         for state in res_json["_embedded"]["_state"]:
-            assert state["_type"] == "dipc-read-li"
+            if not state["_type"] == "dipc-read-li":
+                raise Exception("Invalid response from controller")
      
             o.append(IpcMessage(state["dipc-data"], state["dipc-userdef"],
                 state["dipc-msgtype"], state["dipc-cmd"], state["queue-name"]))
             
             #o.append(RAPIDEventLogEntry(msg_type,code,tstamp,args,title,desc,conseqs,causes,actions))
         return o
     
@@ -666,15 +674,16 @@
         """
         t1=time.time()
         await self._do_post('users/rmmp?json=1', {'privilege': 'modify'})
         while time.time() - t1 < timeout:
             
             res_json=self._do_get('users/rmmp/poll?json=1')
             state = res_json["_embedded"]["_state"][0]
-            assert state["_type"] == "user-rmmp-poll"
+            if not state["_type"] == "user-rmmp-poll":
+                raise Exception("Invalid response from controller")
             status = state["status"]
             if status=="GRANTED":
                 await self.poll_rmmp()
                 return
             elif status!="PENDING":
                 raise Exception("User did not grant remote access")                               
             await asyncio.sleep(0.25)
@@ -710,15 +719,16 @@
                     rmmp_session.cookies.set(c)
         
         rmmp_session=self._rmmp_session        
                 
         res=await rmmp_session.get(url)
         res_json=self._process_response(res)
         state = res_json["_embedded"]["_state"][0]
-        assert state["_type"] == "user-rmmp-poll"
+        if not state["_type"] == "user-rmmp-poll":
+            raise Exception("Invalid response from controller")
                 
         if old_rmmp_session is not None:
             self._rmmp_session=rmmp_session
             self._rmmp_session_t=time.time()
             try:
                 old_rmmp_session.aclose()
             except:
@@ -783,39 +793,42 @@
                     unit = "DRV_1"
                 else:
                     signal = r.param["signal"]
                     network = r.param.get("network", "Local")
                     unit = r.param.get("unit", "DRV_1")
                 payload[f"{payload_ind}"] = f'/rw/iosystem/signals/{network}/{unit}/{signal};state'
             else:
-                assert False, "Invalid resource type"
+                raise Exception("Invalid resource type")
             payload[f"{payload_ind}-p"] = f"{r.priority.value}"
 
         payload["resources"] = [f"{i+1}" for i in range(payload_ind)]
 
                 
         url="/".join([self.base_url, "subscription"]) + "?json=1"
         res1=await self._session.post(url, data=payload)
         try:
             res=self._process_response(res1)
         finally:
             await res1.aclose()
 
-        assert res1.status_code == 201, "Subscription creation failed"
+        if not res1.status_code == 201:
+            raise Exception("Subscription creation failed")
 
         m = re.search(r'<a href="ws:\/\/.*(\/poll\/\d+)" rel="self">', res1.content.decode("ascii"))
-        assert m
+        if not m:
+            raise Exception("Invalid response from controller")
         ws_url = self.base_url.replace("http:","ws:") + m.group(1)
         
         cookie = f"-http-session-={self._session.cookies['-http-session-']}; ABBCX={self._session.cookies['ABBCX']}"
         
         header={'Cookie': cookie}
 
         async with self._websocket_lock:
-            assert self._websocket is None, "Subscription already created"
+            if not self._websocket is None: 
+                raise Exception("Subscription already created")
 
             self._websocket = await websockets.connect(
                 ws_url, 
                 extra_headers = header,
                 subprotocols=['robapi2_subscription']
             )
```

## Comparing `abb_robot_client-0.3.0.dist-info/LICENSE.txt` & `abb_robot_client-0.3.1.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `abb_robot_client-0.3.0.dist-info/METADATA` & `abb_robot_client-0.3.1.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: abb-robot-client
-Version: 0.3.0
+Name: abb_robot_client
+Version: 0.3.1
 Summary: Python client library to access ABB robots using RWS and EGM
 Home-page: https://github.com/johnwason/abb_robot_client
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: setuptools
 Requires-Dist: requests
 Requires-Dist: numpy
```

## Comparing `abb_robot_client-0.3.0.dist-info/RECORD` & `abb_robot_client-0.3.1.dist-info/RECORD`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 abb_robot_client/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 abb_robot_client/egm.py,sha256=YQ2lfB-hfY2EIkqgwVSbie5GDV86LS4jnlqJzsCLQWM,13281
-abb_robot_client/rws.py,sha256=SOVM80DdQOu0LarXZWleaA8rWLoCKz0pDxmKD_VPtdg,44041
-abb_robot_client/rws_aio.py,sha256=CauIFV69dQ1R8V_KZb6nozIxPs9LlBE9QI3XO99kthc,37208
+abb_robot_client/rws.py,sha256=YTeDzeOTCVY6jjbTuODYMQQY4IL9bjxFswWwLI3OiHY,44686
+abb_robot_client/rws_aio.py,sha256=8gOcTuQtKh0RRIMDZPBTXys3XMBUE4bO-9Xw7QCo-yc,37879
 abb_robot_client/_egm_protobuf/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 abb_robot_client/_egm_protobuf/egm_pb2.py,sha256=ohGTm_tdahAgvrxqRzwkokrCyvH8Dudc_rRYATCl0PU,8345
-abb_robot_client-0.3.0.dist-info/LICENSE.txt,sha256=dxI8ffq5vuSIafDhlRTjF0HUY6F2rpaMCmpIvRfbFIo,11601
-abb_robot_client-0.3.0.dist-info/METADATA,sha256=Zn92QgHDh3JzjSnpMW5-D3SpN50fYXfZjoswEiUGkwI,3009
-abb_robot_client-0.3.0.dist-info/WHEEL,sha256=yQN5g4mg4AybRjkgi-9yy4iQEFibGQmlz78Pik5Or-A,92
-abb_robot_client-0.3.0.dist-info/top_level.txt,sha256=3y3bFFGXpD2UMV6RqB_TgnOCGVahgM7NztcMKBj1QFs,17
-abb_robot_client-0.3.0.dist-info/RECORD,,
+abb_robot_client-0.3.1.dist-info/LICENSE.txt,sha256=dxI8ffq5vuSIafDhlRTjF0HUY6F2rpaMCmpIvRfbFIo,11601
+abb_robot_client-0.3.1.dist-info/METADATA,sha256=BZiKqqVEhCQJhUwo5f5z4dW51FdnuBM-0EIBIJw_n_Y,3009
+abb_robot_client-0.3.1.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+abb_robot_client-0.3.1.dist-info/top_level.txt,sha256=3y3bFFGXpD2UMV6RqB_TgnOCGVahgM7NztcMKBj1QFs,17
+abb_robot_client-0.3.1.dist-info/RECORD,,
```

