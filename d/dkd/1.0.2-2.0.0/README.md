# Comparing `tmp/dkd-1.0.2.tar.gz` & `tmp/dkd-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dkd-1.0.2.tar", last modified: Thu Nov  2 05:48:42 2023, max compression
+gzip compressed data, was "dist/dkd-2.0.0.tar", last modified: Fri May 10 15:37:42 2024, max compression
```

## Comparing `dkd-1.0.2.tar` & `dkd-2.0.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-11-02 05:48:42.000000 dkd-1.0.2/
--rw-r--r--   0 moky       (501) staff       (20)     7579 2023-11-02 05:48:42.000000 dkd-1.0.2/PKG-INFO
--rw-r--r--   0 moky       (501) staff       (20)     5783 2021-01-31 04:25:29.000000 dkd-1.0.2/README.md
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-11-02 05:48:42.000000 dkd-1.0.2/dkd/
--rw-r--r--   0 moky       (501) staff       (20)     1955 2023-10-06 14:33:24.000000 dkd-1.0.2/dkd/__init__.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-11-02 05:48:42.000000 dkd-1.0.2/dkd/msg/
--rw-r--r--   0 moky       (501) staff       (20)     1780 2023-10-06 14:28:29.000000 dkd-1.0.2/dkd/msg/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     7807 2023-10-11 03:15:57.000000 dkd-1.0.2/dkd/msg/factory.py
--rw-r--r--   0 moky       (501) staff       (20)     4699 2023-10-09 13:57:32.000000 dkd-1.0.2/dkd/msg/instant.py
--rw-r--r--   0 moky       (501) staff       (20)     2925 2023-10-06 15:13:02.000000 dkd-1.0.2/dkd/msg/reliable.py
--rw-r--r--   0 moky       (501) staff       (20)     6038 2023-10-09 14:01:56.000000 dkd-1.0.2/dkd/msg/secure.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-11-02 05:48:42.000000 dkd-1.0.2/dkd/protocol/
--rw-r--r--   0 moky       (501) staff       (20)     2000 2023-10-06 14:30:49.000000 dkd-1.0.2/dkd/protocol/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     3975 2023-10-28 14:42:41.000000 dkd-1.0.2/dkd/protocol/content.py
--rw-r--r--   0 moky       (501) staff       (20)     4835 2023-10-11 03:16:04.000000 dkd-1.0.2/dkd/protocol/envelope.py
--rw-r--r--   0 moky       (501) staff       (20)     4109 2023-10-11 03:13:47.000000 dkd-1.0.2/dkd/protocol/instant.py
--rw-r--r--   0 moky       (501) staff       (20)     3733 2023-10-09 13:53:08.000000 dkd-1.0.2/dkd/protocol/message.py
--rw-r--r--   0 moky       (501) staff       (20)     3471 2023-10-28 14:28:53.000000 dkd-1.0.2/dkd/protocol/reliable.py
--rw-r--r--   0 moky       (501) staff       (20)     3530 2023-10-06 14:58:28.000000 dkd-1.0.2/dkd/protocol/secure.py
--rw-r--r--   0 moky       (501) staff       (20)     5130 2023-08-18 06:27:03.000000 dkd-1.0.2/dkd/protocol/types.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-11-02 05:48:42.000000 dkd-1.0.2/dkd.egg-info/
--rw-r--r--   0 moky       (501) staff       (20)     7579 2023-11-02 05:48:42.000000 dkd-1.0.2/dkd.egg-info/PKG-INFO
--rw-r--r--   0 moky       (501) staff       (20)      456 2023-11-02 05:48:42.000000 dkd-1.0.2/dkd.egg-info/SOURCES.txt
--rw-r--r--   0 moky       (501) staff       (20)        1 2023-11-02 05:48:42.000000 dkd-1.0.2/dkd.egg-info/dependency_links.txt
--rw-r--r--   0 moky       (501) staff       (20)       11 2023-11-02 05:48:42.000000 dkd-1.0.2/dkd.egg-info/requires.txt
--rw-r--r--   0 moky       (501) staff       (20)        4 2023-11-02 05:48:42.000000 dkd-1.0.2/dkd.egg-info/top_level.txt
--rw-r--r--   0 moky       (501) staff       (20)       38 2023-11-02 05:48:42.000000 dkd-1.0.2/setup.cfg
--rw-r--r--   0 moky       (501) staff       (20)      913 2023-10-28 14:26:05.000000 dkd-1.0.2/setup.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-10 15:37:42.000000 dkd-2.0.0/
+-rw-r--r--   0 moky       (501) staff       (20)     7579 2024-05-10 15:37:42.000000 dkd-2.0.0/PKG-INFO
+-rw-r--r--   0 moky       (501) staff       (20)     5783 2021-01-31 04:25:29.000000 dkd-2.0.0/README.md
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-10 15:37:42.000000 dkd-2.0.0/dkd/
+-rw-r--r--   0 moky       (501) staff       (20)     1955 2023-10-06 14:33:24.000000 dkd-2.0.0/dkd/__init__.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-10 15:37:42.000000 dkd-2.0.0/dkd/msg/
+-rw-r--r--   0 moky       (501) staff       (20)     1780 2023-10-06 14:28:29.000000 dkd-2.0.0/dkd/msg/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     7807 2023-10-11 03:15:57.000000 dkd-2.0.0/dkd/msg/factory.py
+-rw-r--r--   0 moky       (501) staff       (20)     4735 2024-05-06 10:20:32.000000 dkd-2.0.0/dkd/msg/instant.py
+-rw-r--r--   0 moky       (501) staff       (20)     2937 2024-05-06 10:20:47.000000 dkd-2.0.0/dkd/msg/reliable.py
+-rw-r--r--   0 moky       (501) staff       (20)     6086 2024-05-06 10:21:23.000000 dkd-2.0.0/dkd/msg/secure.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-10 15:37:42.000000 dkd-2.0.0/dkd/protocol/
+-rw-r--r--   0 moky       (501) staff       (20)     2000 2023-10-06 14:30:49.000000 dkd-2.0.0/dkd/protocol/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     3975 2023-10-28 14:42:41.000000 dkd-2.0.0/dkd/protocol/content.py
+-rw-r--r--   0 moky       (501) staff       (20)     4835 2023-10-11 03:16:04.000000 dkd-2.0.0/dkd/protocol/envelope.py
+-rw-r--r--   0 moky       (501) staff       (20)     4109 2023-10-11 03:13:47.000000 dkd-2.0.0/dkd/protocol/instant.py
+-rw-r--r--   0 moky       (501) staff       (20)     3733 2023-10-09 13:53:08.000000 dkd-2.0.0/dkd/protocol/message.py
+-rw-r--r--   0 moky       (501) staff       (20)     3471 2023-10-28 14:28:53.000000 dkd-2.0.0/dkd/protocol/reliable.py
+-rw-r--r--   0 moky       (501) staff       (20)     3530 2023-10-06 14:58:28.000000 dkd-2.0.0/dkd/protocol/secure.py
+-rw-r--r--   0 moky       (501) staff       (20)     5130 2023-08-18 06:27:03.000000 dkd-2.0.0/dkd/protocol/types.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-10 15:37:42.000000 dkd-2.0.0/dkd.egg-info/
+-rw-r--r--   0 moky       (501) staff       (20)     7579 2024-05-10 15:37:42.000000 dkd-2.0.0/dkd.egg-info/PKG-INFO
+-rw-r--r--   0 moky       (501) staff       (20)      456 2024-05-10 15:37:42.000000 dkd-2.0.0/dkd.egg-info/SOURCES.txt
+-rw-r--r--   0 moky       (501) staff       (20)        1 2024-05-10 15:37:42.000000 dkd-2.0.0/dkd.egg-info/dependency_links.txt
+-rw-r--r--   0 moky       (501) staff       (20)       11 2024-05-10 15:37:42.000000 dkd-2.0.0/dkd.egg-info/requires.txt
+-rw-r--r--   0 moky       (501) staff       (20)        4 2024-05-10 15:37:42.000000 dkd-2.0.0/dkd.egg-info/top_level.txt
+-rw-r--r--   0 moky       (501) staff       (20)       38 2024-05-10 15:37:42.000000 dkd-2.0.0/setup.cfg
+-rw-r--r--   0 moky       (501) staff       (20)      913 2024-05-10 15:37:23.000000 dkd-2.0.0/setup.py
```

### Comparing `dkd-1.0.2/PKG-INFO` & `dkd-2.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dkd
-Version: 1.0.2
+Version: 2.0.0
 Summary: A common message module
 Home-page: https://github.com/dimchat/dkd-py
 Author: Albert Moky
 Author-email: albert.moky@gmail.com
 License: MIT
 Description: # Dao Ke Dao (道可道) -- Message Module (Python)
```

### Comparing `dkd-1.0.2/README.md` & `dkd-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `dkd-1.0.2/dkd/__init__.py` & `dkd-2.0.0/dkd/__init__.py`

 * *Files identical despite different names*

### Comparing `dkd-1.0.2/dkd/msg/__init__.py` & `dkd-2.0.0/dkd/msg/__init__.py`

 * *Files identical despite different names*

### Comparing `dkd-1.0.2/dkd/msg/factory.py` & `dkd-2.0.0/dkd/msg/factory.py`

 * *Files identical despite different names*

### Comparing `dkd-1.0.2/dkd/msg/instant.py` & `dkd-2.0.0/dkd/msg/instant.py`

 * *Files 8% similar despite different names*

```diff
@@ -55,77 +55,77 @@
     """
 
     #
     #   Encrypt Content
     #
 
     @abstractmethod
-    def serialize_content(self, content: Content, key: SymmetricKey, msg: InstantMessage) -> bytes:
+    async def serialize_content(self, content: Content, key: SymmetricKey, msg: InstantMessage) -> bytes:
         """
         1. Serialize 'message.content' to data (JsON / ProtoBuf / ...)
 
         :param content:  message content
         :param key:      symmetric key (includes data compression algorithm)
         :param msg:      instant message object
         :return: serialized content data
         """
         raise NotImplemented
 
     @abstractmethod
-    def encrypt_content(self, data: bytes, key: SymmetricKey, msg: InstantMessage) -> bytes:
+    async def encrypt_content(self, data: bytes, key: SymmetricKey, msg: InstantMessage) -> bytes:
         """
         2. Encrypt content data to 'message.data' with symmetric key
 
         :param data:     serialized data of message.content
         :param key:      symmetric key
         :param msg:      instant message object
         :return: encrypted message content data
         """
         raise NotImplemented
 
     # @abstractmethod
-    # def encode_data(self, data: bytes, msg: InstantMessage) -> Any:
+    # async def encode_data(self, data: bytes, msg: InstantMessage) -> Any:
     #     """
     #     3. Encode 'message.data' to String (Base64)
     #
     #     :param data:     encrypted content data
     #     :param msg:      instant message object
     #     :return: base64 string
     #     """
     #     raise NotImplemented
 
     #
     #   Encrypt Key
     #
 
     @abstractmethod
-    def serialize_key(self, key: SymmetricKey, msg: InstantMessage) -> Optional[bytes]:
+    async def serialize_key(self, key: SymmetricKey, msg: InstantMessage) -> Optional[bytes]:
         """
         4. Serialize message key to data (JsON / ProtoBuf / ...)
 
         :param key:      symmetric key
         :param msg:      instant message object
         :return: serialized key data, None for reused (or broadcast message)
         """
         raise NotImplemented
 
     @abstractmethod
-    def encrypt_key(self, data: bytes, receiver: ID, msg: InstantMessage) -> Optional[bytes]:
+    async def encrypt_key(self, data: bytes, receiver: ID, msg: InstantMessage) -> Optional[bytes]:
         """
         5. Encrypt key data to 'message.key' with receiver's public key
 
         :param data:     serialized data of symmetric key
         :param receiver: actual receiver (user, or group member)
         :param msg:      instant message object
         :return: encrypted symmetric key data, None on visa not found
         """
         raise NotImplemented
 
     # @abstractmethod
-    # def encode_key(self, data: bytes, msg: InstantMessage) -> Any:
+    # async def encode_key(self, data: bytes, msg: InstantMessage) -> Any:
     #     """
     #     6. Encode 'message.key' to String (Base64)
     #
     #     :param data:     encrypted key data
     #     :param msg:      instant message object
     #     :return: base64 string
     #     """
```

### Comparing `dkd-1.0.2/dkd/msg/reliable.py` & `dkd-2.0.0/dkd/msg/reliable.py`

 * *Files 3% similar despite different names*

```diff
@@ -47,26 +47,26 @@
             | data     |      | data     |  1. verify(data, signature, sender.PK)
             | key/keys |      | key/keys |
             | signature|      +----------+
             +----------+
     """
 
     # @abstractmethod
-    # def decode_signature(self, signature: Any, msg: ReliableMessage) -> Optional[bytes]:
+    # async def decode_signature(self, signature: Any, msg: ReliableMessage) -> Optional[bytes]:
     #     """
     #     1. Decode 'message.signature' from String (Base64)
     #
     #     :param signature: base64 string
     #     :param msg:       reliable message
     #     :return: signature data
     #     """
     #     raise NotImplemented
 
     @abstractmethod
-    def verify_data_signature(self, data: bytes, signature: bytes, msg: ReliableMessage) -> bool:
+    async def verify_data_signature(self, data: bytes, signature: bytes, msg: ReliableMessage) -> bool:
         """
         2. Verify the message data and signature with sender's public key
 
         :param data:      message content(encrypted) data
         :param signature: signature of message content(encrypted) data
         :param msg:       reliable message
         :return: True on signature matched
```

### Comparing `dkd-1.0.2/dkd/msg/secure.py` & `dkd-2.0.0/dkd/msg/secure.py`

 * *Files 9% similar despite different names*

```diff
@@ -55,38 +55,38 @@
     """
 
     #
     #   Decrypt Key
     #
 
     # @abstractmethod
-    # def decode_key(self, key: Any, msg: SecureMessage) -> Optional[bytes]:
+    # async def decode_key(self, key: Any, msg: SecureMessage) -> Optional[bytes]:
     #     """
     #     1. Decode 'message.key' to encrypted symmetric key data
     #
     #     :param key:      base64 string
     #     :param msg:      secure message object
     #     :return: encrypted symmetric key data
     #     """
     #     raise NotImplemented
 
     @abstractmethod
-    def decrypt_key(self, data: bytes, receiver: ID, msg: SecureMessage) -> Optional[bytes]:
+    async def decrypt_key(self, data: bytes, receiver: ID, msg: SecureMessage) -> Optional[bytes]:
         """
         2. Decrypt 'message.key' with receiver's private key
 
         :param data:     encrypted symmetric key data
         :param receiver: actual receiver (user, or group member)
         :param msg:      secure message object
         :return: serialized symmetric key
         """
         raise NotImplemented
 
     @abstractmethod
-    def deserialize_key(self, data: Optional[bytes], msg: SecureMessage) -> Optional[SymmetricKey]:
+    async def deserialize_key(self, data: Optional[bytes], msg: SecureMessage) -> Optional[SymmetricKey]:
         """
         3. Deserialize message key from data (JsON / ProtoBuf / ...)
            (if key data is empty, means it should be reused, get it from key cache)
 
         :param data:     serialized key data, None for reused key
         :param msg:      secure message object
         :return: symmetric key
@@ -94,38 +94,38 @@
         raise NotImplemented
 
     #
     #   Decrypt Content
     #
 
     # @abstractmethod
-    # def decode_data(self, data: Any, msg: SecureMessage) -> Optional[bytes]:
+    # async def decode_data(self, data: Any, msg: SecureMessage) -> Optional[bytes]:
     #     """
     #     4. Decode 'message.data' to encrypted content data
     #
     #     :param data:     base64 string
     #     :param msg:      secure message object
     #     :return: encrypted content data
     #     """
     #     raise NotImplemented
 
     @abstractmethod
-    def decrypt_content(self, data: bytes, key: SymmetricKey, msg: SecureMessage) -> Optional[bytes]:
+    async def decrypt_content(self, data: bytes, key: SymmetricKey, msg: SecureMessage) -> Optional[bytes]:
         """
         5. Decrypt 'message.data' with symmetric key
 
         :param data:     encrypted content data
         :param key:      symmetric key
         :param msg:      secure message object
         :return: serialized message content
         """
         raise NotImplemented
 
     @abstractmethod
-    def deserialize_content(self, data: bytes, key: SymmetricKey, msg: SecureMessage) -> Optional[Content]:
+    async def deserialize_content(self, data: bytes, key: SymmetricKey, msg: SecureMessage) -> Optional[Content]:
         """
         6. Deserialize message content from data (JsON / ProtoBuf / ...)
 
         :param data:     serialized content data
         :param key:      symmetric key (includes data compression algorithm)
         :param msg:      secure message object
         :return: message content
@@ -148,26 +148,26 @@
     """
 
     #
     #   Signature
     #
 
     @abstractmethod
-    def sign_data(self, data: bytes, msg: SecureMessage) -> bytes:
+    async def sign_data(self, data: bytes, msg: SecureMessage) -> bytes:
         """
         1. Sign 'message.data' with sender's private key
 
         :param data:      encrypted message data
         :param msg:       secure message object
         :return: signature of encrypted message data
         """
         raise NotImplemented
 
     # @abstractmethod
-    # def encode_signature(self, signature: bytes, msg: SecureMessage) -> Any:
+    # async def encode_signature(self, signature: bytes, msg: SecureMessage) -> Any:
     #     """
     #     2. Encode 'message.signature' to String (Base64)
     #
     #     :param signature: signature of message.data
     #     :param msg:       secure message object
     #     :return: base64 string
     #     """
```

### Comparing `dkd-1.0.2/dkd/protocol/__init__.py` & `dkd-2.0.0/dkd/protocol/__init__.py`

 * *Files identical despite different names*

### Comparing `dkd-1.0.2/dkd/protocol/content.py` & `dkd-2.0.0/dkd/protocol/content.py`

 * *Files identical despite different names*

### Comparing `dkd-1.0.2/dkd/protocol/envelope.py` & `dkd-2.0.0/dkd/protocol/envelope.py`

 * *Files identical despite different names*

### Comparing `dkd-1.0.2/dkd/protocol/instant.py` & `dkd-2.0.0/dkd/protocol/instant.py`

 * *Files identical despite different names*

### Comparing `dkd-1.0.2/dkd/protocol/message.py` & `dkd-2.0.0/dkd/protocol/message.py`

 * *Files identical despite different names*

### Comparing `dkd-1.0.2/dkd/protocol/reliable.py` & `dkd-2.0.0/dkd/protocol/reliable.py`

 * *Files identical despite different names*

### Comparing `dkd-1.0.2/dkd/protocol/secure.py` & `dkd-2.0.0/dkd/protocol/secure.py`

 * *Files identical despite different names*

### Comparing `dkd-1.0.2/dkd/protocol/types.py` & `dkd-2.0.0/dkd/protocol/types.py`

 * *Files identical despite different names*

### Comparing `dkd-1.0.2/dkd.egg-info/PKG-INFO` & `dkd-2.0.0/dkd.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dkd
-Version: 1.0.2
+Version: 2.0.0
 Summary: A common message module
 Home-page: https://github.com/dimchat/dkd-py
 Author: Albert Moky
 Author-email: albert.moky@gmail.com
 License: MIT
 Description: # Dao Ke Dao (道可道) -- Message Module (Python)
```

### Comparing `dkd-1.0.2/setup.py` & `dkd-2.0.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     Common Message Module for decentralized instant messaging
 """
 
 import io
 
 from setuptools import setup, find_packages
 
-__version__ = '1.0.2'
+__version__ = '2.0.0'
 __author__ = 'Albert Moky'
 __contact__ = 'albert.moky@gmail.com'
 
 with io.open('README.md', 'r', encoding='utf-8') as fh:
     readme = fh.read()
 
 setup(
@@ -32,10 +32,10 @@
     packages=find_packages(),
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
     ],
     install_requires=[
-        'mkm>=1.0.2',
+        'mkm>=2.0.0',
     ]
 )
```

