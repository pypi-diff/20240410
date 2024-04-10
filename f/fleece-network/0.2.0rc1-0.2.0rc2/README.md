# Comparing `tmp/fleece_network-0.2.0rc1.tar.gz` & `tmp/fleece_network-0.2.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fleece_network-0.2.0rc1.tar", max compression
+gzip compressed data, was "fleece_network-0.2.0rc2.tar", max compression
```

## Comparing `fleece_network-0.2.0rc1.tar` & `fleece_network-0.2.0rc2.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0      327 2024-04-06 11:22:41.411003 fleece_network-0.2.0rc1/README.md
--rw-r--r--   0        0        0        0 2024-04-06 11:22:41.411003 fleece_network-0.2.0rc1/fleece_network/__init__.py
--rw-r--r--   0        0        0      349 2024-04-06 11:22:41.411003 fleece_network-0.2.0rc1/fleece_network/aioice/__init__.py
--rw-r--r--   0        0        0     4060 2024-04-06 11:22:41.411003 fleece_network-0.2.0rc1/fleece_network/aioice/candidate.py
--rw-r--r--   0        0        0    41238 2024-04-06 11:22:41.411003 fleece_network-0.2.0rc1/fleece_network/aioice/ice.py
--rw-r--r--   0        0        0     6655 2024-04-06 11:22:41.411003 fleece_network-0.2.0rc1/fleece_network/aioice/mdns.py
--rw-r--r--   0        0        0    12298 2024-04-06 11:22:41.411003 fleece_network-0.2.0rc1/fleece_network/aioice/stun.py
--rw-r--r--   0        0        0    15077 2024-04-06 11:22:41.411003 fleece_network-0.2.0rc1/fleece_network/aioice/turn.py
--rw-r--r--   0        0        0      264 2024-04-06 11:22:41.411003 fleece_network-0.2.0rc1/fleece_network/aioice/utils.py
--rw-r--r--   0        0        0     1226 2024-04-06 11:22:41.411003 fleece_network-0.2.0rc1/fleece_network/aiortc/__init__.py
--rw-r--r--   0        0        0      824 2024-04-06 11:22:41.411003 fleece_network-0.2.0rc1/fleece_network/aiortc/clock.py
--rw-r--r--   0        0        0      180 2024-04-06 11:22:41.411003 fleece_network-0.2.0rc1/fleece_network/aiortc/exceptions.py
--rw-r--r--   0        0        0    21027 2024-04-06 11:22:41.415003 fleece_network-0.2.0rc1/fleece_network/aiortc/rate.py
--rw-r--r--   0        0        0     1040 2024-04-06 11:22:41.415003 fleece_network-0.2.0rc1/fleece_network/aiortc/rtcconfiguration.py
--rw-r--r--   0        0        0     6531 2024-04-06 11:22:41.415003 fleece_network-0.2.0rc1/fleece_network/aiortc/rtcdatachannel.py
--rw-r--r--   0        0        0    13595 2024-04-06 11:22:41.415003 fleece_network-0.2.0rc1/fleece_network/aiortc/rtcdtlstransport.py
--rw-r--r--   0        0        0    11425 2024-04-06 11:22:41.415003 fleece_network-0.2.0rc1/fleece_network/aiortc/rtcicetransport.py
--rw-r--r--   0        0        0    32180 2024-04-06 11:22:41.415003 fleece_network-0.2.0rc1/fleece_network/aiortc/rtcpeerconnection.py
--rw-r--r--   0        0        0     4612 2024-04-06 11:22:41.415003 fleece_network-0.2.0rc1/fleece_network/aiortc/rtcrtpparameters.py
--rw-r--r--   0        0        0    61599 2024-04-06 11:22:41.415003 fleece_network-0.2.0rc1/fleece_network/aiortc/rtcsctptransport.py
--rw-r--r--   0        0        0      500 2024-04-06 11:22:41.415003 fleece_network-0.2.0rc1/fleece_network/aiortc/rtcsessiondescription.py
--rw-r--r--   0        0        0    24050 2024-04-06 11:22:41.415003 fleece_network-0.2.0rc1/fleece_network/aiortc/rtp.py
--rw-r--r--   0        0        0    21763 2024-04-06 11:22:41.415003 fleece_network-0.2.0rc1/fleece_network/aiortc/sdp.py
--rw-r--r--   0        0        0     2879 2024-04-06 11:22:41.415003 fleece_network-0.2.0rc1/fleece_network/aiortc/stats.py
--rw-r--r--   0        0        0      978 2024-04-06 11:22:41.415003 fleece_network-0.2.0rc1/fleece_network/aiortc/utils.py
--rw-r--r--   0        0        0      716 2024-04-06 11:22:41.415003 fleece_network-0.2.0rc1/fleece_network/messages.py
--rw-r--r--   0        0        0    21451 2024-04-06 11:22:41.415003 fleece_network-0.2.0rc1/fleece_network/peer.py
--rw-r--r--   0        0        0        0 2024-04-06 11:22:41.415003 fleece_network-0.2.0rc1/fleece_network/py.typed
--rw-r--r--   0        0        0     2144 2024-04-06 11:22:41.415003 fleece_network-0.2.0rc1/fleece_network/signaling.py
--rw-r--r--   0        0        0      479 2024-04-06 11:22:41.415003 fleece_network-0.2.0rc1/pyproject.toml
--rw-r--r--   0        0        0      983 1970-01-01 00:00:00.000000 fleece_network-0.2.0rc1/PKG-INFO
+-rw-r--r--   0        0        0      327 2024-04-10 06:38:19.579817 fleece_network-0.2.0rc2/README.md
+-rw-r--r--   0        0        0        0 2024-04-10 06:38:19.579817 fleece_network-0.2.0rc2/fleece_network/__init__.py
+-rw-r--r--   0        0        0      349 2024-04-10 06:38:19.579817 fleece_network-0.2.0rc2/fleece_network/aioice/__init__.py
+-rw-r--r--   0        0        0     4060 2024-04-10 06:38:19.579817 fleece_network-0.2.0rc2/fleece_network/aioice/candidate.py
+-rw-r--r--   0        0        0    41684 2024-04-10 06:38:19.579817 fleece_network-0.2.0rc2/fleece_network/aioice/ice.py
+-rw-r--r--   0        0        0     6655 2024-04-10 06:38:19.579817 fleece_network-0.2.0rc2/fleece_network/aioice/mdns.py
+-rw-r--r--   0        0        0    12369 2024-04-10 06:38:19.579817 fleece_network-0.2.0rc2/fleece_network/aioice/stun.py
+-rw-r--r--   0        0        0    15077 2024-04-10 06:38:19.579817 fleece_network-0.2.0rc2/fleece_network/aioice/turn.py
+-rw-r--r--   0        0        0      264 2024-04-10 06:38:19.579817 fleece_network-0.2.0rc2/fleece_network/aioice/utils.py
+-rw-r--r--   0        0        0     1226 2024-04-10 06:38:19.579817 fleece_network-0.2.0rc2/fleece_network/aiortc/__init__.py
+-rw-r--r--   0        0        0      824 2024-04-10 06:38:19.579817 fleece_network-0.2.0rc2/fleece_network/aiortc/clock.py
+-rw-r--r--   0        0        0      180 2024-04-10 06:38:19.579817 fleece_network-0.2.0rc2/fleece_network/aiortc/exceptions.py
+-rw-r--r--   0        0        0    21027 2024-04-10 06:38:19.579817 fleece_network-0.2.0rc2/fleece_network/aiortc/rate.py
+-rw-r--r--   0        0        0     1040 2024-04-10 06:38:19.579817 fleece_network-0.2.0rc2/fleece_network/aiortc/rtcconfiguration.py
+-rw-r--r--   0        0        0     6531 2024-04-10 06:38:19.579817 fleece_network-0.2.0rc2/fleece_network/aiortc/rtcdatachannel.py
+-rw-r--r--   0        0        0    13595 2024-04-10 06:38:19.579817 fleece_network-0.2.0rc2/fleece_network/aiortc/rtcdtlstransport.py
+-rw-r--r--   0        0        0    11425 2024-04-10 06:38:19.579817 fleece_network-0.2.0rc2/fleece_network/aiortc/rtcicetransport.py
+-rw-r--r--   0        0        0    32180 2024-04-10 06:38:19.579817 fleece_network-0.2.0rc2/fleece_network/aiortc/rtcpeerconnection.py
+-rw-r--r--   0        0        0     4612 2024-04-10 06:38:19.579817 fleece_network-0.2.0rc2/fleece_network/aiortc/rtcrtpparameters.py
+-rw-r--r--   0        0        0    61599 2024-04-10 06:38:19.579817 fleece_network-0.2.0rc2/fleece_network/aiortc/rtcsctptransport.py
+-rw-r--r--   0        0        0      500 2024-04-10 06:38:19.579817 fleece_network-0.2.0rc2/fleece_network/aiortc/rtcsessiondescription.py
+-rw-r--r--   0        0        0    24050 2024-04-10 06:38:19.579817 fleece_network-0.2.0rc2/fleece_network/aiortc/rtp.py
+-rw-r--r--   0        0        0    21763 2024-04-10 06:38:19.579817 fleece_network-0.2.0rc2/fleece_network/aiortc/sdp.py
+-rw-r--r--   0        0        0     2879 2024-04-10 06:38:19.579817 fleece_network-0.2.0rc2/fleece_network/aiortc/stats.py
+-rw-r--r--   0        0        0      978 2024-04-10 06:38:19.579817 fleece_network-0.2.0rc2/fleece_network/aiortc/utils.py
+-rw-r--r--   0        0        0      716 2024-04-10 06:38:19.579817 fleece_network-0.2.0rc2/fleece_network/messages.py
+-rw-r--r--   0        0        0    21803 2024-04-10 06:38:19.579817 fleece_network-0.2.0rc2/fleece_network/peer.py
+-rw-r--r--   0        0        0        0 2024-04-10 06:38:19.579817 fleece_network-0.2.0rc2/fleece_network/py.typed
+-rw-r--r--   0        0        0     2144 2024-04-10 06:38:19.579817 fleece_network-0.2.0rc2/fleece_network/signaling.py
+-rw-r--r--   0        0        0      479 2024-04-10 06:38:19.583817 fleece_network-0.2.0rc2/pyproject.toml
+-rw-r--r--   0        0        0      983 1970-01-01 00:00:00.000000 fleece_network-0.2.0rc2/PKG-INFO
```

### Comparing `fleece_network-0.2.0rc1/fleece_network/aioice/candidate.py` & `fleece_network-0.2.0rc2/fleece_network/aioice/candidate.py`

 * *Files identical despite different names*

### Comparing `fleece_network-0.2.0rc1/fleece_network/aioice/ice.py` & `fleece_network-0.2.0rc2/fleece_network/aioice/ice.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,28 +4,31 @@
 import ipaddress
 import logging
 import random
 import secrets
 import socket
 import threading
 from itertools import count
+import time
 from typing import Dict, List, Optional, Set, Text, Tuple, Union, cast
 
 import ifaddr
 
 from . import mdns, stun, turn
 from .candidate import Candidate, candidate_foundation, candidate_priority
 from .utils import random_string
 
 logger = logging.getLogger(__name__)
 
 ICE_COMPLETED = 1
 ICE_FAILED = 2
 
-CONSENT_FAILURES = 6
+CONSENT_DELAY = 0.4
+CONSENT_ALPHA = 0.9
+CONSENT_FAILURES = 3
 CONSENT_INTERVAL = 5
 
 connection_id = count()
 protocol_id = count()
 
 _mdns = threading.local()
 
@@ -236,25 +239,26 @@
 
     async def request(
         self,
         request: stun.Message,
         addr: Tuple[str, int],
         integrity_key: Optional[bytes] = None,
         retransmissions=None,
+        delay=None,
     ) -> Tuple[stun.Message, Tuple[str, int]]:
         """
         Execute a STUN transaction and return the response.
         """
         assert request.transaction_id not in self.transactions
 
         if integrity_key is not None:
             request.add_message_integrity(integrity_key)
 
         transaction = stun.Transaction(
-            request, addr, self, retransmissions=retransmissions
+            request, addr, self, retransmissions=retransmissions, delay=delay
         )
         self.transactions[request.transaction_id] = transaction
         try:
             return await transaction.run()
         finally:
             del self.transactions[request.transaction_id]
 
@@ -995,36 +999,45 @@
             self._components = seen_components
 
     async def query_consent(self) -> None:
         """
         Periodically check consent (RFC 7675).
         """
         failures = 0
+        delay = CONSENT_DELAY
+        alpha = CONSENT_ALPHA
         while True:
             # randomize between 0.8 and 1.2 times CONSENT_INTERVAL
             await asyncio.sleep(CONSENT_INTERVAL * (0.8 + 0.4 * random.random()))
 
             for pair in self._nominated.values():
                 request = self.build_request(pair, nominate=False)
                 try:
                     assert self.remote_password
+                    begin = time.time()
                     await pair.protocol.request(
                         request,
                         pair.remote_addr,
                         integrity_key=self.remote_password.encode("utf8"),
                         retransmissions=0,
+                        delay=delay * 2,
                     )
+                    end = time.time()
                     failures = 0
                 except stun.TransactionError:
                     failures += 1
+                    self.__log_info("Fail with consent delay %s", delay)
                 if failures >= CONSENT_FAILURES:
                     self.__log_info("Consent to send expired")
                     self._query_consent_task = None
                     return await self.close()
 
+                # adjust adaptive delay
+                delay = delay * alpha + (1 - alpha) * (end - begin)
+
     def data_received(self, data: bytes, component: int) -> None:
         self._queue.put_nowait((data, component))
 
     def request_received(
         self,
         message: stun.Message,
         addr: Tuple[str, int],
```

### Comparing `fleece_network-0.2.0rc1/fleece_network/aioice/mdns.py` & `fleece_network-0.2.0rc2/fleece_network/aioice/mdns.py`

 * *Files identical despite different names*

### Comparing `fleece_network-0.2.0rc1/fleece_network/aioice/stun.py` & `fleece_network-0.2.0rc2/fleece_network/aioice/stun.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import asyncio
 import binascii
 import enum
 import hmac
 import ipaddress
 from collections import OrderedDict
 from struct import pack, unpack
+import time
 from typing import Callable, Dict, List, Optional, Protocol, Tuple
 
 from .utils import random_transaction_id
 
 COOKIE = 0x2112A442
 FINGERPRINT_LENGTH = 8
 FINGERPRINT_XOR = 0x5354554E
@@ -275,21 +276,22 @@
 class Transaction:
     def __init__(
         self,
         request: Message,
         addr: Tuple[str, int],
         protocol: SendStun,
         retransmissions: Optional[int] = None,
+        delay: Optional[float] = None,
     ) -> None:
         self.__addr = addr
         self.__future: asyncio.Future[Tuple[Message, Tuple[str, int]]] = (
             asyncio.Future()
         )
         self.__request = request
-        self.__timeout_delay = RETRY_RTO
+        self.__timeout_delay = delay if delay else RETRY_RTO
         self.__timeout_handle: Optional[asyncio.TimerHandle] = None
         self.__protocol = protocol
         self.__tries = 0
         self.__tries_max = 1 + (
             retransmissions if retransmissions is not None else RETRY_MAX
         )
```

### Comparing `fleece_network-0.2.0rc1/fleece_network/aioice/turn.py` & `fleece_network-0.2.0rc2/fleece_network/aioice/turn.py`

 * *Files identical despite different names*

### Comparing `fleece_network-0.2.0rc1/fleece_network/aiortc/__init__.py` & `fleece_network-0.2.0rc2/fleece_network/aiortc/__init__.py`

 * *Files identical despite different names*

### Comparing `fleece_network-0.2.0rc1/fleece_network/aiortc/clock.py` & `fleece_network-0.2.0rc2/fleece_network/aiortc/clock.py`

 * *Files identical despite different names*

### Comparing `fleece_network-0.2.0rc1/fleece_network/aiortc/rate.py` & `fleece_network-0.2.0rc2/fleece_network/aiortc/rate.py`

 * *Files identical despite different names*

### Comparing `fleece_network-0.2.0rc1/fleece_network/aiortc/rtcconfiguration.py` & `fleece_network-0.2.0rc2/fleece_network/aiortc/rtcconfiguration.py`

 * *Files identical despite different names*

### Comparing `fleece_network-0.2.0rc1/fleece_network/aiortc/rtcdatachannel.py` & `fleece_network-0.2.0rc2/fleece_network/aiortc/rtcdatachannel.py`

 * *Files identical despite different names*

### Comparing `fleece_network-0.2.0rc1/fleece_network/aiortc/rtcdtlstransport.py` & `fleece_network-0.2.0rc2/fleece_network/aiortc/rtcdtlstransport.py`

 * *Files identical despite different names*

### Comparing `fleece_network-0.2.0rc1/fleece_network/aiortc/rtcicetransport.py` & `fleece_network-0.2.0rc2/fleece_network/aiortc/rtcicetransport.py`

 * *Files identical despite different names*

### Comparing `fleece_network-0.2.0rc1/fleece_network/aiortc/rtcpeerconnection.py` & `fleece_network-0.2.0rc2/fleece_network/aiortc/rtcpeerconnection.py`

 * *Files identical despite different names*

### Comparing `fleece_network-0.2.0rc1/fleece_network/aiortc/rtcrtpparameters.py` & `fleece_network-0.2.0rc2/fleece_network/aiortc/rtcrtpparameters.py`

 * *Files identical despite different names*

### Comparing `fleece_network-0.2.0rc1/fleece_network/aiortc/rtcsctptransport.py` & `fleece_network-0.2.0rc2/fleece_network/aiortc/rtcsctptransport.py`

 * *Files identical despite different names*

### Comparing `fleece_network-0.2.0rc1/fleece_network/aiortc/rtp.py` & `fleece_network-0.2.0rc2/fleece_network/aiortc/rtp.py`

 * *Files identical despite different names*

### Comparing `fleece_network-0.2.0rc1/fleece_network/aiortc/sdp.py` & `fleece_network-0.2.0rc2/fleece_network/aiortc/sdp.py`

 * *Files identical despite different names*

### Comparing `fleece_network-0.2.0rc1/fleece_network/aiortc/stats.py` & `fleece_network-0.2.0rc2/fleece_network/aiortc/stats.py`

 * *Files identical despite different names*

### Comparing `fleece_network-0.2.0rc1/fleece_network/aiortc/utils.py` & `fleece_network-0.2.0rc2/fleece_network/aiortc/utils.py`

 * *Files identical despite different names*

### Comparing `fleece_network-0.2.0rc1/fleece_network/messages.py` & `fleece_network-0.2.0rc2/fleece_network/messages.py`

 * *Files identical despite different names*

### Comparing `fleece_network-0.2.0rc1/fleece_network/peer.py` & `fleece_network-0.2.0rc2/fleece_network/peer.py`

 * *Files 4% similar despite different names*

```diff
@@ -101,14 +101,16 @@
             except HTTPException as e:
                 await self._send(id, Response(e.detail, e.status_code, e.headers))
             else:
                 if isinstance(result, BaseModel):
                     await self._send(id, Response(result.model_dump_json()))
                 elif isinstance(result, str):
                     await self._send(id, Response(result))
+                elif result is None:
+                    await self._send(id, Response())
                 else:  # assertion
                     raise ValueError("Invalid result type")
 
 
 class Connection(ABC):
     @abstractmethod
     async def send(self, op: str, data: P) -> Response:
@@ -125,17 +127,15 @@
         self.counter = 0
 
         def on_open():
             self.isopen.set()
             self._logger.info("Outward data channel %s opens", self.label())
 
         async def on_message(raw: bytes):
-            self._logger.info(
-                "Outward data channel %s receives message: %s", self.label(), raw
-            )
+            self._logger.info("Outward data channel %s receives message", self.label())
             reply: SimpleReply = pickle.loads(raw)
             async with self.lock:
                 send_stream = self.map.pop(reply.id)
                 await send_stream.send(reply.data)
 
         async def on_close():
             self._logger.warning("Outward data channel %s closes", self.label())
@@ -151,17 +151,15 @@
         await self.isopen.wait()
         send_stream, recv_stream = create_memory_object_stream[Response]()
         async with self.lock:
             id = self.counter
             self.counter += 1
             self.map[id] = send_stream
         self.channel.send(pickle.dumps(SimpleRequest(id, op, data)))
-        self._logger.info(
-            "Outward data channel %s sends message: %s %s", self.label(), op, data
-        )
+        self._logger.info("Outward data channel %s sends message: %s", self.label(), op)
         return await recv_stream.receive()
 
     def close(self):
         self.channel.close()
 
 
 class InwardDataChannel(Inward):
@@ -190,15 +188,15 @@
 
     def label(self) -> str:
         return self.channel.label
 
     async def _send(self, id: int, reply: Response):
         """Although it's not an async function, it requires the existence of an event loop."""
 
-        self._logger.info("Channel %s sends message: %s", self.label(), reply)
+        self._logger.info("Inward data channel %s sends message", self.label())
         self.channel.send(pickle.dumps(SimpleReply(id, reply)))
 
 
 class OutwardLoopback(Outward):
     def __init__(
         self,
         label: str,
@@ -221,27 +219,31 @@
 
         async def onmessage():
             async for message in recv_stream:
                 id, reply = message
                 async with self.lock:
                     send_stream = self.map.pop(id)
                 tg.start_soon(send_stream.send, reply)
+                self._logger.info(
+                    "Outward data channel %s receives message", self.label()
+                )
 
         tg.start_soon(onmessage)
 
     def label(self) -> str:
         return self._label
 
     async def send(self, op: str, data: P) -> Response:
         send_stream, recv_stream = create_memory_object_stream[Response]()
         async with self.lock:
             id = self.counter
             self.counter += 1
             self.map[id] = send_stream
         await self.send_stream.send((id, op, data))
+        self._logger.info("Outward data channel %s sends message: %s", self.label(), op)
         return await recv_stream.receive()
 
     def close(self):
         self.send_stream.close()
         self.recv_stream.close()
 
 
@@ -269,15 +271,15 @@
     def label(self) -> str:
         return self._label
 
     async def _send(self, id: int, reply: Response):
         """Although it's not an async function, it requires the existence of an event loop."""
 
         await self.send_stream.send((id, reply))
-        self._logger.info("Channel %s sends message: %s", self.label(), reply)
+        self._logger.info("Inward data channel %s sends message", self.label())
 
 
 class PeerConnection(Connection):
     class State:
         DEAD = 0
         OFFERED = 1
         WAITING = 2
@@ -342,15 +344,15 @@
 
                     self._logger.info(
                         "Connection (%s, %s) changes state to CONNECTED",
                         self.from_id,
                         self.to_id,
                     )
                 elif pc.connectionState == "failed" or pc.connectionState == "closed":
-                    await self._reset_inner()
+                    self._reset_inner()
 
                     self._logger.info(
                         "Connection (%s, %s) changes state to FAILED",
                         self.from_id,
                         self.to_id,
                     )
 
@@ -541,15 +543,17 @@
             signature = inspect.signature(func)
             type_hints = get_type_hints(func)
 
             parsed_args = []
             for param_name, arg in zip(signature.parameters, args):
                 model_cls = type_hints[param_name]
                 if isinstance(arg, (str, bytes)):
-                    parsed_arg = model_cls.parse_raw(arg)
+                    parsed_arg = model_cls.model_validate_json(arg)
+                elif isinstance(arg, dict):
+                    parsed_arg = model_cls.model_validate(arg)
                 else:
                     parsed_arg = arg
                 parsed_args.append(parsed_arg)
             return func(*parsed_args)
 
         if asyncio.iscoroutinefunction(func):
```

### Comparing `fleece_network-0.2.0rc1/fleece_network/signaling.py` & `fleece_network-0.2.0rc2/fleece_network/signaling.py`

 * *Files identical despite different names*

### Comparing `fleece_network-0.2.0rc1/PKG-INFO` & `fleece_network-0.2.0rc2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fleece-network
-Version: 0.2.0rc1
+Version: 0.2.0rc2
 Summary: P2P socket built on aiortc.
 Author: Linyu Wu
 Author-email: celve03@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

