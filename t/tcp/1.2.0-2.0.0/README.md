# Comparing `tmp/tcp-1.2.0.tar.gz` & `tmp/tcp-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tcp-1.2.0.tar", last modified: Tue Apr 23 09:03:52 2024, max compression
+gzip compressed data, was "dist/tcp-2.0.0.tar", last modified: Fri May 10 15:31:18 2024, max compression
```

## Comparing `tcp-1.2.0.tar` & `tcp-2.0.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-04-23 09:03:52.000000 tcp-1.2.0/
--rw-r--r--   0 moky       (501) staff       (20)      445 2024-04-23 09:03:52.000000 tcp-1.2.0/PKG-INFO
--rw-r--r--   0 moky       (501) staff       (20)       19 2020-07-17 14:54:20.000000 tcp-1.2.0/README.md
--rw-r--r--   0 moky       (501) staff       (20)       38 2024-04-23 09:03:52.000000 tcp-1.2.0/setup.cfg
--rw-r--r--   0 moky       (501) staff       (20)      849 2024-04-23 08:31:29.000000 tcp-1.2.0/setup.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-04-23 09:03:52.000000 tcp-1.2.0/tcp/
--rw-r--r--   0 moky       (501) staff       (20)     2828 2023-01-13 12:35:58.000000 tcp-1.2.0/tcp/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     7571 2024-03-13 10:03:59.000000 tcp-1.2.0/tcp/channel.py
--rw-r--r--   0 moky       (501) staff       (20)    10086 2024-04-23 08:31:56.000000 tcp-1.2.0/tcp/hub.py
--rw-r--r--   0 moky       (501) staff       (20)     4471 2024-03-06 15:36:17.000000 tcp-1.2.0/tcp/startrek.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-04-23 09:03:52.000000 tcp-1.2.0/tcp.egg-info/
--rw-r--r--   0 moky       (501) staff       (20)      445 2024-04-23 09:03:52.000000 tcp-1.2.0/tcp.egg-info/PKG-INFO
--rw-r--r--   0 moky       (501) staff       (20)      210 2024-04-23 09:03:52.000000 tcp-1.2.0/tcp.egg-info/SOURCES.txt
--rw-r--r--   0 moky       (501) staff       (20)        1 2024-04-23 09:03:52.000000 tcp-1.2.0/tcp.egg-info/dependency_links.txt
--rw-r--r--   0 moky       (501) staff       (20)       16 2024-04-23 09:03:52.000000 tcp-1.2.0/tcp.egg-info/requires.txt
--rw-r--r--   0 moky       (501) staff       (20)        4 2024-04-23 09:03:52.000000 tcp-1.2.0/tcp.egg-info/top_level.txt
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-10 15:31:18.000000 tcp-2.0.0/
+-rw-r--r--   0 moky       (501) staff       (20)      445 2024-05-10 15:31:18.000000 tcp-2.0.0/PKG-INFO
+-rw-r--r--   0 moky       (501) staff       (20)       19 2020-07-17 14:54:20.000000 tcp-2.0.0/README.md
+-rw-r--r--   0 moky       (501) staff       (20)       38 2024-05-10 15:31:18.000000 tcp-2.0.0/setup.cfg
+-rw-r--r--   0 moky       (501) staff       (20)      849 2024-05-10 15:30:49.000000 tcp-2.0.0/setup.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-10 15:31:18.000000 tcp-2.0.0/tcp/
+-rw-r--r--   0 moky       (501) staff       (20)     2828 2023-01-13 12:35:58.000000 tcp-2.0.0/tcp/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     7631 2024-05-07 09:35:54.000000 tcp-2.0.0/tcp/channel.py
+-rw-r--r--   0 moky       (501) staff       (20)    10581 2024-05-09 18:52:45.000000 tcp-2.0.0/tcp/hub.py
+-rw-r--r--   0 moky       (501) staff       (20)     4519 2024-05-07 14:35:33.000000 tcp-2.0.0/tcp/startrek.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-10 15:31:18.000000 tcp-2.0.0/tcp.egg-info/
+-rw-r--r--   0 moky       (501) staff       (20)      445 2024-05-10 15:31:18.000000 tcp-2.0.0/tcp.egg-info/PKG-INFO
+-rw-r--r--   0 moky       (501) staff       (20)      210 2024-05-10 15:31:18.000000 tcp-2.0.0/tcp.egg-info/SOURCES.txt
+-rw-r--r--   0 moky       (501) staff       (20)        1 2024-05-10 15:31:18.000000 tcp-2.0.0/tcp.egg-info/dependency_links.txt
+-rw-r--r--   0 moky       (501) staff       (20)       16 2024-05-10 15:31:18.000000 tcp-2.0.0/tcp.egg-info/requires.txt
+-rw-r--r--   0 moky       (501) staff       (20)        4 2024-05-10 15:31:18.000000 tcp-2.0.0/tcp.egg-info/top_level.txt
```

### Comparing `tcp-1.2.0/setup.py` & `tcp-2.0.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     ~~~
 
     Transmission Control Protocol
 """
 
 from setuptools import setup, find_packages
 
-__version__ = '1.2.0'
+__version__ = '2.0.0'
 __author__ = 'Albert Moky'
 __contact__ = 'albert.moky@gmail.com'
 
 with open('README.md', 'r') as fh:
     readme = fh.read()
 
 setup(
@@ -30,10 +30,10 @@
     packages=find_packages(),
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
     ],
     install_requires=[
-        'startrek>=1.2.0'
+        'startrek>=2.0.0'
     ]
 )
```

### Comparing `tcp-1.2.0/tcp/__init__.py` & `tcp-2.0.0/tcp/__init__.py`

 * *Files identical despite different names*

### Comparing `tcp-1.2.0/tcp/channel.py` & `tcp-2.0.0/tcp/channel.py`

 * *Files 8% similar despite different names*

```diff
@@ -89,77 +89,77 @@
                 # print('[NET] socket error: remote peer reset socket %s' % sock)
                 return socket.error('remote peer reset socket %s' % sock)
 
 
 class StreamChannelReader(ChannelReader):
 
     # noinspection PyMethodMayBeStatic
-    def _try_read(self, max_len: int, sock: socket.socket) -> Optional[bytes]:
+    async def _try_read(self, max_len: int, sock: socket.socket) -> Optional[bytes]:
         try:
             return sock.recv(max_len)
         except socket.error as error:
             error = ChannelChecker.check_error(error=error, sock=sock)
             if error is None:
                 # received nothing
                 return None
             else:
                 # connection lost?
                 raise error
 
     # Override
-    def read(self, max_len: int) -> Optional[bytes]:
+    async def read(self, max_len: int) -> Optional[bytes]:
         sock = self.sock
         if sock is None or is_closed(sock=sock):
             raise ConnectionError('socket closed')
         # 1. try to read data
-        data = self._try_read(max_len=max_len, sock=sock)
+        data = await self._try_read(max_len=max_len, sock=sock)
         # 2. check data
         error = ChannelChecker.check_data(data=data, sock=sock)
         if error is not None:
             # connection lost!
             raise error
         # OK
         return data
 
     # Override
-    def receive(self, max_len: int) -> Tuple[Optional[bytes], Optional[SocketAddress]]:
-        data = self.read(max_len=max_len)
+    async def receive(self, max_len: int) -> Tuple[Optional[bytes], Optional[SocketAddress]]:
+        data = await self.read(max_len=max_len)
         if data is None or len(data) == 0:
             return None, None
         else:
             return data, self.remote_address
 
 
 class StreamChannelWriter(ChannelWriter):
 
     # noinspection PyMethodMayBeStatic
-    def _try_write(self, data: bytes, sock: socket.socket) -> int:
+    async def _try_write(self, data: bytes, sock: socket.socket) -> int:
         try:
             return sock.send(data)
         except socket.error as error:
             error = ChannelChecker.check_error(error=error, sock=sock)
             if error is not None:
                 # connection lost?
                 raise error
             # buffer overflow!
             return 0
 
     # Override
-    def write(self, data: bytes) -> int:
+    async def write(self, data: bytes) -> int:
         """ Return the number of bytes sent;
             this may be less than len(data) if the network is busy. """
         sock = self.sock
         if sock is None or is_closed(sock=sock):
             raise ConnectionError('socket closed')
         # sent = sock.sendall(data)
         sent = 0
         rest = len(data)
         # assert rest > 0, 'cannot send empty data'
         while True:  # while is_opened(sock=sock):
-            cnt = self._try_write(data=data, sock=sock)
+            cnt = await self._try_write(data=data, sock=sock)
             # check send result
             if cnt <= 0:
                 # buffer overflow?
                 break
             # something sent, check remaining data
             sent += cnt
             rest -= cnt
@@ -175,20 +175,20 @@
         elif cnt < 0:
             assert cnt == -1, 'sent error: %d' % cnt
             return -1
         else:
             return 0
 
     # Override
-    def send(self, data: bytes, target: SocketAddress) -> int:
+    async def send(self, data: bytes, target: SocketAddress) -> int:
         # TCP channel will be always connected
         # so the target address must be the remote address
         remote = self.remote_address
         assert target is None or target == remote, 'target error: %s, remote=%s' % (target, remote)
-        return self.write(data=data)
+        return await self.write(data=data)
 
 
 class StreamChannel(BaseChannel):
     """ Stream Channel """
 
     # Override
     def _create_reader(self):
```

### Comparing `tcp-1.2.0/tcp/hub.py` & `tcp-2.0.0/tcp/hub.py`

 * *Files 8% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 import socket
 import threading
 import time
 from abc import ABC
 from typing import Optional, Iterable
 
 from startrek.types import SocketAddress, AddressPairMap
-from startrek.fsm import Runnable, Daemon
+from startrek.fsm import Runnable, Runner, Daemon
 from startrek import Channel, BaseChannel
 from startrek import Connection, ConnectionDelegate
 from startrek import BaseConnection, ActiveConnection
 from startrek import BaseHub
 
 from .channel import StreamChannel
 
@@ -48,28 +48,28 @@
 
     # Override
     def set(self, item: Optional[Channel],
             remote: Optional[SocketAddress], local: Optional[SocketAddress]) -> Optional[Channel]:
         # 1. remove cached item
         cached = super().remove(item=item, remote=remote, local=local)
         if cached is not None and cached is not item:
-            cached.close()
+            Runner.async_run(coroutine=cached.close())
         # 2. set new item
         old = super().set(item=item, remote=remote, local=local)
         assert old is None, 'should not happen: %s' % old
         return cached
 
     # Override
     def remove(self, item: Optional[Channel],
                remote: Optional[SocketAddress], local: Optional[SocketAddress]) -> Optional[Channel]:
         cached = super().remove(item=item, remote=remote, local=local)
         if cached is not None and cached is not item:
-            cached.close()
+            Runner.async_run(coroutine=cached.close())
         if item is not None:
-            item.close()
+            Runner.async_run(coroutine=item.close())
         return cached
 
 
 # noinspection PyAbstractClass
 class StreamHub(BaseHub, ABC):
     """ Base Stream Hub """
 
@@ -110,29 +110,28 @@
         """ cache channel """
         return self.__channel_pool.set(item=channel, remote=remote, local=local)
 
 
 class ServerHub(StreamHub, Runnable):
     """ Stream Server Hub """
 
-    def __init__(self, delegate: ConnectionDelegate, daemonic: bool = True):
+    def __init__(self, delegate: ConnectionDelegate):
         super().__init__(delegate=delegate)
         self.__local = None   # SocketAddress
         self.__master = None  # socket.socket
-        # running thread
-        self.__daemon = Daemon(target=self, daemonic=daemonic)
+        self.__daemon = Daemon(target=self)
         self.__running = False
 
     # Override
     def _create_connection(self, remote: SocketAddress, local: Optional[SocketAddress]) -> Optional[Connection]:
         conn = BaseConnection(remote=remote, local=local)
         conn.delegate = self.delegate  # gate
         return conn
 
-    def bind(self, address: Optional[SocketAddress] = None, host: Optional[str] = None, port: Optional[int] = 0):
+    async def bind(self, address: Optional[SocketAddress] = None, host: Optional[str] = None, port: Optional[int] = 0):
         if address is None:
             if port > 0:
                 assert host is not None, 'host should not be empty'
                 address = (host, port)
             else:
                 address = self.__local
                 assert address is not None, 'local address not set'
@@ -164,47 +163,56 @@
     #   Threading
     #
 
     @property
     def running(self) -> bool:
         return self.__running
 
-    def start(self):
-        self.stop()
+    async def start(self):
+        assert not self.__running, 'server hub is running: %s' % self
+        # 1. mark this hub to running
         self.__running = True
-        return self.__daemon.start()
+        # 2. start an async task for this hub
+        self.__daemon.start()
+        # await self.run()
 
-    def stop(self):
+    async def stop(self):
+        # 1. mark this hub to stopped
         self.__running = False
+        # 2. waiting for the hub to stop
+        await Runner.sleep(seconds=0.25)
+        # 3. cancel the async task
         self.__daemon.stop()
 
     # Override
-    def run(self):
+    async def run(self):
         self.__running = True
         while self.running:
             try:
                 master = self._get_master()
                 sock, address = master.accept()
-                if sock is not None:
-                    self._accept(remote=address, local=self.local_address, sock=sock)
+                if sock is None:
+                    await Runner.sleep(seconds=Runner.INTERVAL_NORMAL)
+                else:
+                    await self._accept(remote=address, local=self.local_address, sock=sock)
             except socket.error as error:
                 print('[TCP] socket error: %s' % error)
             except Exception as error:
                 print('[TCP] accept error: %s' % error)
 
-    def _accept(self, remote: SocketAddress, local: SocketAddress, sock: socket.socket):
+    async def _accept(self, remote: SocketAddress, local: SocketAddress, sock: socket.socket):
         # override for user-customized channel
         channel = self._create_channel(remote=remote, local=local)
         assert isinstance(channel, BaseChannel), 'channel error: %s, %s' % (remote, channel)
         # set socket for this channel
-        channel.set_socket(sock=sock)
+        await channel.set_socket(sock=sock)
         self._set_channel(channel=channel, remote=channel.remote_address, local=channel.local_address)
 
     # Override
-    def open(self, remote: Optional[SocketAddress], local: Optional[SocketAddress]) -> Optional[Channel]:
+    async def open(self, remote: Optional[SocketAddress], local: Optional[SocketAddress]) -> Optional[Channel]:
         assert remote is not None, 'remote address empty: %s, %s' % (remote, local)
         return self._get_channel(remote=remote, local=local)
 
 
 class ClientHub(StreamHub):
     """ Stream Client Hub """
 
@@ -215,40 +223,40 @@
     # Override
     def _create_connection(self, remote: SocketAddress, local: Optional[SocketAddress]) -> Optional[Connection]:
         conn = ActiveConnection(remote=remote, local=local)
         conn.delegate = self.delegate  # gate
         return conn
 
     # Override
-    def open(self, remote: Optional[SocketAddress], local: Optional[SocketAddress]) -> Optional[Channel]:
+    async def open(self, remote: Optional[SocketAddress], local: Optional[SocketAddress]) -> Optional[Channel]:
         assert remote is not None, 'remote address empty: %s, %s' % (remote, local)
         # try to get channel
         with self.__lock:
             old = self._get_channel(remote=remote, local=local)
             if old is None:
                 # create channel with socket
                 channel = self._create_channel(remote=remote, local=local)
                 self._set_channel(channel, remote=remote, local=local)
             else:
                 channel = old
         if old is None:
             # initialize socket
-            sock = create_socket(remote=remote, local=local)
+            sock = await create_socket(remote=remote, local=local)
             if sock is None:
                 print('[TCP] failed to prepare socket: %s -> %s' % (local, remote))
                 self._remove_channel(channel, remote=remote, local=local)
                 channel = None
             else:
                 assert isinstance(channel, BaseChannel), 'channel error: %s, %s' % (remote, channel)
                 # set socket for this channel
-                channel.set_socket(sock=sock)
+                await channel.set_socket(sock=sock)
         return channel
 
 
-def create_socket(remote: SocketAddress, local: Optional[SocketAddress]) -> Optional[socket.socket]:
+async def create_socket(remote: SocketAddress, local: Optional[SocketAddress]) -> Optional[socket.socket]:
     try:
         sock = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
         sock.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEPORT, 0)
         sock.setblocking(True)
         # try to bind
         if local is not None:
             sock.bind(local)
```

### Comparing `tcp-1.2.0/tcp/startrek.py` & `tcp-2.0.0/tcp/startrek.py`

 * *Files 4% similar despite different names*

```diff
@@ -102,42 +102,42 @@
     def _get_arrivals(self, data: bytes) -> List[Arrival]:
         if data is None or len(data) == 0:
             return []
         else:
             return [self._create_arrival(pack=data)]
 
     # Override
-    def _check_arrival(self, ship: Arrival) -> Optional[Arrival]:
+    async def _check_arrival(self, ship: Arrival) -> Optional[Arrival]:
         assert isinstance(ship, PlainArrival), 'arrival ship error: %s' % ship
         data = ship.package
         if len(data) == 4:
             if data == PING:
                 # PING -> PONG
-                self.send(payload=PONG, priority=DeparturePriority.SLOWER)
+                await self.send(payload=PONG, priority=DeparturePriority.SLOWER)
                 return None
             if data == PONG or data == NOOP:
                 # ignore
                 return None
         return ship
 
     #
     #   Sending
     #
 
-    def send(self, payload: bytes, priority: int) -> bool:
+    async def send(self, payload: bytes, priority: int) -> bool:
         """ sending payload with priority """
         ship = self._create_departure(pack=payload, priority=priority)
-        return self.send_ship(ship=ship)
+        return await self.send_ship(ship=ship)
 
     # Override
-    def send_data(self, payload: Union[bytes, bytearray]) -> bool:
-        return self.send(payload=payload, priority=DeparturePriority.NORMAL)
+    async def send_data(self, payload: Union[bytes, bytearray]) -> bool:
+        return await self.send(payload=payload, priority=DeparturePriority.NORMAL)
 
     # Override
-    def heartbeat(self):
-        self.send(payload=PING, priority=DeparturePriority.SLOWER)
+    async def heartbeat(self):
+        await self.send(payload=PING, priority=DeparturePriority.SLOWER)
 
 
 PING = b'PING'
 PONG = b'PONG'
 NOOP = b'NOOP'
 OK = b'OK'
```

