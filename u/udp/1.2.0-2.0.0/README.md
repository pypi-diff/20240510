# Comparing `tmp/udp-1.2.0.tar.gz` & `tmp/udp-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/udp-1.2.0.tar", last modified: Tue Apr 23 09:04:45 2024, max compression
+gzip compressed data, was "dist/udp-2.0.0.tar", last modified: Fri May 10 15:33:25 2024, max compression
```

## Comparing `udp-1.2.0.tar` & `udp-2.0.0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-04-23 09:04:45.000000 udp-1.2.0/
--rw-r--r--   0 moky       (501) staff       (20)      438 2024-04-23 09:04:45.000000 udp-1.2.0/PKG-INFO
--rw-r--r--   0 moky       (501) staff       (20)       19 2020-07-17 14:54:20.000000 udp-1.2.0/README.md
--rw-r--r--   0 moky       (501) staff       (20)       38 2024-04-23 09:04:45.000000 udp-1.2.0/setup.cfg
--rw-r--r--   0 moky       (501) staff       (20)      835 2024-04-23 08:32:23.000000 udp-1.2.0/setup.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-04-23 09:04:45.000000 udp-1.2.0/udp/
--rw-r--r--   0 moky       (501) staff       (20)     2832 2023-01-13 16:49:26.000000 udp-1.2.0/udp/__init__.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-04-23 09:04:45.000000 udp-1.2.0/udp/ba/
--rw-r--r--   0 moky       (501) staff       (20)     1944 2021-09-16 08:10:15.000000 udp-1.2.0/udp/ba/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     9574 2024-02-26 16:22:28.000000 udp-1.2.0/udp/ba/array.py
--rw-r--r--   0 moky       (501) staff       (20)     3345 2021-09-16 08:10:15.000000 udp-1.2.0/udp/ba/convert.py
--rw-r--r--   0 moky       (501) staff       (20)     7763 2023-01-13 16:00:06.000000 udp-1.2.0/udp/ba/data.py
--rw-r--r--   0 moky       (501) staff       (20)     7219 2023-01-13 15:58:57.000000 udp-1.2.0/udp/ba/helper.py
--rw-r--r--   0 moky       (501) staff       (20)     8436 2021-09-16 08:10:15.000000 udp-1.2.0/udp/ba/integer.py
--rw-r--r--   0 moky       (501) staff       (20)     4852 2021-09-16 08:10:15.000000 udp-1.2.0/udp/ba/mutable.py
--rw-r--r--   0 moky       (501) staff       (20)    15161 2023-01-13 16:00:39.000000 udp-1.2.0/udp/ba/utils.py
--rw-r--r--   0 moky       (501) staff       (20)     9393 2024-03-06 16:08:05.000000 udp-1.2.0/udp/channel.py
--rw-r--r--   0 moky       (501) staff       (20)     8167 2024-04-22 17:50:56.000000 udp-1.2.0/udp/hub.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-04-23 09:04:45.000000 udp-1.2.0/udp/mtp/
--rw-r--r--   0 moky       (501) staff       (20)     1678 2021-09-16 08:10:15.000000 udp-1.2.0/udp/mtp/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)    15551 2023-01-02 14:11:01.000000 udp-1.2.0/udp/mtp/header.py
--rw-r--r--   0 moky       (501) staff       (20)     4505 2023-01-02 14:11:01.000000 udp-1.2.0/udp/mtp/package.py
--rw-r--r--   0 moky       (501) staff       (20)     8003 2023-01-02 14:11:01.000000 udp-1.2.0/udp/mtp/packer.py
--rw-r--r--   0 moky       (501) staff       (20)     6708 2021-09-16 08:10:15.000000 udp-1.2.0/udp/mtp/protocol.py
--rw-r--r--   0 moky       (501) staff       (20)    11523 2024-03-06 16:13:05.000000 udp-1.2.0/udp/startrek.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-04-23 09:04:45.000000 udp-1.2.0/udp.egg-info/
--rw-r--r--   0 moky       (501) staff       (20)      438 2024-04-23 09:04:45.000000 udp-1.2.0/udp.egg-info/PKG-INFO
--rw-r--r--   0 moky       (501) staff       (20)      442 2024-04-23 09:04:45.000000 udp-1.2.0/udp.egg-info/SOURCES.txt
--rw-r--r--   0 moky       (501) staff       (20)        1 2024-04-23 09:04:45.000000 udp-1.2.0/udp.egg-info/dependency_links.txt
--rw-r--r--   0 moky       (501) staff       (20)       16 2024-04-23 09:04:45.000000 udp-1.2.0/udp.egg-info/requires.txt
--rw-r--r--   0 moky       (501) staff       (20)        4 2024-04-23 09:04:45.000000 udp-1.2.0/udp.egg-info/top_level.txt
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-10 15:33:25.000000 udp-2.0.0/
+-rw-r--r--   0 moky       (501) staff       (20)      438 2024-05-10 15:33:25.000000 udp-2.0.0/PKG-INFO
+-rw-r--r--   0 moky       (501) staff       (20)       19 2020-07-17 14:54:20.000000 udp-2.0.0/README.md
+-rw-r--r--   0 moky       (501) staff       (20)       38 2024-05-10 15:33:25.000000 udp-2.0.0/setup.cfg
+-rw-r--r--   0 moky       (501) staff       (20)      835 2024-05-10 15:32:29.000000 udp-2.0.0/setup.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-10 15:33:25.000000 udp-2.0.0/udp/
+-rw-r--r--   0 moky       (501) staff       (20)     2832 2023-01-13 16:49:26.000000 udp-2.0.0/udp/__init__.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-10 15:33:25.000000 udp-2.0.0/udp/ba/
+-rw-r--r--   0 moky       (501) staff       (20)     1944 2021-09-16 08:10:15.000000 udp-2.0.0/udp/ba/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     9574 2024-02-26 16:22:28.000000 udp-2.0.0/udp/ba/array.py
+-rw-r--r--   0 moky       (501) staff       (20)     3345 2021-09-16 08:10:15.000000 udp-2.0.0/udp/ba/convert.py
+-rw-r--r--   0 moky       (501) staff       (20)     7763 2023-01-13 16:00:06.000000 udp-2.0.0/udp/ba/data.py
+-rw-r--r--   0 moky       (501) staff       (20)     7219 2023-01-13 15:58:57.000000 udp-2.0.0/udp/ba/helper.py
+-rw-r--r--   0 moky       (501) staff       (20)     8436 2021-09-16 08:10:15.000000 udp-2.0.0/udp/ba/integer.py
+-rw-r--r--   0 moky       (501) staff       (20)     4852 2021-09-16 08:10:15.000000 udp-2.0.0/udp/ba/mutable.py
+-rw-r--r--   0 moky       (501) staff       (20)    15161 2023-01-13 16:00:39.000000 udp-2.0.0/udp/ba/utils.py
+-rw-r--r--   0 moky       (501) staff       (20)     9489 2024-05-07 14:50:50.000000 udp-2.0.0/udp/channel.py
+-rw-r--r--   0 moky       (501) staff       (20)     8265 2024-05-09 15:46:48.000000 udp-2.0.0/udp/hub.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-10 15:33:25.000000 udp-2.0.0/udp/mtp/
+-rw-r--r--   0 moky       (501) staff       (20)     1678 2021-09-16 08:10:15.000000 udp-2.0.0/udp/mtp/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)    15551 2023-01-02 14:11:01.000000 udp-2.0.0/udp/mtp/header.py
+-rw-r--r--   0 moky       (501) staff       (20)     4505 2023-01-02 14:11:01.000000 udp-2.0.0/udp/mtp/package.py
+-rw-r--r--   0 moky       (501) staff       (20)     8003 2023-01-02 14:11:01.000000 udp-2.0.0/udp/mtp/packer.py
+-rw-r--r--   0 moky       (501) staff       (20)     6708 2021-09-16 08:10:15.000000 udp-2.0.0/udp/mtp/protocol.py
+-rw-r--r--   0 moky       (501) staff       (20)    11702 2024-05-07 15:14:23.000000 udp-2.0.0/udp/startrek.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-10 15:33:25.000000 udp-2.0.0/udp.egg-info/
+-rw-r--r--   0 moky       (501) staff       (20)      438 2024-05-10 15:33:25.000000 udp-2.0.0/udp.egg-info/PKG-INFO
+-rw-r--r--   0 moky       (501) staff       (20)      442 2024-05-10 15:33:25.000000 udp-2.0.0/udp.egg-info/SOURCES.txt
+-rw-r--r--   0 moky       (501) staff       (20)        1 2024-05-10 15:33:25.000000 udp-2.0.0/udp.egg-info/dependency_links.txt
+-rw-r--r--   0 moky       (501) staff       (20)       16 2024-05-10 15:33:25.000000 udp-2.0.0/udp.egg-info/requires.txt
+-rw-r--r--   0 moky       (501) staff       (20)        4 2024-05-10 15:33:25.000000 udp-2.0.0/udp.egg-info/top_level.txt
```

### Comparing `udp-1.2.0/setup.py` & `udp-2.0.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     ~~~
 
     User Datagram Protocol
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

### Comparing `udp-1.2.0/udp/__init__.py` & `udp-2.0.0/udp/__init__.py`

 * *Files identical despite different names*

### Comparing `udp-1.2.0/udp/ba/__init__.py` & `udp-2.0.0/udp/ba/__init__.py`

 * *Files identical despite different names*

### Comparing `udp-1.2.0/udp/ba/array.py` & `udp-2.0.0/udp/ba/array.py`

 * *Files identical despite different names*

### Comparing `udp-1.2.0/udp/ba/convert.py` & `udp-2.0.0/udp/ba/convert.py`

 * *Files identical despite different names*

### Comparing `udp-1.2.0/udp/ba/data.py` & `udp-2.0.0/udp/ba/data.py`

 * *Files identical despite different names*

### Comparing `udp-1.2.0/udp/ba/helper.py` & `udp-2.0.0/udp/ba/helper.py`

 * *Files identical despite different names*

### Comparing `udp-1.2.0/udp/ba/integer.py` & `udp-2.0.0/udp/ba/integer.py`

 * *Files identical despite different names*

### Comparing `udp-1.2.0/udp/ba/mutable.py` & `udp-2.0.0/udp/ba/mutable.py`

 * *Files identical despite different names*

### Comparing `udp-1.2.0/udp/ba/utils.py` & `udp-2.0.0/udp/ba/utils.py`

 * *Files identical despite different names*

### Comparing `udp-1.2.0/udp/channel.py` & `udp-2.0.0/udp/channel.py`

 * *Files 9% similar despite different names*

```diff
@@ -90,104 +90,104 @@
                 return socket.error('remote peer reset socket %s' % sock)
 
 
 class PacketChannelReader(ChannelReader):
     """ Datagram Packet Channel Reader """
 
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
 
     # noinspection PyMethodMayBeStatic
-    def _try_receive(self, max_len: int, sock: socket.socket) -> Tuple[Optional[bytes], Optional[SocketAddress]]:
+    async def _try_receive(self, max_len: int, sock: socket.socket) -> Tuple[Optional[bytes], Optional[SocketAddress]]:
         try:
             return sock.recvfrom(max_len)
         except socket.error as error:
             error = ChannelChecker.check_error(error=error, sock=sock)
             if error is None:
                 # received nothing
                 return None, None
             else:
                 # connection lost?
                 raise error
 
-    def _receive_from(self, max_len: int, sock: socket.socket) -> Tuple[Optional[bytes], Optional[SocketAddress]]:
-        data, remote = self._try_receive(max_len=max_len, sock=sock)
+    async def _receive_from(self, max_len: int, sock: socket.socket) -> Tuple[Optional[bytes], Optional[SocketAddress]]:
+        data, remote = await self._try_receive(max_len=max_len, sock=sock)
         # check data
         error = ChannelChecker.check_data(data=data, sock=sock)
         if error is None:
             # OK
             return data, remote
         else:
             # connection lost!
             raise error
 
     # Override
-    def receive(self, max_len: int) -> Tuple[Optional[bytes], Optional[SocketAddress]]:
+    async def receive(self, max_len: int) -> Tuple[Optional[bytes], Optional[SocketAddress]]:
         remote = self.remote_address
         if remote is None:
             # not connect (UDP)
-            return self._receive_from(max_len=max_len, sock=self.sock)
+            return await self._receive_from(max_len=max_len, sock=self.sock)
         else:
             # connected (TCP/UDP)
-            return self.read(max_len=max_len), remote
+            return await self.read(max_len=max_len), remote
 
 
 class PacketChannelWriter(ChannelWriter):
     """ Datagram Packet Channel Writer """
 
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
@@ -203,39 +203,39 @@
         elif cnt < 0:
             assert cnt == -1, 'sent error: %d' % cnt
             return -1
         else:
             return 0
 
     # noinspection PyMethodMayBeStatic
-    def _try_send(self, data: bytes, target: SocketAddress, sock: socket.socket) -> int:
+    async def _try_send(self, data: bytes, target: SocketAddress, sock: socket.socket) -> int:
         try:
             return sock.sendto(data, target)
         except socket.error as error:
             error = ChannelChecker.check_error(error=error, sock=sock)
             if error is None:
                 # buffer overflow!
                 return -1
             else:
                 # connection lost?
                 raise error
 
     # Override
-    def send(self, data: bytes, target: SocketAddress) -> int:
+    async def send(self, data: bytes, target: SocketAddress) -> int:
         remote = self.remote_address
         if remote is None:
             # not connect (UDP)
             assert target is not None, 'target missed for unbound channel'
-            return self._try_send(data=data, target=target, sock=self.sock)
+            return await self._try_send(data=data, target=target, sock=self.sock)
         else:
             # connected (TCP/UDP)
             remote = self.remote_address
             assert target is None or target == remote, 'target error: %s, remote=%s' % (target, remote)
             # return sock.send(data)
-            return self._try_write(data=data, sock=self.sock)
+            return await self._try_write(data=data, sock=self.sock)
 
 
 class PacketChannel(BaseChannel):
     """ Datagram Packet Channel """
 
     # Override
     def _create_reader(self):
```

### Comparing `udp-1.2.0/udp/hub.py` & `udp-2.0.0/udp/hub.py`

 * *Files 3% similar despite different names*

```diff
@@ -29,14 +29,15 @@
 # ==============================================================================
 
 import socket
 from abc import ABC
 from typing import Optional, Iterable
 
 from startrek.types import SocketAddress, AddressPairMap
+from startrek.fsm import Runner
 from startrek import Channel, BaseChannel
 from startrek import Connection, ConnectionDelegate
 from startrek import BaseConnection, ActiveConnection
 from startrek import BaseHub
 
 from .channel import PacketChannel
 
@@ -86,28 +87,28 @@
 
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
 class PacketHub(BaseHub, ABC):
     """ Base Datagram Hub """
 
@@ -115,29 +116,29 @@
         super().__init__(delegate=delegate)
         self.__channel_pool = self._create_channel_pool()
 
     # noinspection PyMethodMayBeStatic
     def _create_channel_pool(self):
         return ChannelPool()
 
-    def bind(self, address: SocketAddress = None, host: str = None, port: int = 0):
+    async def bind(self, address: SocketAddress = None, host: str = None, port: int = 0):
         if address is None:
             assert host is not None and port > 0, 'address error: (%s:%d)' % (host, port)
             address = (host, port)
         channel = self.__channel_pool.get(remote=None, local=address)
         if channel is None:
             channel = self._create_channel(remote=None, local=address)
             assert isinstance(channel, BaseChannel), 'channel error: %s, %s' % (address, channel)
             sock = socket.socket(socket.AF_INET, socket.SOCK_DGRAM)
             sock.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEPORT, 1)
             sock.setblocking(True)
             sock.bind(address)
             sock.setblocking(False)
             # set socket for this channel
-            channel.set_socket(sock=sock)
+            await channel.set_socket(sock=sock)
             self.__channel_pool.set(item=channel, remote=None, local=address)
 
     #
     #   Channel
     #
 
     # noinspection PyMethodMayBeStatic
@@ -172,26 +173,25 @@
     # Override
     def _create_connection(self, remote: SocketAddress, local: Optional[SocketAddress]) -> Optional[Connection]:
         conn = BaseConnection(remote=remote, local=local)
         conn.delegate = self.delegate  # gate
         return conn
 
     # Override
-    def open(self, remote: Optional[SocketAddress], local: Optional[SocketAddress]) -> Optional[Channel]:
+    async def open(self, remote: Optional[SocketAddress], local: Optional[SocketAddress]) -> Optional[Channel]:
         # get channel with direction (remote, local)
         return self._get_channel(remote=remote, local=local)
 
 
 class ClientHub(PacketHub):
     """ Datagram Client Hub """
 
     # Override
     def _create_connection(self, remote: SocketAddress, local: Optional[SocketAddress]) -> Optional[Connection]:
         conn = ActiveConnection(remote=remote, local=local)
         conn.delegate = self.delegate  # gate
-        conn.start(hub=self)  # start FSM
         return conn
 
     # Override
-    def open(self, remote: Optional[SocketAddress], local: Optional[SocketAddress]) -> Optional[Channel]:
+    async def open(self, remote: Optional[SocketAddress], local: Optional[SocketAddress]) -> Optional[Channel]:
         # get channel with direction (remote, local)
         return self._get_channel(remote=remote, local=local)
```

### Comparing `udp-1.2.0/udp/mtp/__init__.py` & `udp-2.0.0/udp/mtp/__init__.py`

 * *Files identical despite different names*

### Comparing `udp-1.2.0/udp/mtp/header.py` & `udp-2.0.0/udp/mtp/header.py`

 * *Files identical despite different names*

### Comparing `udp-1.2.0/udp/mtp/package.py` & `udp-2.0.0/udp/mtp/package.py`

 * *Files identical despite different names*

### Comparing `udp-1.2.0/udp/mtp/packer.py` & `udp-2.0.0/udp/mtp/packer.py`

 * *Files identical despite different names*

### Comparing `udp-1.2.0/udp/mtp/protocol.py` & `udp-2.0.0/udp/mtp/protocol.py`

 * *Files identical despite different names*

### Comparing `udp-1.2.0/udp/startrek.py` & `udp-2.0.0/udp/startrek.py`

 * *Files 4% similar despite different names*

```diff
@@ -178,15 +178,15 @@
         pack = self._parse_package(data=data)
         if pack is None:
             return []
         else:
             return [self._create_arrival(pack=pack)]
 
     # Override
-    def _check_arrival(self, ship: Arrival) -> Optional[Arrival]:
+    async def _check_arrival(self, ship: Arrival) -> Optional[Arrival]:
         assert isinstance(ship, PackageArrival), 'arrival ship error: %s' % ship
         pack = ship.package
         if pack is None:
             fragments = ship.fragments
             if fragments is None or len(fragments) == 0:
                 raise ValueError('fragments error: %s' % ship)
             # each ship can carry one fragment only
@@ -195,49 +195,49 @@
         head = pack.head
         body = pack.body
         data_type = head.data_type
         if data_type.is_command_response:
             # process CommandResponse
             #       'PONG'
             #       'OK'
-            self._check_response(ship=ship)
+            await self._check_response(ship=ship)
             if body == PONG or body == OK:
                 # command responded
                 return None
             # extra data in CommandResponse?
             # let the caller to process it
         elif data_type.is_command:
             # process Command:
             #       'PING'
             #       '...'
             if body == PING:
                 # PING -> PONG
-                self._respond_command(sn=head.sn, body=PONG)
+                await self._respond_command(sn=head.sn, body=PONG)
                 return None
             else:
                 # respond for Command
-                self._respond_command(sn=head.sn, body=OK)
+                await self._respond_command(sn=head.sn, body=OK)
             # Unknown Command?
             # let the caller to process it
         elif data_type.is_message_response:
             # process MessageResponse
             #       'OK'
             #       'AGAIN'
             if body == AGAIN:
                 # TODO: reset retries?
                 return None
-            self._check_response(ship=ship)
+            await self._check_response(ship=ship)
             if body == OK:
                 # message responded
                 return None
             # extra data in MessageResponse?
             # let the caller to process it
         else:
             # respond for Message/Fragment
-            self._respond_message(sn=head.sn, pages=head.pages, index=head.index)
+            await self._respond_message(sn=head.sn, pages=head.pages, index=head.index)
             if data_type.is_message_fragment:
                 # assemble MessageFragment with cached fragments to completed Message
                 # let the caller to process the completed message
                 return self._assemble_arrival(ship=ship)
             assert data_type.is_message, 'unknown data type: %s' % data_type
             # let the caller to process the message
 
@@ -248,15 +248,15 @@
             elif body == PING or body == PONG:
                 # FIXME: these bodies should be in a Command
                 # ignore them
                 return None
         return ship
 
     #
-    #   Sending
+    #   Packing
     #
 
     # noinspection PyMethodMayBeStatic
     def _create_command(self, body: Union[bytes, bytearray]) -> Package:
         return Package.new(data_type=DataType.COMMAND, body=Data(buffer=body))
 
     # noinspection PyMethodMayBeStatic
@@ -267,44 +267,48 @@
     def _create_command_response(self, sn: TransactionID, body: bytes) -> Package:
         return Package.new(data_type=DataType.COMMAND_RESPONSE, sn=sn, body=Data(buffer=body))
 
     # noinspection PyMethodMayBeStatic
     def _create_message_response(self, sn: TransactionID, pages: int, index: int) -> Package:
         return Package.new(data_type=DataType.MESSAGE_RESPONSE, sn=sn, pages=pages, index=index, body=Data(buffer=OK))
 
+    #
+    #   Sending
+    #
+
     # protected
-    def _respond_command(self, sn: TransactionID, body: bytes):
+    async def _respond_command(self, sn: TransactionID, body: bytes) -> bool:
         pack = self._create_command_response(sn=sn, body=body)
-        self.send_package(pack=pack)
+        return await self.send_package(pack=pack)
 
     # protected
-    def _respond_message(self, sn: TransactionID, pages: int, index: int):
+    async def _respond_message(self, sn: TransactionID, pages: int, index: int) -> bool:
         pack = self._create_message_response(sn=sn, pages=pages, index=index)
-        self.send_package(pack=pack)
+        return await self.send_package(pack=pack)
 
-    def send_command(self, body: Union[bytes, bytearray]) -> bool:
+    async def send_command(self, body: Union[bytes, bytearray]) -> bool:
         pack = self._create_command(body=body)
-        return self.send_package(pack=pack, priority=DeparturePriority.SLOWER)
+        return await self.send_package(pack=pack, priority=DeparturePriority.SLOWER)
 
-    def send_message(self, body: Union[bytes, bytearray]) -> bool:
+    async def send_message(self, body: Union[bytes, bytearray]) -> bool:
         pack = self._create_message(body=body)
-        return self.send_package(pack=pack, priority=DeparturePriority.NORMAL)
+        return await self.send_package(pack=pack, priority=DeparturePriority.NORMAL)
 
-    def send_package(self, pack: Package, priority: int = 0) -> bool:
+    async def send_package(self, pack: Package, priority: int = 0) -> bool:
         """ send data package with priority """
         outgo = self._create_departure(pack=pack, priority=priority)
-        return self.send_ship(ship=outgo)
+        return await self.send_ship(ship=outgo)
 
     # Override
-    def send_data(self, payload: Union[bytes, bytearray]) -> bool:
-        return self.send_message(body=payload)
+    async def send_data(self, payload: Union[bytes, bytearray]) -> bool:
+        return await self.send_message(body=payload)
 
     # Override
-    def heartbeat(self):
-        self.send_command(body=PING)
+    async def heartbeat(self):
+        await self.send_command(body=PING)
 
 
 PING = b'PING'
 PONG = b'PONG'
 NOOP = b'NOOP'
 OK = b'OK'
 AGAIN = b'AGAIN'
```

