# Comparing `tmp/netpywork-0.0.3.tar.gz` & `tmp/netpywork-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netpywork-0.0.3.tar", last modified: Mon Apr  8 14:04:04 2024, max compression
+gzip compressed data, was "netpywork-0.0.4.tar", last modified: Wed Apr 10 14:08:19 2024, max compression
```

## Comparing `netpywork-0.0.3.tar` & `netpywork-0.0.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-04-08 14:04:03.947058 netpywork-0.0.3/
--rw-rw-rw-   0        0        0     3070 2024-04-08 14:04:03.946060 netpywork-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     2110 2024-04-08 13:25:46.000000 netpywork-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2024-04-08 14:04:03.931098 netpywork-0.0.3/netpywork/
--rw-rw-rw-   0        0        0      304 2024-04-08 13:22:33.000000 netpywork-0.0.3/netpywork/__init__.py
--rw-rw-rw-   0        0        0     4081 2024-04-08 13:15:31.000000 netpywork-0.0.3/netpywork/client.py
--rw-rw-rw-   0        0        0       84 2024-04-08 14:03:16.000000 netpywork-0.0.3/netpywork/constants.py
--rw-rw-rw-   0        0        0       93 2024-04-08 12:13:40.000000 netpywork-0.0.3/netpywork/protocol.py
--rw-rw-rw-   0        0        0     2284 2024-04-08 14:01:27.000000 netpywork-0.0.3/netpywork/sequence_manager.py
--rw-rw-rw-   0        0        0     5656 2024-04-08 13:15:27.000000 netpywork-0.0.3/netpywork/server.py
--rw-rw-rw-   0        0        0     3789 2024-04-08 13:51:29.000000 netpywork-0.0.3/netpywork/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-08 14:04:03.943068 netpywork-0.0.3/netpywork.egg-info/
--rw-rw-rw-   0        0        0     3070 2024-04-08 14:04:03.000000 netpywork-0.0.3/netpywork.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      306 2024-04-08 14:04:03.000000 netpywork-0.0.3/netpywork.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-08 14:04:03.000000 netpywork-0.0.3/netpywork.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2024-04-08 14:04:03.000000 netpywork-0.0.3/netpywork.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-08 14:04:03.948105 netpywork-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      719 2024-04-08 13:45:44.000000 netpywork-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-10 14:08:19.882687 netpywork-0.0.4/
+-rw-rw-rw-   0        0        0     1065 2024-04-10 14:08:19.881728 netpywork-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0      505 2024-04-10 13:33:55.000000 netpywork-0.0.4/README.md
+drwxrwxrwx   0        0        0        0 2024-04-10 14:08:19.865734 netpywork-0.0.4/netpywork/
+-rw-rw-rw-   0        0        0      211 2024-04-10 12:49:34.000000 netpywork-0.0.4/netpywork/__init__.py
+-rw-rw-rw-   0        0        0     5359 2024-04-10 12:36:43.000000 netpywork-0.0.4/netpywork/client.py
+-rw-rw-rw-   0        0        0       84 2024-04-10 14:07:46.000000 netpywork-0.0.4/netpywork/constants.py
+-rw-rw-rw-   0        0        0       93 2024-04-08 12:13:40.000000 netpywork-0.0.4/netpywork/protocol.py
+-rw-rw-rw-   0        0        0     2284 2024-04-08 14:01:27.000000 netpywork-0.0.4/netpywork/sequence_manager.py
+-rw-rw-rw-   0        0        0     7316 2024-04-10 12:41:31.000000 netpywork-0.0.4/netpywork/server.py
+-rw-rw-rw-   0        0        0     3799 2024-04-09 14:08:35.000000 netpywork-0.0.4/netpywork/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-10 14:08:19.877735 netpywork-0.0.4/netpywork.egg-info/
+-rw-rw-rw-   0        0        0     1065 2024-04-10 14:08:19.000000 netpywork-0.0.4/netpywork.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      306 2024-04-10 14:08:19.000000 netpywork-0.0.4/netpywork.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-10 14:08:19.000000 netpywork-0.0.4/netpywork.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2024-04-10 14:08:19.000000 netpywork-0.0.4/netpywork.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-10 14:08:19.883685 netpywork-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      719 2024-04-08 13:45:44.000000 netpywork-0.0.4/setup.py
```

### Comparing `netpywork-0.0.3/netpywork/client.py` & `netpywork-0.0.4/netpywork/client.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,28 +1,33 @@
 import socket
 from threading import Thread
 from .sequence_manager import sequence_manager
 from .utils import *
+from .utils import _utils
 from .protocol import *
 
 class client:
     def __init__(self,ip: str,port: int) -> None:
         self.ip: str = ip
         self.port: int = port
         self.address: tuple = None
+        self.auto_receive_udp: bool = True
+        self.auto_receive_tcp: bool = True
         self.on_receive = None
         self.on_connect = None
 
         self.__tcp_socket: socket.socket = socket.socket(socket.AF_INET,socket.SOCK_STREAM)
 
         self.__udp_socket: socket.socket = socket.socket(socket.AF_INET,socket.SOCK_DGRAM)
 
         self.__tcp_thread: Thread = None
         self.__udp_thread: Thread = None
 
+        self.__udp_messages: list = []
+        self.__tcp_messages: list = []
         self.__seq_manager: sequence_manager = sequence_manager()
         self.__udp_seq = 0
         self.__is_running = False
     def connect(self):
         self.__is_running = True
         self.__tcp_thread = Thread(target=self.__run_tcp)
         self.__tcp_socket.connect((self.ip,self.port))
@@ -32,66 +37,89 @@
         self.__seq_manager.add_addr(server_address)
 
         self.__udp_thread = Thread(target=self.__run_udp)
         self.__udp_socket.bind(self.address)
         self.__udp_socket.settimeout(1)
         self.__udp_thread.start()
         if(self.on_connect):
-            self.on_connect(server_address)
+            self.on_connect(server_address,self)
     def close(self):
         self.__is_running = False
         server_address = self.__tcp_socket.getpeername()
         self.__tcp_socket.close()
         self.__tcp_thread.join()
         self.__seq_manager.delete_addr(server_address)
 
         self.__udp_thread.join()
         self.__udp_socket.close()
 
         self.__seq_manager.stop()
+    def has_tcp_messages(self) -> bool:
+        return len(self.__tcp_messages) > 0
+    def read_tcp_message(self) -> tcp_msg:
+        while len(self.__tcp_messages) < 1:
+            continue
+        return self.__tcp_messages.pop(0)
+    def has_udp_messages(self) -> bool:
+        return len(self.__udp_messages) > 0
+    def read_udp_message(self) -> udp_msg:
+        while len(self.__udp_messages) < 1:
+            continue
+        return self.__udp_messages.pop(0)
+    def send(self,msg:bytes,proto:protocol = protocol.TCP):
+        if(proto == protocol.TCP):
+            self.send_reliable(msg)
+        elif(proto == protocol.UDP):
+            self.send_unreliable(msg)
+        else:
+            raise ValueError(f"Protocol type is unknown")
     def send_reliable(self,msg: bytes):
-        utils.send_tcp(self.__tcp_socket,msg)
+        _utils.send_tcp(self.__tcp_socket,msg)
     def send_unreliable(self,msg: bytes):
         msg_len = len(msg)
-        if(msg_len <= utils.MAX_UDP_PACKET_SIZE):
-            utils.send_udp(self.__udp_socket,self.address[1],(self.ip,self.port),msg,self.__udp_seq,0,1)
+        if(msg_len <= _utils.MAX_UDP_PACKET_SIZE):
+            _utils.send_udp(self.__udp_socket,self.address[1],(self.ip,self.port),msg,self.__udp_seq,0,1)
         else:
             parts = []
-            while (len(msg) > utils.MAX_UDP_PACKET_SIZE):
-                parts.append(msg[0:utils.MAX_UDP_PACKET_SIZE])
-                msg = msg[utils.MAX_UDP_PACKET_SIZE:]
+            while (len(msg) > _utils.MAX_UDP_PACKET_SIZE):
+                parts.append(msg[0:_utils.MAX_UDP_PACKET_SIZE])
+                msg = msg[_utils.MAX_UDP_PACKET_SIZE:]
             parts.append(msg)
             for i in range(len(parts)):
-                utils.send_udp(self.__udp_socket,self.address[1],(self.ip,self.port),parts[i],self.__udp_seq,i,len(parts))
+                _utils.send_udp(self.__udp_socket,self.address[1],(self.ip,self.port),parts[i],self.__udp_seq,i,len(parts))
         self.__udp_seq += 1
     def __run_udp(self):
         while self.__is_running:
             try:
-                message: udp_msg = utils.read_udp_msg(self.__udp_socket)
+                message: udp_msg = _utils.read_udp_msg(self.__udp_socket)
                 self.__seq_manager.add_seq(message.address,message.seq_no,message.data,message.seq_id)
                 if(message.amount == self.__seq_manager.get_amount(message.address,message.seq_no)):
                     # TODO : move to logging
                     # print("UDP",)
                     data = self.__seq_manager.get_result(message.address,message.seq_no)
                     result_msg = udp_msg()
                     result_msg.data = data
                     result_msg.address = message.address
                     result_msg.length = len(data)
                     result_msg.port = message.port
                     result_msg.amount = message.amount
                     result_msg.seq_no = message.seq_no
-                    if(self.on_receive):
-                        self.on_receive(result_msg,protocol.UDP)
+                    self.__udp_messages.append(result_msg)
             except:
                 continue
+            finally:
+                while(self.on_receive and self.auto_receive_udp and self.has_udp_messages()):
+                    self.on_receive(self.__udp_messages.pop(0),protocol.UDP,self)
     def __run_tcp(self):
         while self.__is_running:
             try:
-                message: tcp_msg = utils.read_tcp_msg(self.__tcp_socket)
+                message: tcp_msg = _utils.read_tcp_msg(self.__tcp_socket)
                 # Remove the length of the is end byte to match udp length which is the data length
                 message.length -= 1
+                self.__tcp_messages.append(message)
                 # TODO : move to logging
                 #print("TCP",message.data)
-                if(self.on_receive):
-                        self.on_receive(message,protocol.TCP)
             except:
-                continue
+                continue
+            finally:
+                while(self.on_receive and self.auto_receive_tcp and self.has_tcp_messages()):
+                    self.on_receive(self.__tcp_messages.pop(0),protocol.TCP,self)
```

### Comparing `netpywork-0.0.3/netpywork/sequence_manager.py` & `netpywork-0.0.4/netpywork/sequence_manager.py`

 * *Files identical despite different names*

### Comparing `netpywork-0.0.3/netpywork/server.py` & `netpywork-0.0.4/netpywork/server.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,36 +1,42 @@
 import socket
 import select
 from threading import Thread
 from .protocol import *
 from .sequence_manager import sequence_manager
 from .utils import *
+from .utils import _utils
 
 class server:
     def __init__(self,port : int) -> None:
         self.port : int = port
+        self.auto_receive_udp: bool = True
+        self.auto_receive_tcp: bool = True
         self.on_receive = None
         self.on_connect = None
         self.on_disconnect = None
 
         self.__tcp_socket: socket.socket = socket.socket(socket.AF_INET,socket.SOCK_STREAM)
         self.__tcp_socket.bind(('',port))
 
         self.__udp_socket: socket.socket = socket.socket(socket.AF_INET,socket.SOCK_DGRAM)
         self.__udp_socket.bind(('',port))
 
         self.__tcp_thread: Thread = None
         self.__udp_thread: Thread = None
 
+        self.__udp_messages: list = []
+        self.__tcp_messages: list = []
         self.__clients: list = []
         self.__seq_manager: sequence_manager = sequence_manager()
         self.__addr_to_sock: dict = {}
         self.__udp_seq = 0
         self.__is_running = False
-
+    def get_clients(self):
+        return [x.getpeername() for x in self.__clients]
     def run(self):
         self.__is_running = True
         self.__tcp_thread = Thread(target=self.__run_tcp)
         self.__tcp_socket.listen()
         self.__tcp_thread.start()
 
         self.__udp_thread = Thread(target=self.__run_udp)
@@ -41,88 +47,116 @@
         self.__tcp_socket.close()
         self.__tcp_thread.join()
         for client in self.__clients:
             self.__seq_manager.delete_addr(client.getpeername())
         self.__udp_thread.join()
         self.__udp_socket.close()
         self.__seq_manager.stop()
+    def has_tcp_messages(self) -> bool:
+        return len(self.__tcp_messages) > 0
+    def read_tcp_message(self) -> tcp_msg:
+        while len(self.__tcp_messages) < 1:
+            continue
+        return self.__tcp_messages.pop(0)
+    def has_udp_messages(self) -> bool:
+        return len(self.__udp_messages) > 0
+    def read_udp_message(self) -> udp_msg:
+        while len(self.__udp_messages) < 1:
+            continue
+        return self.__udp_messages.pop(0)
+    def send_all(self,msg:bytes,proto:protocol = protocol.TCP,exceptions: list = []):
+        for client in self.get_clients():
+            if(client in exceptions):
+                continue
+            self.send(msg,client,proto)
+    def send(self,msg:bytes,address:tuple,proto:protocol = protocol.TCP):
+        if(proto == protocol.TCP):
+            self.send_reliable(msg,address)
+        elif(proto == protocol.UDP):
+            self.send_unreliable(msg,address)
+        else:
+            raise ValueError(f"Protocol type is unknown")
     def send_reliable(self,msg: bytes,address:tuple):
-        utils.send_tcp(self.__addr_to_sock[address],msg)
+        _utils.send_tcp(self.__addr_to_sock[address],msg)
     def __get_actual_address(self,address):
         return self.__addr_to_sock[address].getpeername()
     def send_unreliable(self,msg: bytes,address:tuple):
         msg_len = len(msg)
-        if(msg_len <= utils.MAX_UDP_PACKET_SIZE):
-            utils.send_udp(self.__udp_socket,self.__tcp_socket.getsockname()[1],self.__get_actual_address(address),msg,self.__udp_seq,0,1)
+        if(msg_len <= _utils.MAX_UDP_PACKET_SIZE):
+            _utils.send_udp(self.__udp_socket,self.__tcp_socket.getsockname()[1],self.__get_actual_address(address),msg,self.__udp_seq,0,1)
         else:
             parts = []
-            while (len(msg) > utils.MAX_UDP_PACKET_SIZE):
-                parts.append(msg[0:utils.MAX_UDP_PACKET_SIZE])
-                msg = msg[utils.MAX_UDP_PACKET_SIZE:]
+            while (len(msg) > _utils.MAX_UDP_PACKET_SIZE):
+                parts.append(msg[0:_utils.MAX_UDP_PACKET_SIZE])
+                msg = msg[_utils.MAX_UDP_PACKET_SIZE:]
             parts.append(msg)
             for i in range(len(parts)):
-                utils.send_udp(self.__udp_socket,self.__tcp_socket.getsockname()[1],self.__get_actual_address(address),parts[i],self.__udp_seq,i,len(parts))
+                _utils.send_udp(self.__udp_socket,self.__tcp_socket.getsockname()[1],self.__get_actual_address(address),parts[i],self.__udp_seq,i,len(parts))
         self.__udp_seq += 1
     def __has_client(self,address):
         for client in self.__clients:
             client_address = client.getpeername()
             if(address == client_address):
                 return True
         return False
     
     def __delete_client(self,sock):
         self.__clients.remove(sock)
         socket_addr = sock.getpeername()
         self.__seq_manager.delete_addr(socket_addr)
         del self.__addr_to_sock[socket_addr]
         if(self.on_disconnect):
-            self.on_disconnect(socket_addr)
+            self.on_disconnect(socket_addr,self)
     def __run_udp(self):
         while self.__is_running:
             try:
-                message: udp_msg = utils.read_udp_msg(self.__udp_socket)
+                message: udp_msg = _utils.read_udp_msg(self.__udp_socket)
                 if(not self.__has_client(message.address)):
                     continue
                 self.__seq_manager.add_seq(message.address,message.seq_no,message.data,message.seq_id)
                 if(message.amount == self.__seq_manager.get_amount(message.address,message.seq_no)):
                     # TODO : move to logging
                     # print("UDP",)
                     data = self.__seq_manager.get_result(message.address,message.seq_no)
                     result_msg = udp_msg()
                     result_msg.data = data
                     result_msg.address = message.address
                     result_msg.length = len(data)
                     result_msg.port = message.port
                     result_msg.amount = message.amount
                     result_msg.seq_no = message.seq_no
-                    if(self.on_receive):
-                        self.on_receive(result_msg,protocol.UDP)
+                    self.__udp_messages.append(result_msg)
             except:
                 continue
+            finally:
+                while(self.on_receive and self.auto_receive_udp and self.has_udp_messages()):
+                    self.on_receive(self.__udp_messages.pop(0),protocol.UDP,self)
     def __run_tcp(self):
         while self.__is_running:
             try:
                 sockets,_,_ = select.select(self.__clients + [self.__tcp_socket],[],[])
                 for sock in sockets:
                     if(sock == self.__tcp_socket):
                         client_socket,_ = sock.accept()
                         self.__clients.append(client_socket)
                         client_addr = client_socket.getpeername()
                         self.__seq_manager.add_addr(client_addr)
                         self.__addr_to_sock[client_addr] = client_socket
                         if(self.on_connect):
-                            self.on_connect(client_addr)
+                            self.on_connect(client_addr,self)
                     else:
                         try:
-                            message: tcp_msg = utils.read_tcp_msg(sock)
+                            message: tcp_msg = _utils.read_tcp_msg(sock)
                             # Remove the length of the is end byte to match udp length which is the data length
                             message.length -= 1
+                            self.__tcp_messages.append(message)
                             # TODO : move to logging
-                            # print("TCP",message.data)
-                            if(self.on_receive):
-                                self.on_receive(message,protocol.TCP)
+                            #print("TCP",message.data)
                             if(message.closing):
                                 self.__delete_client(sock)
                         except:
                             self.__delete_client(sock)
+                        finally:
+                            while(self.on_receive and self.auto_receive_tcp and self.has_tcp_messages()):
+                                self.on_receive(self.__tcp_messages.pop(0),protocol.TCP,self)
             except:
                 continue
```

### Comparing `netpywork-0.0.3/netpywork/utils.py` & `netpywork-0.0.4/netpywork/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -35,15 +35,15 @@
     """
     length:int = -1
     port:int = -1
     address: tuple = ()
     data:bytes = None
     closing:bool = False
 
-class utils:
+class _utils:
     MAX_UDP_PACKET_SIZE = 65507 - 4 - 2 - 4 - 2 - 2
     def peek_udp(sock: socket.socket,size: int):
             buffer = bytearray(size)
             # Windows workaround as it errors out with errorcode 10040 even though it peeked the msg
             try:
                 sock.recv_into(buffer,size,socket.MSG_PEEK)
             except OSError as ex:
@@ -54,26 +54,26 @@
         if(length == -1):
             length = len(byte)
         result = byte[0:length]
         for _ in range(length):
             del byte[0]
         return bytes(result)
     def read_udp_msg(socket: socket.socket) -> udp_msg:
-        length = utils.peek_udp(socket,4)
+        length = _utils.peek_udp(socket,4)
         # MSG Size + Size len
         length = int.from_bytes(length,"big") + 4
         result,result_address = socket.recvfrom(length)
         result = bytearray(result)
-        utils.read_message(result,4)
-        port = int.from_bytes(utils.read_message(result,2),"big")
+        _utils.read_message(result,4)
+        port = int.from_bytes(_utils.read_message(result,2),"big")
         full_address = (result_address[0],port)
-        seqno = int.from_bytes(utils.read_message(result,4),"big")
-        seqid = int.from_bytes(utils.read_message(result,2),"big")
-        amount = int.from_bytes(utils.read_message(result,2),"big")
-        result = utils.read_message(result)
+        seqno = int.from_bytes(_utils.read_message(result,4),"big")
+        seqid = int.from_bytes(_utils.read_message(result,2),"big")
+        amount = int.from_bytes(_utils.read_message(result,2),"big")
+        result = _utils.read_message(result)
         udp_message = udp_msg()
         udp_message.address = full_address
         udp_message.data = result
         udp_message.amount = amount
         udp_message.length = length
         udp_message.port = port
         udp_message.seq_no = seqno
@@ -82,16 +82,16 @@
     def read_tcp_msg(socket: socket.socket):
         length = socket.recv(4)
         length = int.from_bytes(length,"big")
         buffer = socket.recv(length)
         while len(buffer) < length:
             buffer += socket.recv(1)
         buffer = bytearray(buffer)
-        close_con = int.from_bytes(utils.read_message(buffer,1),"big") == 1
-        result = utils.read_message(buffer)
+        close_con = int.from_bytes(_utils.read_message(buffer,1),"big") == 1
+        result = _utils.read_message(buffer)
         address = socket.getpeername()
         tcp_message = tcp_msg()
         tcp_message.address = address
         tcp_message.closing = close_con
         tcp_message.data = result
         tcp_message.length = length
         tcp_message.port = address[1]
```

### Comparing `netpywork-0.0.3/setup.py` & `netpywork-0.0.4/setup.py`

 * *Files identical despite different names*

