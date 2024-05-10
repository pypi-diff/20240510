# Comparing `tmp/pytoniq-0.1.8.tar.gz` & `tmp/pytoniq-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytoniq-0.1.8.tar", last modified: Sat Oct 14 07:28:08 2023, max compression
+gzip compressed data, was "pytoniq-0.1.9.tar", last modified: Tue Oct 17 15:42:03 2023, max compression
```

## Comparing `pytoniq-0.1.8.tar` & `pytoniq-0.1.9.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 yungwine   (501) staff       (20)        0 2023-10-14 07:28:08.872290 pytoniq-0.1.8/
--rw-r--r--   0 yungwine   (501) staff       (20)       53 2023-09-27 16:16:05.000000 pytoniq-0.1.8/MANIFEST.in
--rw-r--r--   0 yungwine   (501) staff       (20)     5916 2023-10-14 07:28:08.872166 pytoniq-0.1.8/PKG-INFO
--rw-r--r--   0 yungwine   (501) staff       (20)     5510 2023-09-27 15:58:46.000000 pytoniq-0.1.8/README.md
-drwxr-xr-x   0 yungwine   (501) staff       (20)        0 2023-10-14 07:28:08.869396 pytoniq-0.1.8/pytoniq/
--rw-r--r--   0 yungwine   (501) staff       (20)      229 2023-09-27 16:18:26.000000 pytoniq-0.1.8/pytoniq/__init__.py
-drwxr-xr-x   0 yungwine   (501) staff       (20)        0 2023-10-14 07:28:08.870360 pytoniq-0.1.8/pytoniq/adnl/
--rw-r--r--   0 yungwine   (501) staff       (20)      140 2023-09-27 16:18:26.000000 pytoniq-0.1.8/pytoniq/adnl/__init__.py
--rw-r--r--   0 yungwine   (501) staff       (20)    17154 2023-10-14 07:27:26.000000 pytoniq-0.1.8/pytoniq/adnl/adnl.py
--rw-r--r--   0 yungwine   (501) staff       (20)     9165 2023-09-28 06:37:27.000000 pytoniq-0.1.8/pytoniq/adnl/dht.py
-drwxr-xr-x   0 yungwine   (501) staff       (20)        0 2023-10-14 07:28:08.870849 pytoniq-0.1.8/pytoniq/contract/
--rw-r--r--   0 yungwine   (501) staff       (20)       88 2023-08-04 06:37:21.000000 pytoniq-0.1.8/pytoniq/contract/__init__.py
--rw-r--r--   0 yungwine   (501) staff       (20)     6805 2023-08-04 06:37:21.000000 pytoniq-0.1.8/pytoniq/contract/contract.py
-drwxr-xr-x   0 yungwine   (501) staff       (20)        0 2023-10-14 07:28:08.871162 pytoniq-0.1.8/pytoniq/contract/nft/
--rw-r--r--   0 yungwine   (501) staff       (20)       25 2023-07-27 17:13:15.000000 pytoniq-0.1.8/pytoniq/contract/nft/__init__.py
--rw-r--r--   0 yungwine   (501) staff       (20)     3415 2023-08-04 06:37:21.000000 pytoniq-0.1.8/pytoniq/contract/nft/nft.py
--rw-r--r--   0 yungwine   (501) staff       (20)     5929 2023-08-04 06:37:20.000000 pytoniq-0.1.8/pytoniq/contract/nft/nft_sale.py
--rw-r--r--   0 yungwine   (501) staff       (20)      102 2023-07-22 17:41:04.000000 pytoniq-0.1.8/pytoniq/contract/utils.py
-drwxr-xr-x   0 yungwine   (501) staff       (20)        0 2023-10-14 07:28:08.871500 pytoniq-0.1.8/pytoniq/contract/wallets/
--rw-r--r--   0 yungwine   (501) staff       (20)      151 2023-07-23 15:42:41.000000 pytoniq-0.1.8/pytoniq/contract/wallets/__init__.py
--rw-r--r--   0 yungwine   (501) staff       (20)     7675 2023-08-04 06:37:21.000000 pytoniq-0.1.8/pytoniq/contract/wallets/highload.py
--rw-r--r--   0 yungwine   (501) staff       (20)    18839 2023-08-04 06:37:21.000000 pytoniq-0.1.8/pytoniq/contract/wallets/wallet.py
-drwxr-xr-x   0 yungwine   (501) staff       (20)        0 2023-10-14 07:28:08.871977 pytoniq-0.1.8/pytoniq/liteclient/
--rw-r--r--   0 yungwine   (501) staff       (20)       88 2023-07-23 15:42:41.000000 pytoniq-0.1.8/pytoniq/liteclient/__init__.py
--rw-r--r--   0 yungwine   (501) staff       (20)    41966 2023-10-14 07:25:52.000000 pytoniq-0.1.8/pytoniq/liteclient/client.py
--rw-r--r--   0 yungwine   (501) staff       (20)     5420 2023-08-04 06:37:21.000000 pytoniq-0.1.8/pytoniq/liteclient/sync.py
--rw-r--r--   0 yungwine   (501) staff       (20)      636 2023-08-04 06:37:21.000000 pytoniq-0.1.8/pytoniq/liteclient/utils.py
-drwxr-xr-x   0 yungwine   (501) staff       (20)        0 2023-10-14 07:28:08.869971 pytoniq-0.1.8/pytoniq.egg-info/
--rw-r--r--   0 yungwine   (501) staff       (20)     5916 2023-10-14 07:28:08.000000 pytoniq-0.1.8/pytoniq.egg-info/PKG-INFO
--rw-r--r--   0 yungwine   (501) staff       (20)      672 2023-10-14 07:28:08.000000 pytoniq-0.1.8/pytoniq.egg-info/SOURCES.txt
--rw-r--r--   0 yungwine   (501) staff       (20)        1 2023-10-14 07:28:08.000000 pytoniq-0.1.8/pytoniq.egg-info/dependency_links.txt
--rw-r--r--   0 yungwine   (501) staff       (20)       56 2023-10-14 07:28:08.000000 pytoniq-0.1.8/pytoniq.egg-info/requires.txt
--rw-r--r--   0 yungwine   (501) staff       (20)        8 2023-10-14 07:28:08.000000 pytoniq-0.1.8/pytoniq.egg-info/top_level.txt
--rw-r--r--   0 yungwine   (501) staff       (20)       38 2023-10-14 07:28:08.872335 pytoniq-0.1.8/setup.cfg
--rw-r--r--   0 yungwine   (501) staff       (20)      855 2023-10-14 07:27:37.000000 pytoniq-0.1.8/setup.py
+drwxr-xr-x   0 yungwine   (501) staff       (20)        0 2023-10-17 15:42:03.879776 pytoniq-0.1.9/
+-rw-r--r--   0 yungwine   (501) staff       (20)       53 2023-09-27 16:16:05.000000 pytoniq-0.1.9/MANIFEST.in
+-rw-r--r--   0 yungwine   (501) staff       (20)     5965 2023-10-17 15:42:03.879686 pytoniq-0.1.9/PKG-INFO
+-rw-r--r--   0 yungwine   (501) staff       (20)     5510 2023-09-27 15:58:46.000000 pytoniq-0.1.9/README.md
+drwxr-xr-x   0 yungwine   (501) staff       (20)        0 2023-10-17 15:42:03.877036 pytoniq-0.1.9/pytoniq/
+-rw-r--r--   0 yungwine   (501) staff       (20)      229 2023-09-27 16:18:26.000000 pytoniq-0.1.9/pytoniq/__init__.py
+drwxr-xr-x   0 yungwine   (501) staff       (20)        0 2023-10-17 15:42:03.877878 pytoniq-0.1.9/pytoniq/adnl/
+-rw-r--r--   0 yungwine   (501) staff       (20)      140 2023-09-27 16:18:26.000000 pytoniq-0.1.9/pytoniq/adnl/__init__.py
+-rw-r--r--   0 yungwine   (501) staff       (20)    17542 2023-10-17 15:33:51.000000 pytoniq-0.1.9/pytoniq/adnl/adnl.py
+-rw-r--r--   0 yungwine   (501) staff       (20)     9165 2023-09-28 06:37:27.000000 pytoniq-0.1.9/pytoniq/adnl/dht.py
+drwxr-xr-x   0 yungwine   (501) staff       (20)        0 2023-10-17 15:42:03.878214 pytoniq-0.1.9/pytoniq/contract/
+-rw-r--r--   0 yungwine   (501) staff       (20)       88 2023-08-04 06:37:21.000000 pytoniq-0.1.9/pytoniq/contract/__init__.py
+-rw-r--r--   0 yungwine   (501) staff       (20)     6805 2023-08-04 06:37:21.000000 pytoniq-0.1.9/pytoniq/contract/contract.py
+drwxr-xr-x   0 yungwine   (501) staff       (20)        0 2023-10-17 15:42:03.878503 pytoniq-0.1.9/pytoniq/contract/nft/
+-rw-r--r--   0 yungwine   (501) staff       (20)       25 2023-07-27 17:13:15.000000 pytoniq-0.1.9/pytoniq/contract/nft/__init__.py
+-rw-r--r--   0 yungwine   (501) staff       (20)     3415 2023-08-04 06:37:21.000000 pytoniq-0.1.9/pytoniq/contract/nft/nft.py
+-rw-r--r--   0 yungwine   (501) staff       (20)     5929 2023-08-04 06:37:20.000000 pytoniq-0.1.9/pytoniq/contract/nft/nft_sale.py
+-rw-r--r--   0 yungwine   (501) staff       (20)      102 2023-07-22 17:41:04.000000 pytoniq-0.1.9/pytoniq/contract/utils.py
+drwxr-xr-x   0 yungwine   (501) staff       (20)        0 2023-10-17 15:42:03.878832 pytoniq-0.1.9/pytoniq/contract/wallets/
+-rw-r--r--   0 yungwine   (501) staff       (20)      151 2023-07-23 15:42:41.000000 pytoniq-0.1.9/pytoniq/contract/wallets/__init__.py
+-rw-r--r--   0 yungwine   (501) staff       (20)     7675 2023-08-04 06:37:21.000000 pytoniq-0.1.9/pytoniq/contract/wallets/highload.py
+-rw-r--r--   0 yungwine   (501) staff       (20)    18839 2023-08-04 06:37:21.000000 pytoniq-0.1.9/pytoniq/contract/wallets/wallet.py
+drwxr-xr-x   0 yungwine   (501) staff       (20)        0 2023-10-17 15:42:03.879529 pytoniq-0.1.9/pytoniq/liteclient/
+-rw-r--r--   0 yungwine   (501) staff       (20)       88 2023-07-23 15:42:41.000000 pytoniq-0.1.9/pytoniq/liteclient/__init__.py
+-rw-r--r--   0 yungwine   (501) staff       (20)    41943 2023-10-17 15:37:42.000000 pytoniq-0.1.9/pytoniq/liteclient/client.py
+-rw-r--r--   0 yungwine   (501) staff       (20)     5420 2023-08-04 06:37:21.000000 pytoniq-0.1.9/pytoniq/liteclient/sync.py
+-rw-r--r--   0 yungwine   (501) staff       (20)      636 2023-08-04 06:37:21.000000 pytoniq-0.1.9/pytoniq/liteclient/utils.py
+drwxr-xr-x   0 yungwine   (501) staff       (20)        0 2023-10-17 15:42:03.877545 pytoniq-0.1.9/pytoniq.egg-info/
+-rw-r--r--   0 yungwine   (501) staff       (20)     5965 2023-10-17 15:42:03.000000 pytoniq-0.1.9/pytoniq.egg-info/PKG-INFO
+-rw-r--r--   0 yungwine   (501) staff       (20)      672 2023-10-17 15:42:03.000000 pytoniq-0.1.9/pytoniq.egg-info/SOURCES.txt
+-rw-r--r--   0 yungwine   (501) staff       (20)        1 2023-10-17 15:42:03.000000 pytoniq-0.1.9/pytoniq.egg-info/dependency_links.txt
+-rw-r--r--   0 yungwine   (501) staff       (20)       57 2023-10-17 15:42:03.000000 pytoniq-0.1.9/pytoniq.egg-info/requires.txt
+-rw-r--r--   0 yungwine   (501) staff       (20)        8 2023-10-17 15:42:03.000000 pytoniq-0.1.9/pytoniq.egg-info/top_level.txt
+-rw-r--r--   0 yungwine   (501) staff       (20)       38 2023-10-17 15:42:03.879817 pytoniq-0.1.9/setup.cfg
+-rw-r--r--   0 yungwine   (501) staff       (20)      904 2023-10-17 15:41:45.000000 pytoniq-0.1.9/setup.py
```

### Comparing `pytoniq-0.1.8/PKG-INFO` & `pytoniq-0.1.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: pytoniq
-Version: 0.1.8
+Version: 0.1.9
 Summary: TON Blockchain SDK
 Home-page: https://github.com/yungwine/pytoniq
 Author: Maksim Kurbatov
 Author-email: cyrbatoff@gmail.com
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries
-Requires-Python: >=3.10
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 
 # pytoniq
 
 [![PyPI version](https://badge.fury.io/py/pytoniq.svg)](https://badge.fury.io/py/pytoniq) 
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pytoniq)](https://pypi.org/project/pytoniq/)
 ![](https://pepy.tech/badge/pytoniq)
```

### Comparing `pytoniq-0.1.8/README.md` & `pytoniq-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `pytoniq-0.1.8/pytoniq/adnl/adnl.py` & `pytoniq-0.1.9/pytoniq/adnl/adnl.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import asyncio
 import base64
 import logging
 import time
 import hashlib
+import types
 import typing
 from asyncio import transports
 from typing import Any
 
 from pytoniq_core.tl.generator import TlGenerator
 
 from pytoniq_core.crypto.ciphers import Server, Client, AdnlChannel, get_random, aes_ctr_encrypt, aes_ctr_decrypt, get_shared_key, create_aes_ctr_sipher_from_key_n_data
@@ -20,15 +21,15 @@
         self._packets = asyncio.Queue(1000)
         self.timeout = timeout
         self.logger = logging.getLogger(self.__class__.__name__)
 
     def connection_made(self, transport: transports.DatagramTransport) -> None:
         super().connection_made(transport)
 
-    def datagram_received(self, data: bytes, addr: tuple[str | Any, int]) -> None:
+    def datagram_received(self, data: bytes, addr: typing.Tuple[typing.Union[str, Any], int]) -> None:
         self.logger.debug(f'received {len(data)} bytes')
         self._packets.put_nowait((data, addr))
         super().datagram_received(data, addr)
 
     def error_received(self, exc: Exception) -> None:
         raise exc
         super().error_received(exc)
@@ -113,14 +114,15 @@
         """
 
         """########### init ###########"""
         self.loop: asyncio.AbstractEventLoop = None
         self.timeout = kwargs.get('timeout', 10)
         self.listener = None
         self.tasks: typing.Dict[str, asyncio.Future] = {}
+        self.query_handlers: typing.Dict[str, typing.Callable] = {}
 
         """########### connection ###########"""
         self.transport: asyncio.DatagramTransport = None
         self.protocol: SocketProtocol = None
         self.local_address = local_address
 
         """########### TL ###########"""
@@ -254,21 +256,26 @@
                     futures.append(future)
         return futures
 
     @staticmethod
     async def _receive(futures: typing.List[asyncio.Future]) -> list:
         return list(await asyncio.gather(*futures))
 
-    def process_incoming_message(self, message: dict):
+    async def process_incoming_message(self, message: dict):
         if message['@type'] == 'adnl.message.answer':
             future = self.tasks.pop(message.get('query_id'))
             future.set_result(message['answer'])
         elif message['@type'] == 'adnl.message.confirmChannel':
             future = self.tasks.pop(message.get('peer_key'))
             future.set_result(message)
+        elif message['@type'] == 'adnl.message.query':
+            query = message.get('query')
+            handler = self.query_handlers.get(query['@type'])
+            if handler:
+                handler(query)
         else:
             raise AdnlTransportError(f'unexpected message type received as a client: {message}')
 
     async def listen(self):
         while True:
             if not self.tasks:
                 await asyncio.sleep(0)
@@ -283,18 +290,18 @@
                 if received_confirm_seqno > peer.confirm_seqno:
                     peer.confirm_seqno = received_confirm_seqno
 
             message = response.get('message')
             messages = response.get('messages')
 
             if message:
-                self.process_incoming_message(message)
+                await self.process_incoming_message(message)
             if messages:
                 for message in messages:
-                    self.process_incoming_message(message)
+                    await self.process_incoming_message(message)
 
     async def send_message_in_channel(self, data: dict, channel: typing.Optional[AdnlChannel] = None, peer: Node = None) -> list:
 
         if peer is None:
             raise AdnlTransportError('Must provide peer')
 
         data = self._prepare_packet_content_msg(data, peer)
@@ -439,14 +446,16 @@
         data = {
             'message': message,
         }
 
         result = await self.send_message_in_channel(data, None, peer)
         return result
 
+    async def send_answer_message(self, ):
+        pass
     async def send_custom_message(self, message: bytes, peer) -> list:
         # TODO test
 
         custom_message = {
             '@type': 'adnl.message.custom',
             'data': message
         }
```

### Comparing `pytoniq-0.1.8/pytoniq/adnl/dht.py` & `pytoniq-0.1.9/pytoniq/adnl/dht.py`

 * *Files identical despite different names*

### Comparing `pytoniq-0.1.8/pytoniq/contract/contract.py` & `pytoniq-0.1.9/pytoniq/contract/contract.py`

 * *Files identical despite different names*

### Comparing `pytoniq-0.1.8/pytoniq/contract/nft/nft.py` & `pytoniq-0.1.9/pytoniq/contract/nft/nft.py`

 * *Files identical despite different names*

### Comparing `pytoniq-0.1.8/pytoniq/contract/nft/nft_sale.py` & `pytoniq-0.1.9/pytoniq/contract/nft/nft_sale.py`

 * *Files identical despite different names*

### Comparing `pytoniq-0.1.8/pytoniq/contract/wallets/highload.py` & `pytoniq-0.1.9/pytoniq/contract/wallets/highload.py`

 * *Files identical despite different names*

### Comparing `pytoniq-0.1.8/pytoniq/contract/wallets/wallet.py` & `pytoniq-0.1.9/pytoniq/contract/wallets/wallet.py`

 * *Files identical despite different names*

### Comparing `pytoniq-0.1.8/pytoniq/liteclient/client.py` & `pytoniq-0.1.9/pytoniq/liteclient/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,32 +1,30 @@
 import base64
 import hashlib
 import logging
-import os
 import asyncio
 import random
 import socket
 import struct
-import time
 import typing
 
 import requests
 
-from .sync import persistent_state_ttl, choose_key_block, sync
+from .sync import choose_key_block, sync
 from .utils import init_mainnet_block, init_testnet_block
-from pytoniq_core.boc import Slice, Cell, Builder
+from pytoniq_core.boc import Slice, Cell
 from pytoniq_core.proof.check_proof import check_block_header_proof, check_shard_proof, check_account_proof, check_proof, \
     check_block_signatures, compute_validator_set
 from pytoniq_core.boc.address import Address
 
 from pytoniq_core.crypto.ciphers import Server, Client, get_random, create_aes_ctr_cipher, aes_ctr_encrypt, aes_ctr_decrypt, get_shared_key
 from pytoniq_core.crypto.crc import crc16
 
 from pytoniq_core.tl.generator import TlGenerator, TlSchema
-from pytoniq_core.tl.block import BlockId, BlockIdExt
+from pytoniq_core.tl.block import BlockIdExt, BlockId  # do not remove this import!
 from pytoniq_core.tlb.config import ConfigParam34, ConfigParam28, ConfigParam
 from pytoniq_core.tlb.transaction import Transaction
 from pytoniq_core.tlb.utils import deserialize_shard_hashes
 
 from pytoniq_core.tlb.vm_stack import VmStack
 from pytoniq_core.tlb.block import Block, ShardDescr, BinTree, ShardStateUnsplit, KeyExtBlkRef
 from pytoniq_core.tlb.account import Account, SimpleAccount, ShardAccount, AccountBlock
```

### Comparing `pytoniq-0.1.8/pytoniq/liteclient/sync.py` & `pytoniq-0.1.9/pytoniq/liteclient/sync.py`

 * *Files identical despite different names*

### Comparing `pytoniq-0.1.8/pytoniq/liteclient/utils.py` & `pytoniq-0.1.9/pytoniq/liteclient/utils.py`

 * *Files identical despite different names*

### Comparing `pytoniq-0.1.8/pytoniq.egg-info/PKG-INFO` & `pytoniq-0.1.9/pytoniq.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: pytoniq
-Version: 0.1.8
+Version: 0.1.9
 Summary: TON Blockchain SDK
 Home-page: https://github.com/yungwine/pytoniq
 Author: Maksim Kurbatov
 Author-email: cyrbatoff@gmail.com
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries
-Requires-Python: >=3.10
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 
 # pytoniq
 
 [![PyPI version](https://badge.fury.io/py/pytoniq.svg)](https://badge.fury.io/py/pytoniq) 
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pytoniq)](https://pypi.org/project/pytoniq/)
 ![](https://pepy.tech/badge/pytoniq)
```

### Comparing `pytoniq-0.1.8/pytoniq.egg-info/SOURCES.txt` & `pytoniq-0.1.9/pytoniq.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pytoniq-0.1.8/setup.py` & `pytoniq-0.1.9/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pytoniq",
-    version="0.1.8",
+    version="0.1.9",
     author="Maksim Kurbatov",
     author_email="cyrbatoff@gmail.com",
     description="TON Blockchain SDK",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages('.', exclude=['tests', 'examples']),
     include_package_data=True,
     classifiers=[
+        "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Topic :: Software Development :: Libraries",
     ],
     url="https://github.com/yungwine/pytoniq",
-    python_requires='>=3.10',
+    python_requires='>=3.9',
     py_modules=["pytoniq"],
     install_requires=[
-        "pytoniq-core>=0.1.8",
+        "pytoniq-core>=0.1.10",
         "requests>=2.31.0",
         "setuptools>=65.5.1",
     ]
 )
```

