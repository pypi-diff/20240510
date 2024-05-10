# Comparing `tmp/dimp-1.0.3.tar.gz` & `tmp/dimp-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dimp-1.0.3.tar", last modified: Tue Dec  5 09:56:09 2023, max compression
+gzip compressed data, was "dist/dimp-2.0.0.tar", last modified: Fri May 10 15:40:05 2024, max compression
```

## Comparing `dimp-1.0.3.tar` & `dimp-2.0.0.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-12-05 09:56:09.000000 dimp-1.0.3/
--rw-r--r--   0 moky       (501) staff       (20)     1057 2023-12-05 09:56:09.000000 dimp-1.0.3/PKG-INFO
--rw-r--r--   0 moky       (501) staff       (20)      562 2021-01-31 04:25:38.000000 dimp-1.0.3/README.md
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-12-05 09:56:08.000000 dimp-1.0.3/dimp/
--rw-r--r--   0 moky       (501) staff       (20)     4694 2023-10-29 06:48:41.000000 dimp-1.0.3/dimp/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     8053 2023-10-29 06:39:01.000000 dimp-1.0.3/dimp/barrack.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-12-05 09:56:08.000000 dimp-1.0.3/dimp/crypto/
--rw-r--r--   0 moky       (501) staff       (20)     2331 2023-10-13 03:43:03.000000 dimp-1.0.3/dimp/crypto/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     5651 2023-10-28 15:12:28.000000 dimp-1.0.3/dimp/crypto/keys.py
--rw-r--r--   0 moky       (501) staff       (20)     4712 2023-10-28 15:17:23.000000 dimp-1.0.3/dimp/crypto/pnf.py
--rw-r--r--   0 moky       (501) staff       (20)     5046 2023-10-28 15:21:45.000000 dimp-1.0.3/dimp/crypto/ted.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-12-05 09:56:08.000000 dimp-1.0.3/dimp/dkd/
--rw-r--r--   0 moky       (501) staff       (20)     3986 2023-10-29 06:22:37.000000 dimp-1.0.3/dimp/dkd/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     4725 2023-10-13 07:24:40.000000 dimp-1.0.3/dimp/dkd/base.py
--rw-r--r--   0 moky       (501) staff       (20)     5783 2023-12-04 11:29:47.000000 dimp-1.0.3/dimp/dkd/commands.py
--rw-r--r--   0 moky       (501) staff       (20)    11728 2023-12-04 11:22:16.000000 dimp-1.0.3/dimp/dkd/contents.py
--rw-r--r--   0 moky       (501) staff       (20)     3312 2023-10-13 08:03:25.000000 dimp-1.0.3/dimp/dkd/customized.py
--rw-r--r--   0 moky       (501) staff       (20)     3501 2023-10-29 06:10:49.000000 dimp-1.0.3/dimp/dkd/factory.py
--rw-r--r--   0 moky       (501) staff       (20)     8437 2023-10-13 08:07:52.000000 dimp-1.0.3/dimp/dkd/files.py
--rw-r--r--   0 moky       (501) staff       (20)     3849 2023-10-29 06:26:44.000000 dimp-1.0.3/dimp/dkd/group_admins.py
--rw-r--r--   0 moky       (501) staff       (20)     7683 2023-12-04 10:58:47.000000 dimp-1.0.3/dimp/dkd/groups.py
--rw-r--r--   0 moky       (501) staff       (20)     4391 2023-10-13 08:19:45.000000 dimp-1.0.3/dimp/dkd/money.py
--rw-r--r--   0 moky       (501) staff       (20)     4737 2023-10-29 06:21:49.000000 dimp-1.0.3/dimp/dkd/receipt.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-12-05 09:56:08.000000 dimp-1.0.3/dimp/mkm/
--rw-r--r--   0 moky       (501) staff       (20)     2591 2023-10-29 06:06:22.000000 dimp-1.0.3/dimp/mkm/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     2045 2023-10-06 16:19:19.000000 dimp-1.0.3/dimp/mkm/delegate.py
--rw-r--r--   0 moky       (501) staff       (20)     5965 2023-10-28 15:36:22.000000 dimp-1.0.3/dimp/mkm/docs.py
--rw-r--r--   0 moky       (501) staff       (20)    10276 2023-10-13 07:54:26.000000 dimp-1.0.3/dimp/mkm/document.py
--rw-r--r--   0 moky       (501) staff       (20)     5629 2023-10-28 15:41:09.000000 dimp-1.0.3/dimp/mkm/entity.py
--rw-r--r--   0 moky       (501) staff       (20)     5804 2023-10-29 05:52:08.000000 dimp-1.0.3/dimp/mkm/group.py
--rw-r--r--   0 moky       (501) staff       (20)     6446 2023-10-29 05:49:42.000000 dimp-1.0.3/dimp/mkm/helper.py
--rw-r--r--   0 moky       (501) staff       (20)     8637 2023-10-13 16:17:40.000000 dimp-1.0.3/dimp/mkm/meta.py
--rw-r--r--   0 moky       (501) staff       (20)    11017 2023-10-29 05:54:03.000000 dimp-1.0.3/dimp/mkm/user.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-12-05 09:56:08.000000 dimp-1.0.3/dimp/msg/
--rw-r--r--   0 moky       (501) staff       (20)     1737 2023-10-12 08:33:49.000000 dimp-1.0.3/dimp/msg/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     4099 2023-10-28 14:58:31.000000 dimp-1.0.3/dimp/msg/base.py
--rw-r--r--   0 moky       (501) staff       (20)     4212 2023-10-28 15:04:37.000000 dimp-1.0.3/dimp/msg/envelope.py
--rw-r--r--   0 moky       (501) staff       (20)     3446 2023-10-28 15:06:22.000000 dimp-1.0.3/dimp/msg/instant.py
--rw-r--r--   0 moky       (501) staff       (20)     3003 2023-10-28 15:09:07.000000 dimp-1.0.3/dimp/msg/reliable.py
--rw-r--r--   0 moky       (501) staff       (20)     4012 2023-10-10 10:02:29.000000 dimp-1.0.3/dimp/msg/secure.py
--rw-r--r--   0 moky       (501) staff       (20)     3290 2023-10-10 08:32:29.000000 dimp-1.0.3/dimp/packer.py
--rw-r--r--   0 moky       (501) staff       (20)     3106 2022-12-11 05:04:56.000000 dimp-1.0.3/dimp/processor.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-12-05 09:56:09.000000 dimp-1.0.3/dimp/protocol/
--rw-r--r--   0 moky       (501) staff       (20)     4228 2023-10-29 06:45:03.000000 dimp-1.0.3/dimp/protocol/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     6144 2023-12-04 11:30:11.000000 dimp-1.0.3/dimp/protocol/commands.py
--rw-r--r--   0 moky       (501) staff       (20)     8435 2023-12-04 11:23:28.000000 dimp-1.0.3/dimp/protocol/contents.py
--rw-r--r--   0 moky       (501) staff       (20)     2552 2023-10-10 04:21:03.000000 dimp-1.0.3/dimp/protocol/customized.py
--rw-r--r--   0 moky       (501) staff       (20)     3386 2023-10-28 14:10:54.000000 dimp-1.0.3/dimp/protocol/docs.py
--rw-r--r--   0 moky       (501) staff       (20)     8654 2023-10-28 14:54:13.000000 dimp-1.0.3/dimp/protocol/files.py
--rw-r--r--   0 moky       (501) staff       (20)     7267 2023-12-04 10:59:34.000000 dimp-1.0.3/dimp/protocol/groups.py
--rw-r--r--   0 moky       (501) staff       (20)     3574 2023-10-29 06:01:28.000000 dimp-1.0.3/dimp/protocol/money.py
--rw-r--r--   0 moky       (501) staff       (20)     5613 2023-10-10 05:41:02.000000 dimp-1.0.3/dimp/protocol/receipt.py
--rw-r--r--   0 moky       (501) staff       (20)     8980 2023-10-10 08:55:56.000000 dimp-1.0.3/dimp/transceiver.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2023-12-05 09:56:08.000000 dimp-1.0.3/dimp.egg-info/
--rw-r--r--   0 moky       (501) staff       (20)     1057 2023-12-05 09:56:08.000000 dimp-1.0.3/dimp.egg-info/PKG-INFO
--rw-r--r--   0 moky       (501) staff       (20)     1060 2023-12-05 09:56:08.000000 dimp-1.0.3/dimp.egg-info/SOURCES.txt
--rw-r--r--   0 moky       (501) staff       (20)        1 2023-12-05 09:56:08.000000 dimp-1.0.3/dimp.egg-info/dependency_links.txt
--rw-r--r--   0 moky       (501) staff       (20)       22 2023-12-05 09:56:08.000000 dimp-1.0.3/dimp.egg-info/requires.txt
--rw-r--r--   0 moky       (501) staff       (20)        5 2023-12-05 09:56:08.000000 dimp-1.0.3/dimp.egg-info/top_level.txt
--rw-r--r--   0 moky       (501) staff       (20)       38 2023-12-05 09:56:09.000000 dimp-1.0.3/setup.cfg
--rw-r--r--   0 moky       (501) staff       (20)     1151 2023-12-04 11:36:53.000000 dimp-1.0.3/setup.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-10 15:40:05.000000 dimp-2.0.0/
+-rw-r--r--   0 moky       (501) staff       (20)     1057 2024-05-10 15:40:05.000000 dimp-2.0.0/PKG-INFO
+-rw-r--r--   0 moky       (501) staff       (20)      562 2021-01-31 04:25:38.000000 dimp-2.0.0/README.md
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-10 15:40:05.000000 dimp-2.0.0/dimp/
+-rw-r--r--   0 moky       (501) staff       (20)     4694 2023-10-29 06:48:41.000000 dimp-2.0.0/dimp/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     8299 2024-05-06 15:17:24.000000 dimp-2.0.0/dimp/barrack.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-10 15:40:05.000000 dimp-2.0.0/dimp/crypto/
+-rw-r--r--   0 moky       (501) staff       (20)     2331 2023-10-13 03:43:03.000000 dimp-2.0.0/dimp/crypto/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     5651 2023-10-28 15:12:28.000000 dimp-2.0.0/dimp/crypto/keys.py
+-rw-r--r--   0 moky       (501) staff       (20)     4712 2023-10-28 15:17:23.000000 dimp-2.0.0/dimp/crypto/pnf.py
+-rw-r--r--   0 moky       (501) staff       (20)     5046 2023-10-28 15:21:45.000000 dimp-2.0.0/dimp/crypto/ted.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-10 15:40:05.000000 dimp-2.0.0/dimp/dkd/
+-rw-r--r--   0 moky       (501) staff       (20)     3986 2023-10-29 06:22:37.000000 dimp-2.0.0/dimp/dkd/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     4725 2023-10-13 07:24:40.000000 dimp-2.0.0/dimp/dkd/base.py
+-rw-r--r--   0 moky       (501) staff       (20)     5783 2023-12-04 11:29:47.000000 dimp-2.0.0/dimp/dkd/commands.py
+-rw-r--r--   0 moky       (501) staff       (20)    11002 2024-05-06 14:54:04.000000 dimp-2.0.0/dimp/dkd/contents.py
+-rw-r--r--   0 moky       (501) staff       (20)     3312 2023-10-13 08:03:25.000000 dimp-2.0.0/dimp/dkd/customized.py
+-rw-r--r--   0 moky       (501) staff       (20)     3501 2023-10-29 06:10:49.000000 dimp-2.0.0/dimp/dkd/factory.py
+-rw-r--r--   0 moky       (501) staff       (20)     6330 2024-05-06 14:54:14.000000 dimp-2.0.0/dimp/dkd/files.py
+-rw-r--r--   0 moky       (501) staff       (20)     3849 2023-10-29 06:26:44.000000 dimp-2.0.0/dimp/dkd/group_admins.py
+-rw-r--r--   0 moky       (501) staff       (20)     7683 2023-12-04 10:58:47.000000 dimp-2.0.0/dimp/dkd/groups.py
+-rw-r--r--   0 moky       (501) staff       (20)     4391 2023-10-13 08:19:45.000000 dimp-2.0.0/dimp/dkd/money.py
+-rw-r--r--   0 moky       (501) staff       (20)     4737 2023-10-29 06:21:49.000000 dimp-2.0.0/dimp/dkd/receipt.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-10 15:40:05.000000 dimp-2.0.0/dimp/mkm/
+-rw-r--r--   0 moky       (501) staff       (20)     2591 2023-10-29 06:06:22.000000 dimp-2.0.0/dimp/mkm/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     2065 2024-05-06 14:57:44.000000 dimp-2.0.0/dimp/mkm/delegate.py
+-rw-r--r--   0 moky       (501) staff       (20)     5965 2023-10-28 15:36:22.000000 dimp-2.0.0/dimp/mkm/docs.py
+-rw-r--r--   0 moky       (501) staff       (20)    10276 2023-10-13 07:54:26.000000 dimp-2.0.0/dimp/mkm/document.py
+-rw-r--r--   0 moky       (501) staff       (20)     5693 2024-05-06 15:03:29.000000 dimp-2.0.0/dimp/mkm/entity.py
+-rw-r--r--   0 moky       (501) staff       (20)     6064 2024-05-06 15:13:53.000000 dimp-2.0.0/dimp/mkm/group.py
+-rw-r--r--   0 moky       (501) staff       (20)     6446 2023-10-29 05:49:42.000000 dimp-2.0.0/dimp/mkm/helper.py
+-rw-r--r--   0 moky       (501) staff       (20)     8637 2023-10-13 16:17:40.000000 dimp-2.0.0/dimp/mkm/meta.py
+-rw-r--r--   0 moky       (501) staff       (20)    11326 2024-05-06 15:07:07.000000 dimp-2.0.0/dimp/mkm/user.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-10 15:40:05.000000 dimp-2.0.0/dimp/msg/
+-rw-r--r--   0 moky       (501) staff       (20)     1737 2023-10-12 08:33:49.000000 dimp-2.0.0/dimp/msg/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     4099 2023-10-28 14:58:31.000000 dimp-2.0.0/dimp/msg/base.py
+-rw-r--r--   0 moky       (501) staff       (20)     4212 2023-10-28 15:04:37.000000 dimp-2.0.0/dimp/msg/envelope.py
+-rw-r--r--   0 moky       (501) staff       (20)     3446 2023-10-28 15:06:22.000000 dimp-2.0.0/dimp/msg/instant.py
+-rw-r--r--   0 moky       (501) staff       (20)     3003 2023-10-28 15:09:07.000000 dimp-2.0.0/dimp/msg/reliable.py
+-rw-r--r--   0 moky       (501) staff       (20)     4012 2023-10-10 10:02:29.000000 dimp-2.0.0/dimp/msg/secure.py
+-rw-r--r--   0 moky       (501) staff       (20)     3326 2024-05-06 10:58:51.000000 dimp-2.0.0/dimp/packer.py
+-rw-r--r--   0 moky       (501) staff       (20)     3136 2024-05-06 10:59:11.000000 dimp-2.0.0/dimp/processor.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-10 15:40:05.000000 dimp-2.0.0/dimp/protocol/
+-rw-r--r--   0 moky       (501) staff       (20)     4228 2023-10-29 06:45:03.000000 dimp-2.0.0/dimp/protocol/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     6144 2023-12-04 11:30:11.000000 dimp-2.0.0/dimp/protocol/commands.py
+-rw-r--r--   0 moky       (501) staff       (20)     7939 2024-05-06 14:37:02.000000 dimp-2.0.0/dimp/protocol/contents.py
+-rw-r--r--   0 moky       (501) staff       (20)     2552 2023-10-10 04:21:03.000000 dimp-2.0.0/dimp/protocol/customized.py
+-rw-r--r--   0 moky       (501) staff       (20)     3386 2023-10-28 14:10:54.000000 dimp-2.0.0/dimp/protocol/docs.py
+-rw-r--r--   0 moky       (501) staff       (20)     8622 2024-05-06 14:34:26.000000 dimp-2.0.0/dimp/protocol/files.py
+-rw-r--r--   0 moky       (501) staff       (20)     7267 2023-12-04 10:59:34.000000 dimp-2.0.0/dimp/protocol/groups.py
+-rw-r--r--   0 moky       (501) staff       (20)     3574 2023-10-29 06:01:28.000000 dimp-2.0.0/dimp/protocol/money.py
+-rw-r--r--   0 moky       (501) staff       (20)     5613 2023-10-10 05:41:02.000000 dimp-2.0.0/dimp/protocol/receipt.py
+-rw-r--r--   0 moky       (501) staff       (20)     9140 2024-05-06 14:58:22.000000 dimp-2.0.0/dimp/transceiver.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-10 15:40:05.000000 dimp-2.0.0/dimp.egg-info/
+-rw-r--r--   0 moky       (501) staff       (20)     1057 2024-05-10 15:40:05.000000 dimp-2.0.0/dimp.egg-info/PKG-INFO
+-rw-r--r--   0 moky       (501) staff       (20)     1060 2024-05-10 15:40:05.000000 dimp-2.0.0/dimp.egg-info/SOURCES.txt
+-rw-r--r--   0 moky       (501) staff       (20)        1 2024-05-10 15:40:05.000000 dimp-2.0.0/dimp.egg-info/dependency_links.txt
+-rw-r--r--   0 moky       (501) staff       (20)       22 2024-05-10 15:40:05.000000 dimp-2.0.0/dimp.egg-info/requires.txt
+-rw-r--r--   0 moky       (501) staff       (20)        5 2024-05-10 15:40:05.000000 dimp-2.0.0/dimp.egg-info/top_level.txt
+-rw-r--r--   0 moky       (501) staff       (20)       38 2024-05-10 15:40:05.000000 dimp-2.0.0/setup.cfg
+-rw-r--r--   0 moky       (501) staff       (20)     1151 2024-05-10 15:39:50.000000 dimp-2.0.0/setup.py
```

### Comparing `dimp-1.0.3/PKG-INFO` & `dimp-2.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dimp
-Version: 1.0.3
+Version: 2.0.0
 Summary: Decentralized Instant Messaging Protocol
 Home-page: https://github.com/dimchat/core-py
 Author: Albert Moky
 Author-email: albert.moky@gmail.com
 License: MIT
 Description: # Decentralized Instant Messaging Protocol (Python)
```

### Comparing `dimp-1.0.3/README.md` & `dimp-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `dimp-1.0.3/dimp/__init__.py` & `dimp-2.0.0/dimp/__init__.py`

 * *Files identical despite different names*

### Comparing `dimp-1.0.3/dimp/barrack.py` & `dimp-2.0.0/dimp/barrack.py`

 * *Files 8% similar despite different names*

```diff
@@ -81,156 +81,156 @@
         """
         finger = 0
         finger = thanos(self.__users, finger)
         finger = thanos(self.__groups, finger)
         return finger >> 1
 
     @abstractmethod  # protected
-    def create_user(self, identifier: ID) -> Optional[User]:
+    async def create_user(self, identifier: ID) -> Optional[User]:
         """
         Create user when visa.key exists
 
         :param identifier: user ID
         :return: user, None on not ready
         """
         raise NotImplemented
 
     @abstractmethod  # protected
-    def create_group(self, identifier: ID) -> Optional[Group]:
+    async def create_group(self, identifier: ID) -> Optional[Group]:
         """
         Create group when members exist
 
         :param identifier: group ID
         :return: group, None on not ready
         """
         raise NotImplemented
 
     # protected
-    def visa_key(self, identifier: ID) -> Optional[EncryptKey]:
-        visa = self.visa(identifier=identifier)
+    async def get_visa_key(self, identifier: ID) -> Optional[EncryptKey]:
+        visa = await self.get_visa(identifier=identifier)
         if visa is not None:  # and visa.valid:
             return visa.public_key
 
     # protected
-    def meta_key(self, identifier: ID) -> Optional[VerifyKey]:
-        meta = self.meta(identifier=identifier)
+    async def get_meta_key(self, identifier: ID) -> Optional[VerifyKey]:
+        meta = await self.get_meta(identifier=identifier)
         if meta is not None:  # and meta.valid:
             return meta.public_key
 
-    def visa(self, identifier: ID) -> Optional[Visa]:
+    async def get_visa(self, identifier: ID) -> Optional[Visa]:
         """ Get last visa document """
-        documents = self.documents(identifier=identifier)
+        documents = await self.get_documents(identifier=identifier)
         return DocumentHelper.last_visa(documents=documents)
 
-    def bulletin(self, identifier: ID) -> Optional[Bulletin]:
+    async def get_bulletin(self, identifier: ID) -> Optional[Bulletin]:
         """ get last bulletin document """
-        documents = self.documents(identifier=identifier)
+        documents = await self.get_documents(identifier=identifier)
         return DocumentHelper.last_bulletin(documents=documents)
 
     #
     #   Entity Delegate
     #
 
     # Override
-    def user(self, identifier: ID) -> Optional[User]:
+    async def get_user(self, identifier: ID) -> Optional[User]:
         # 1. get from user cache
         usr = self.__users.get(identifier)
         if usr is None:
             # 2. create and cache it
-            usr = self.create_user(identifier=identifier)
+            usr = await self.create_user(identifier=identifier)
             if usr is not None:
                 self.cache_user(user=usr)
         return usr
 
     # Override
-    def group(self, identifier: ID) -> Optional[Group]:
+    async def get_group(self, identifier: ID) -> Optional[Group]:
         # 1. get from group cache
         grp = self.__groups.get(identifier)
         if grp is None:
             # 2. create and cache it
-            grp = self.create_group(identifier=identifier)
+            grp = await self.create_group(identifier=identifier)
             if grp is not None:
                 self.cache_group(group=grp)
         return grp
 
     #
     #   UserDataSource
     #
 
     # Override
-    def public_key_for_encryption(self, identifier: ID) -> Optional[EncryptKey]:
+    async def public_key_for_encryption(self, identifier: ID) -> Optional[EncryptKey]:
         # 1. get key from visa
-        key = self.visa_key(identifier=identifier)
+        key = await self.get_visa_key(identifier=identifier)
         if key is not None:
             # if visa.key exists, use it for encryption
             return key
         # 2. get key from meta
-        key = self.meta_key(identifier=identifier)
+        key = await self.get_meta_key(identifier=identifier)
         if isinstance(key, EncryptKey):
             # if visa.key not exists and meta.key is encrypt key,
             # use it for encryption
             return key
 
     # Override
-    def public_keys_for_verification(self, identifier: ID) -> List[VerifyKey]:
+    async def public_keys_for_verification(self, identifier: ID) -> List[VerifyKey]:
         keys = []
         # 1. get key from meta
-        key = self.meta_key(identifier=identifier)
+        key = await self.get_meta_key(identifier=identifier)
         if key is not None:
             # the sender may use identity key to sign message.data,
             # try to verify it with meta.key
             keys.append(key)
         # 2. get key from visa
-        key = self.visa_key(identifier=identifier)
+        key = await self.get_visa_key(identifier=identifier)
         if isinstance(key, VerifyKey):
             # the sender may use communication key to sign message.data,
             # so try to verify it with visa.key here
             keys.append(key)
         assert len(keys) > 0, 'failed to get verify key for user: %s' % identifier
         return keys
 
     #
     #   GroupDataSource
     #
 
     # Override
-    def founder(self, identifier: ID) -> Optional[ID]:
+    async def get_founder(self, identifier: ID) -> Optional[ID]:
         # check for broadcast
         if identifier.is_broadcast:
             # founder of broadcast group
             return BroadcastHelper.broadcast_founder(group=identifier)
         # get from document
-        doc = self.bulletin(identifier=identifier)
+        doc = await self.get_bulletin(identifier=identifier)
         if doc is not None:  # and doc.valid:
             return doc.founder
         # TODO: load founder from database
 
     # Override
-    def owner(self, identifier: ID) -> Optional[ID]:
+    async def get_owner(self, identifier: ID) -> Optional[ID]:
         # check for broadcast
         if identifier.is_broadcast:
             # owner of broadcast group
             return BroadcastHelper.broadcast_owner(group=identifier)
         # check group type
         if identifier.type == EntityType.GROUP:
             # Polylogue's owner is its founder
-            return self.founder(identifier=identifier)
+            return await self.get_founder(identifier=identifier)
         # TODO: load owner from database
 
     # Override
-    def members(self, identifier: ID) -> List[ID]:
+    async def get_members(self, identifier: ID) -> List[ID]:
         # check for broadcast
         if identifier.is_broadcast:
             # members of broadcast group
             return BroadcastHelper.broadcast_members(group=identifier)
         # TODO: load members from database
         return []
 
     # Override
-    def assistants(self, identifier: ID) -> List[ID]:
-        doc = self.bulletin(identifier=identifier)
+    async def get_assistants(self, identifier: ID) -> List[ID]:
+        doc = await self.get_bulletin(identifier=identifier)
         if doc is not None:  # and doc.valid:
             bots = doc.assistants
             if bots is not None:
                 return bots
         # TODO: get group bots from SP configuration
         return []
```

### Comparing `dimp-1.0.3/dimp/crypto/__init__.py` & `dimp-2.0.0/dimp/crypto/__init__.py`

 * *Files identical despite different names*

### Comparing `dimp-1.0.3/dimp/crypto/keys.py` & `dimp-2.0.0/dimp/crypto/keys.py`

 * *Files identical despite different names*

### Comparing `dimp-1.0.3/dimp/crypto/pnf.py` & `dimp-2.0.0/dimp/crypto/pnf.py`

 * *Files identical despite different names*

### Comparing `dimp-1.0.3/dimp/crypto/ted.py` & `dimp-2.0.0/dimp/crypto/ted.py`

 * *Files identical despite different names*

### Comparing `dimp-1.0.3/dimp/dkd/__init__.py` & `dimp-2.0.0/dimp/dkd/__init__.py`

 * *Files identical despite different names*

### Comparing `dimp-1.0.3/dimp/dkd/base.py` & `dimp-2.0.0/dimp/dkd/base.py`

 * *Files identical despite different names*

### Comparing `dimp-1.0.3/dimp/dkd/commands.py` & `dimp-2.0.0/dimp/dkd/commands.py`

 * *Files identical despite different names*

### Comparing `dimp-1.0.3/dimp/dkd/contents.py` & `dimp-2.0.0/dimp/dkd/contents.py`

 * *Files 17% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 # ==============================================================================
 
 from typing import Optional, Any, Dict, List
 
-from mkm.format import TransportableData, PortableNetworkFile
+from mkm.format import PortableNetworkFile
 from mkm.types import URI
 from mkm import ID
 from dkd import ContentType, Content
 from dkd import ReliableMessage
 
 from ..protocol import TextContent, ArrayContent, ForwardContent
 from ..protocol import PageContent, NameCard
@@ -195,38 +195,34 @@
             encoding  : "utf8",
             base      : "about:blank"     // Base URL
         }
     """
 
     def __init__(self, content: Dict[str, Any] = None,
                  url: URI = None, html: str = None, title: str = None,
-                 desc: Optional[str] = None, icon: Optional[TransportableData] = None):
+                 desc: Optional[str] = None, icon: Optional[URI] = None):
         if content is None:
             # 1. new content with url, title, desc & icon
             assert url is not None and title is not None, 'page info error: %s, %s, %s, %s' % (url, title, desc, icon)
             msg_type = ContentType.PAGE.value
             super().__init__(None, msg_type)
-            # URL or HTML
-            if url is not None:
-                self.url = url
-            if html is not None:
-                self.html = html
-            # title, icon, description
-            self.title = title
-            if desc is not None:
-                self.desc = desc
-            if icon is not None:
-                self.set_icon(icon)
         else:
             # 2. content info from network
-            assert url is None and title is None and desc is None and icon is None, \
-                'params error: %s, %s, %s, %s, %s' % (content, url, title, desc, icon)
             super().__init__(content)
-        # lazy
-        self.__icon = icon
+        # URL or HTML
+        if url is not None:
+            self.url = url
+        if html is not None:
+            self.html = html
+        # title, icon, description
+        self.title = title
+        if desc is not None:
+            self.desc = desc
+        if icon is not None:
+            self.icon = icon
 
     #
     #   Web Title
     #
 
     @property  # Override
     def title(self) -> str:
@@ -237,36 +233,22 @@
         self['title'] = string
 
     #
     #   Fav Icon
     #
 
     @property  # Override
-    def icon(self) -> Optional[bytes]:
-        ted = self.__icon
-        if ted is None:
-            base64 = self.get('icon')
-            self.__icon = ted = TransportableData.parse(base64)
-        if ted is not None:
-            return ted.data
+    def icon(self) -> Optional[URI]:
+        base64 = self.get_str(key='icon', default=None)
+        # TODO: convert 'data:' URI
+        return base64
 
     @icon.setter  # Override
-    def icon(self, image: Optional[bytes]):
-        if image is None or len(image) == 0:
-            ted = None
-        else:
-            ted = TransportableData.create(data=image)
-        self.set_icon(ted)
-
-    def set_icon(self, ted: Optional[TransportableData]):
-        if ted is None:
-            self.pop('icon')
-        else:
-            self['icon'] = ted.object
-        self.__icon = ted
+    def icon(self, base64: URI):
+        self['icon'] = base64
 
     #
     #   Description
     #
 
     @property  # Override
     def desc(self) -> Optional[str]:
```

### Comparing `dimp-1.0.3/dimp/dkd/customized.py` & `dimp-2.0.0/dimp/dkd/customized.py`

 * *Files identical despite different names*

### Comparing `dimp-1.0.3/dimp/dkd/factory.py` & `dimp-2.0.0/dimp/dkd/factory.py`

 * *Files identical despite different names*

### Comparing `dimp-1.0.3/dimp/dkd/files.py` & `dimp-2.0.0/dimp/protocol/files.py`

 * *Files 16% similar despite different names*

```diff
@@ -24,215 +24,234 @@
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 # ==============================================================================
 
-from typing import Optional, Any, Dict
+from abc import ABC, abstractmethod
+from typing import Optional
 
-from mkm.format import TransportableData
 from mkm.types import URI
+from mkm.format import TransportableData
 from mkm.crypto import DecryptKey
-
-from dkd import ContentType
-
-from ..crypto import BaseFileWrapper
-from ..protocol import FileContent, ImageContent, AudioContent, VideoContent
-
-from .contents import BaseContent
+from dkd import ContentType, Content
 
 
-class BaseFileContent(BaseContent, FileContent):
+class FileContent(Content, ABC):
     """
         File Message Content
         ~~~~~~~~~~~~~~~~~~~~
 
         data format: {
             type : 0x10,
             sn   : 123,
 
-            URL      : "http://", // upload to CDN
-            data     : "...",     // if (!URL) base64_encode(fileContent)
-            filename : "..."
+            data     : "...",        // base64_encode(fileContent)
+            filename : "photo.png",
+
+            URL      : "http://...", // download from CDN
+            // before fileContent uploaded to a public CDN,
+            // it should be encrypted by a symmetric key
+            key      : {             // symmetric key to decrypt file content
+                algorithm : "AES",   // "DES", ...
+                data      : "{BASE64_ENCODE}",
+                ...
+            }
         }
     """
 
-    def __init__(self, content: Dict[str, Any] = None,
-                 msg_type: int = None,
-                 data: Optional[TransportableData] = None, filename: Optional[str] = None,
-                 url: Optional[URI] = None, password: Optional[DecryptKey] = None):
-        if content is None:
-            # 1. new content with type, data, filename, url & password
-            if msg_type is None:
-                msg_type = ContentType.FILE.value
-            super().__init__(None, msg_type)
-            # access via the wrapper
-            wrapper = BaseFileWrapper(dictionary=self.dictionary)
-            if data is not None:
-                wrapper.data = data
-            if filename is not None:
-                wrapper.filename = filename
-            if url is not None:
-                wrapper.url = url
-            if password is not None:
-                wrapper.password = password
-        else:
-            # 2. content from network
-            assert msg_type is None and data is None and filename is None and url is None and password is None, \
-                'params error: %s, %s, %s, %s, %s, %s' % (content, msg_type, data, filename, url, password)
-            super().__init__(content)
-            wrapper = BaseFileWrapper(dictionary=self.dictionary)
-        self.__wrapper = wrapper
-
-    @property  # Override
+    @property
+    @abstractmethod
     def data(self) -> Optional[bytes]:
-        ted = self.__wrapper.data
-        if ted is not None:
-            return ted.data
-
-    @data.setter  # Override
-    def data(self, attachment: bytes):
-        self.__wrapper.set_data(attachment)
+        # file data (it's too big to set in the dictionary)
+        raise NotImplemented
+
+    @data.setter
+    @abstractmethod
+    def data(self, attachment: Optional[bytes]):
+        raise NotImplemented
 
-    @property  # Override
+    @property
+    @abstractmethod
     def filename(self) -> Optional[str]:
-        return self.__wrapper.filename
+        raise NotImplemented
 
-    @filename.setter  # Override
+    @filename.setter
+    @abstractmethod
     def filename(self, name: str):
-        self.__wrapper.filename = name
+        raise NotImplemented
 
-    @property  # Override
+    @property
+    @abstractmethod
     def url(self) -> Optional[URI]:
-        return self.__wrapper.url
+        raise NotImplemented
 
-    @url.setter  # Override
-    def url(self, remote: str):
-        self.__wrapper.url = remote
+    @url.setter
+    @abstractmethod
+    def url(self, remote: URI):
+        raise NotImplemented
 
-    @property  # Override
+    @property
+    @abstractmethod
     def password(self) -> Optional[DecryptKey]:
-        return self.__wrapper.password
+        """ symmetric key to decrypt the encrypted data from URL """
+        raise NotImplemented
 
-    @password.setter  # Override
+    @password.setter
+    @abstractmethod
     def password(self, key: DecryptKey):
-        self.__wrapper.password = key
+        raise NotImplemented
 
+    #
+    #  Factories
+    #
+
+    @classmethod
+    def create(cls, msg_type: int,
+               data: Optional[TransportableData] = None, filename: Optional[str] = None,
+               url: Optional[URI] = None, password: Optional[DecryptKey] = None):
+        assert msg_type > 0, 'file type error: %d' % msg_type
+        if msg_type == ContentType.IMAGE.value:
+            from ..dkd import ImageFileContent
+            return ImageFileContent(data=data, filename=filename, url=url, password=password)
+        elif msg_type == ContentType.AUDIO.value:
+            from ..dkd import AudioFileContent
+            return AudioFileContent(data=data, filename=filename, url=url, password=password)
+        elif msg_type == ContentType.VIDEO.value:
+            from ..dkd import VideoFileContent
+            return VideoFileContent(data=data, filename=filename, url=url, password=password)
+        else:
+            from ..dkd import BaseFileContent
+            return BaseFileContent(msg_type=msg_type, data=data, filename=filename, url=url, password=password)
+
+    @classmethod
+    def file(cls, data: Optional[TransportableData] = None, filename: Optional[str] = None,
+             url: Optional[URI] = None, password: Optional[DecryptKey] = None):
+        from ..dkd import BaseFileContent
+        return BaseFileContent(data=data, filename=filename, url=url, password=password)
+
+    @classmethod
+    def image(cls, data: Optional[TransportableData] = None, filename: Optional[str] = None,
+              url: Optional[URI] = None, password: Optional[DecryptKey] = None):
+        from ..dkd import ImageFileContent
+        return ImageFileContent(data=data, filename=filename, url=url, password=password)
+
+    @classmethod
+    def audio(cls, data: Optional[TransportableData] = None, filename: Optional[str] = None,
+              url: Optional[URI] = None, password: Optional[DecryptKey] = None):
+        from ..dkd import AudioFileContent
+        return AudioFileContent(data=data, filename=filename, url=url, password=password)
+
+    @classmethod
+    def video(cls, data: Optional[TransportableData] = None, filename: Optional[str] = None,
+              url: Optional[URI] = None, password: Optional[DecryptKey] = None):
+        from ..dkd import VideoFileContent
+        return VideoFileContent(data=data, filename=filename, url=url, password=password)
 
-class ImageFileContent(BaseFileContent, ImageContent):
+
+class ImageContent(FileContent, ABC):
     """
         Image Message Content
         ~~~~~~~~~~~~~~~~~~~~~
 
         data format: {
             type : 0x12,
             sn   : 123,
 
-            URL       : "http://", // upload to CDN
-            data      : "...",     // if (!URL) base64_encode(image)
-            thumbnail : "...",     // base64_encode(smallImage)
-            filename  : "..."
+            data     : "...",        // base64_encode(fileContent)
+            filename : "photo.png",
+
+            URL      : "http://...", // download from CDN
+            // before fileContent uploaded to a public CDN,
+            // it should be encrypted by a symmetric key
+            key      : {             // symmetric key to decrypt file content
+                algorithm : "AES",   // "DES", ...
+                data      : "{BASE64_ENCODE}",
+                ...
+            },
+            thumbnail : "data:image/jpeg;base64,..."
         }
     """
 
-    def __init__(self, content: Dict[str, Any] = None,
-                 data: Optional[TransportableData] = None, filename: Optional[str] = None,
-                 url: Optional[URI] = None, password: Optional[DecryptKey] = None):
-        msg_type = ContentType.IMAGE.value if content is None else None
-        super().__init__(content, msg_type, data=data, filename=filename, url=url, password=password)
-        # lazy load
-        self.__thumbnail: Optional[TransportableData] = None
-
-    @property  # Override
-    def thumbnail(self) -> Optional[bytes]:
-        ted = self.__thumbnail
-        if ted is None:
-            base64 = self.get('thumbnail')
-            self.__thumbnail = ted = TransportableData.parse(base64)
-        if ted is not None:
-            return ted.data
-
-    @thumbnail.setter  # Override
-    def thumbnail(self, image: bytes):
-        if image is None:  # or len(image) == 0:
-            self.pop('thumbnail', None)
-            ted = None
-        else:
-            ted = TransportableData.create(data=image)
-            self['thumbnail'] = ted.object
-        self.__thumbnail = ted
+    @property
+    @abstractmethod
+    def thumbnail(self) -> Optional[URI]:
+        # thumbnail of image
+        raise NotImplemented
+
+    @thumbnail.setter
+    @abstractmethod
+    def thumbnail(self, base64: URI):
+        raise NotImplemented
 
 
-class AudioFileContent(BaseFileContent, AudioContent):
+class AudioContent(FileContent, ABC):
     """
         Audio Message Content
         ~~~~~~~~~~~~~~~~~~~~~
 
         data format: {
             type : 0x14,
             sn   : 123,
 
-            URL      : "http://", // upload to CDN
-            data     : "...",     // if (!URL) base64_encode(audio)
-            text     : "...",     // Automatic Speech Recognition
-            filename : "..."
+            data     : "...",        // base64_encode(fileContent)
+            filename : "photo.png",
+
+            URL      : "http://...", // download from CDN
+            // before fileContent uploaded to a public CDN,
+            // it should be encrypted by a symmetric key
+            key      : {             // symmetric key to decrypt file content
+                algorithm : "AES",   // "DES", ...
+                data      : "{BASE64_ENCODE}",
+                ...
+            },
+            text     : "..."         // Automatic Speech Recognition
         }
     """
 
-    def __init__(self, content: Dict[str, Any] = None,
-                 data: Optional[TransportableData] = None, filename: Optional[str] = None,
-                 url: Optional[URI] = None, password: Optional[DecryptKey] = None):
-        msg_type = ContentType.AUDIO.value if content is None else None
-        super().__init__(content, msg_type, data=data, filename=filename, url=url, password=password)
-
-    @property  # Override
-    def text(self) -> Optional[str]:
-        return self.get_str(key='text', default=None)
+    @property
+    @abstractmethod
+    def text(self) -> Optional[bytes]:
+        # Automatic Speech Recognition
+        raise NotImplemented
 
-    @text.setter  # Override
+    @text.setter
+    @abstractmethod
     def text(self, asr: str):
-        self['text'] = asr
+        raise NotImplemented
 
 
-class VideoFileContent(BaseFileContent, VideoContent):
+class VideoContent(FileContent, ABC):
     """
         Video Message Content
         ~~~~~~~~~~~~~~~~~~~~~
 
         data format: {
             type : 0x16,
             sn   : 123,
 
-            URL      : "http://", // upload to CDN
-            data     : "...",     // if (!URL) base64_encode(video)
-            snapshot : "...",     // base64_encode(smallImage)
-            filename : "..."
+            data     : "...",        // base64_encode(fileContent)
+            filename : "photo.png",
+
+            URL      : "http://...", // download from CDN
+            // before fileContent uploaded to a public CDN,
+            // it should be encrypted by a symmetric key
+            key      : {             // symmetric key to decrypt file content
+                algorithm : "AES",   // "DES", ...
+                data      : "{BASE64_ENCODE}",
+                ...
+            },
+            snapshot : "data:image/jpeg;base64,..."
         }
     """
 
-    def __init__(self, content: Dict[str, Any] = None,
-                 data: Optional[TransportableData] = None, filename: Optional[str] = None,
-                 url: Optional[URI] = None, password: Optional[DecryptKey] = None):
-        msg_type = ContentType.VIDEO.value if content is None else None
-        super().__init__(content, msg_type, data=data, filename=filename, url=url, password=password)
-        # lazy load
-        self.__snapshot: Optional[TransportableData] = None
-
-    @property  # Override
-    def snapshot(self) -> Optional[bytes]:
-        ted = self.__snapshot
-        if ted is None:
-            base64 = self.get('snapshot')
-            self.__snapshot = ted = TransportableData.parse(base64)
-        if ted is not None:
-            return ted.data
-
-    @snapshot.setter  # Override
-    def snapshot(self, image: bytes):
-        if image is None:  # or len(image) == 0:
-            self.pop('snapshot', None)
-            ted = None
-        else:
-            ted = TransportableData.create(data=image)
-            self['snapshot'] = ted.object
-        self.__snapshot = ted
+    @property
+    @abstractmethod
+    def snapshot(self) -> Optional[URI]:
+        # snapshot of video
+        raise NotImplemented
+
+    @snapshot.setter
+    @abstractmethod
+    def snapshot(self, base64: URI):
+        raise NotImplemented
```

### Comparing `dimp-1.0.3/dimp/dkd/group_admins.py` & `dimp-2.0.0/dimp/dkd/group_admins.py`

 * *Files identical despite different names*

### Comparing `dimp-1.0.3/dimp/dkd/groups.py` & `dimp-2.0.0/dimp/dkd/groups.py`

 * *Files identical despite different names*

### Comparing `dimp-1.0.3/dimp/dkd/money.py` & `dimp-2.0.0/dimp/dkd/money.py`

 * *Files identical despite different names*

### Comparing `dimp-1.0.3/dimp/dkd/receipt.py` & `dimp-2.0.0/dimp/dkd/receipt.py`

 * *Files identical despite different names*

### Comparing `dimp-1.0.3/dimp/mkm/__init__.py` & `dimp-2.0.0/dimp/mkm/__init__.py`

 * *Files identical despite different names*

### Comparing `dimp-1.0.3/dimp/mkm/delegate.py` & `dimp-2.0.0/dimp/mkm/delegate.py`

 * *Files 10% similar despite different names*

```diff
@@ -37,25 +37,25 @@
 from .user import User
 from .group import Group
 
 
 class EntityDelegate(ABC):
 
     @abstractmethod
-    def user(self, identifier: ID) -> Optional[User]:
+    async def get_user(self, identifier: ID) -> Optional[User]:
         """
         Create user with ID
 
         :param identifier: ID object
         :return: User object
         """
         raise NotImplemented
 
     @abstractmethod
-    def group(self, identifier: ID) -> Optional[Group]:
+    async def get_group(self, identifier: ID) -> Optional[Group]:
         """
         Create group with ID
 
         :param identifier: ID object
         :return: Group object
         """
         raise NotImplemented
```

### Comparing `dimp-1.0.3/dimp/mkm/docs.py` & `dimp-2.0.0/dimp/mkm/docs.py`

 * *Files identical despite different names*

### Comparing `dimp-1.0.3/dimp/mkm/document.py` & `dimp-2.0.0/dimp/mkm/document.py`

 * *Files identical despite different names*

### Comparing `dimp-1.0.3/dimp/mkm/entity.py` & `dimp-2.0.0/dimp/mkm/entity.py`

 * *Files 4% similar despite different names*

```diff
@@ -44,25 +44,25 @@
         1. meta for user, which is generated by the user's private key
         2. meta for group, which is generated by the founder's private key
         3. meta key, which can verify message sent by this user(or group founder)
         4. visa key, which can encrypt message for the receiver(user)
     """
 
     @abstractmethod
-    def meta(self, identifier: ID) -> Optional[Meta]:
+    async def get_meta(self, identifier: ID) -> Optional[Meta]:
         """
         Get meta for entity
 
         :param identifier: entity ID
         :return: Meta object
         """
         raise NotImplemented
 
     @abstractmethod
-    def documents(self, identifier: ID) -> List[Document]:
+    async def get_documents(self, identifier: ID) -> List[Document]:
         """
         Get documents for entity ID
 
         :param identifier: entity ID
         :return: Document list
         """
         raise NotImplemented
@@ -100,21 +100,21 @@
     @abstractmethod
     def type(self) -> int:
         """ Entity type """
         raise NotImplemented
 
     @property
     @abstractmethod
-    def meta(self) -> Meta:
+    async def meta(self) -> Meta:
         """ Get meta """
         raise NotImplemented
 
     @property
     @abstractmethod
-    def documents(self) -> List[Document]:
+    async def documents(self) -> List[Document]:
         """ Get documents """
         raise NotImplemented
 
 
 class BaseEntity(Entity):
 
     def __init__(self, identifier: ID):
@@ -172,17 +172,17 @@
 
     @property  # Override
     def type(self) -> int:
         """ Entity type """
         return self.__id.type
 
     @property  # Override
-    def meta(self) -> Meta:
+    async def meta(self) -> Meta:
         delegate = self.data_source
         # assert delegate is not None, 'entity delegate not set yet'
-        return delegate.meta(identifier=self.__id)
+        return await delegate.get_meta(identifier=self.__id)
 
     @property  # Override
-    def documents(self) -> List[Document]:
+    async def documents(self) -> List[Document]:
         delegate = self.data_source
         # assert delegate is not None, 'entity delegate not set yet'
-        return delegate.documents(identifier=self.__id)
+        return await delegate.get_documents(identifier=self.__id)
```

### Comparing `dimp-1.0.3/dimp/mkm/group.py` & `dimp-2.0.0/dimp/mkm/group.py`

 * *Files 20% similar despite different names*

```diff
@@ -46,45 +46,45 @@
         ~~~~~~~~~~~~~~~~~
 
         1. founder has the same public key with the group's meta.key
         2. owner and members should be set complying with the consensus algorithm
     """
 
     @abstractmethod
-    def founder(self, identifier: ID) -> Optional[ID]:
+    async def get_founder(self, identifier: ID) -> Optional[ID]:
         """
         Get founder of the group
 
         :param identifier: group ID
         :return: founder ID
         """
         raise NotImplemented
 
     @abstractmethod
-    def owner(self, identifier: ID) -> Optional[ID]:
+    async def get_owner(self, identifier: ID) -> Optional[ID]:
         """
         Get current owner of the group
 
         :param identifier: group ID
         :return: owner ID
         """
         raise NotImplemented
 
     @abstractmethod
-    def members(self, identifier: ID) -> List[ID]:
+    async def get_members(self, identifier: ID) -> List[ID]:
         """
         Get all members in the group
 
         :param identifier: group ID
         :return: member ID list
         """
         raise NotImplemented
 
     @abstractmethod
-    def assistants(self, identifier: ID) -> List[ID]:
+    async def get_assistants(self, identifier: ID) -> List[ID]:
         """
         Get assistants for this group
 
         :param identifier: group ID
         :return: bot ID list
         """
         raise NotImplemented
@@ -112,39 +112,39 @@
     # @data_source.setter
     # @abstractmethod
     # def data_source(self, delegate: GroupDataSource):
     #     raise NotImplemented
 
     @property
     @abstractmethod
-    def bulletin(self) -> Optional[Bulletin]:
+    async def bulletin(self) -> Optional[Bulletin]:
         """ Group Document """
         # return self.document(doc_type=Document.BULLETIN)
         raise NotImplemented
 
     @property
     @abstractmethod
-    def founder(self) -> ID:
+    async def founder(self) -> ID:
         raise NotImplemented
 
     @property
     @abstractmethod
-    def owner(self) -> ID:
+    async def owner(self) -> ID:
         raise NotImplemented
 
     @property
     @abstractmethod
-    def members(self) -> List[ID]:
+    async def members(self) -> List[ID]:
         """ NOTICE: the owner must be a member
             (usually the first one) """
         raise NotImplemented
 
     @property
     @abstractmethod
-    def assistants(self) -> List[ID]:
+    async def assistants(self) -> List[ID]:
         raise NotImplemented
 
 
 class BaseGroup(BaseEntity, Group):
 
     def __init__(self, identifier: ID):
         super().__init__(identifier=identifier)
@@ -156,35 +156,36 @@
         return super().data_source
 
     # @data_source.setter  # Override
     # def data_source(self, delegate: GroupDataSource):
     #     super(BaseGroup, BaseGroup).data_source.__set__(self, delegate)
 
     @property  # Override
-    def bulletin(self) -> Optional[Bulletin]:
-        return DocumentHelper.last_bulletin(documents=self.documents)
+    async def bulletin(self) -> Optional[Bulletin]:
+        docs = await self.documents
+        return await DocumentHelper.last_bulletin(documents=docs)
 
     @property  # Override
-    def founder(self) -> ID:
+    async def founder(self) -> ID:
         if self.__founder is None:
-            delegate = self.data_source
-            # assert delegate is not None, 'group delegate not set yet'
-            self.__founder = delegate.founder(identifier=self.identifier)
+            barrack = self.data_source
+            # assert isinstance(barrack, GroupDataSource), 'group delegate error: %s' % barrack
+            self.__founder = await barrack.get_founder(identifier=self.identifier)
         return self.__founder
 
     @property  # Override
-    def owner(self) -> ID:
-        delegate = self.data_source
-        # assert delegate is not None, 'group delegate not set yet'
-        return delegate.owner(identifier=self.identifier)
+    async def owner(self) -> ID:
+        barrack = self.data_source
+        # assert isinstance(barrack, GroupDataSource), 'group delegate error: %s' % barrack
+        return await barrack.get_owner(identifier=self.identifier)
 
     @property  # Override
-    def members(self) -> List[ID]:
-        delegate = self.data_source
-        # assert delegate is not None, 'group delegate not set yet'
-        return delegate.members(identifier=self.identifier)
+    async def members(self) -> List[ID]:
+        barrack = self.data_source
+        # assert isinstance(barrack, GroupDataSource), 'group delegate error: %s' % barrack
+        return await barrack.get_members(identifier=self.identifier)
 
     @property  # Override
-    def assistants(self) -> List[ID]:
-        delegate = self.data_source
-        # assert delegate is not None, 'group delegate not set yet'
-        return delegate.assistants(identifier=self.identifier)
+    async def assistants(self) -> List[ID]:
+        barrack = self.data_source
+        # assert isinstance(barrack, GroupDataSource), 'group delegate error: %s' % barrack
+        return await barrack.get_assistants(identifier=self.identifier)
```

### Comparing `dimp-1.0.3/dimp/mkm/helper.py` & `dimp-2.0.0/dimp/mkm/helper.py`

 * *Files identical despite different names*

### Comparing `dimp-1.0.3/dimp/mkm/meta.py` & `dimp-2.0.0/dimp/mkm/meta.py`

 * *Files identical despite different names*

### Comparing `dimp-1.0.3/dimp/mkm/user.py` & `dimp-2.0.0/dimp/mkm/user.py`

 * *Files 6% similar despite different names*

```diff
@@ -62,69 +62,69 @@
         5. private key for visa signature
            the private key pared with meta.key
         6. public key for visa verification
            meta.key only
     """
 
     @abstractmethod
-    def contacts(self, identifier: ID) -> List[ID]:
+    async def get_contacts(self, identifier: ID) -> List[ID]:
         """
         Get user's contacts list
 
         :param identifier: user ID
         :return: contact ID list
         """
         pass
 
     @abstractmethod
-    def public_key_for_encryption(self, identifier: ID) -> Optional[EncryptKey]:
+    async def public_key_for_encryption(self, identifier: ID) -> Optional[EncryptKey]:
         """
         Get user's public key for encryption
         (visa.key or meta.key)
 
         :param identifier: user ID
         :return: public key
         """
         pass
 
     @abstractmethod
-    def public_keys_for_verification(self, identifier: ID) -> List[VerifyKey]:
+    async def public_keys_for_verification(self, identifier: ID) -> List[VerifyKey]:
         """
         Get user's public keys for verification
         [visa.key, meta.key]
 
         :param identifier: user ID
         :return: public keys
         """
         pass
 
     @abstractmethod
-    def private_keys_for_decryption(self, identifier: ID) -> List[DecryptKey]:
+    async def private_keys_for_decryption(self, identifier: ID) -> List[DecryptKey]:
         """
         Get user's private keys for decryption
         (which paired with [visa.key, meta.key])
 
         :param identifier: user ID
         :return: private keys
         """
         raise NotImplemented
 
     @abstractmethod
-    def private_key_for_signature(self, identifier: ID) -> Optional[SignKey]:
+    async def private_key_for_signature(self, identifier: ID) -> Optional[SignKey]:
         """
         Get user's private key for signature
         (which paired with visa.key or meta.key)
 
         :param identifier: user ID
         :return: private key
         """
         raise NotImplemented
 
     @abstractmethod
-    def private_key_for_visa_signature(self, identifier: ID) -> Optional[SignKey]:
+    async def private_key_for_visa_signature(self, identifier: ID) -> Optional[SignKey]:
         """
         Get user's private key for signing visa
 
         :param identifier: user ID
         :return: private key
         """
         raise NotImplemented
@@ -153,85 +153,85 @@
     # @data_source.setter
     # @abstractmethod
     # def data_source(self, delegate: UserDataSource):
     #     raise NotImplemented
 
     @property
     @abstractmethod
-    def visa(self) -> Optional[Visa]:
+    async def visa(self) -> Optional[Visa]:
         """ User Document """
         # return self.document(doc_type=Document.VISA)
         raise NotImplemented
 
     @property
     @abstractmethod
-    def contacts(self) -> List[ID]:
+    async def contacts(self) -> List[ID]:
         """
         Get all contacts of the user
 
         :return: contacts list
         """
         raise NotImplemented
 
     @abstractmethod
-    def verify(self, data: bytes, signature: bytes) -> bool:
+    async def verify(self, data: bytes, signature: bytes) -> bool:
         """
         Verify data and signature with user's public keys
 
         :param data:
         :param signature:
         :return:
         """
         raise NotImplemented
 
     @abstractmethod
-    def encrypt(self, data: bytes) -> bytes:
+    async def encrypt(self, data: bytes) -> bytes:
         """
         Encrypt data, try visa.key first, if not found, use meta.key
 
         :param data: plaintext
         :return: encrypted data
         """
         raise NotImplemented
 
     #
     #   interfaces for local user
     #
 
     @abstractmethod
-    def sign(self, data: bytes) -> bytes:
+    async def sign(self, data: bytes) -> bytes:
         """
         Sign data with user's private key
 
         :param data: message data
         :return: signature
         """
         raise NotImplemented
 
     @abstractmethod
-    def decrypt(self, data: bytes) -> Optional[bytes]:
+    async def decrypt(self, data: bytes) -> Optional[bytes]:
         """
         Decrypt data with user's private key(s)
 
         :param data: encrypted data
         :return: plaintext
         """
         raise NotImplemented
 
     #
     #   Interfaces for Visa
     #
 
     @abstractmethod
-    def sign_visa(self, visa: Visa) -> Optional[Visa]:
+    async def sign_visa(self, visa: Visa) -> Optional[Visa]:
         # NOTICE: only sign visa with the private key paired with your meta.key
         raise NotImplemented
 
     @abstractmethod
-    def verify_visa(self, visa: Visa) -> bool:
+    async def verify_visa(self, visa: Visa) -> bool:
         # NOTICE: only verify visa with meta.key
         #         (if meta not exists, user won't be created)
         raise NotImplemented
 
 
 class BaseUser(BaseEntity, User):
 
@@ -243,87 +243,89 @@
         return super().data_source
 
     # @data_source.setter  # Override
     # def data_source(self, barrack: UserDataSource):
     #     super(BaseUser, BaseUser).data_source.__set__(self, barrack)
 
     @property  # Override
-    def visa(self) -> Optional[Visa]:
-        return DocumentHelper.last_visa(documents=self.documents)
+    async def visa(self) -> Optional[Visa]:
+        docs = await self.documents
+        return DocumentHelper.last_visa(documents=docs)
 
     @property  # Override
-    def contacts(self) -> List[ID]:
+    async def contacts(self) -> List[ID]:
         barrack = self.data_source
-        # assert barrack is not None, 'user delegate not set yet'
-        return barrack.contacts(identifier=self.identifier)
+        # assert isinstance(barrack, UserDataSource), 'user delegate error: %s' % barrack
+        return await barrack.get_contacts(identifier=self.identifier)
 
     # Override
-    def verify(self, data: bytes, signature: bytes) -> bool:
+    async def verify(self, data: bytes, signature: bytes) -> bool:
         barrack = self.data_source
-        assert barrack is not None, 'user data source not set yet'
-        keys = barrack.public_keys_for_verification(identifier=self.identifier)
+        assert isinstance(barrack, UserDataSource), 'user delegate error: %s' % barrack
+        keys = await barrack.public_keys_for_verification(identifier=self.identifier)
         assert len(keys) > 0, 'failed to get verify keys: %s' % self.identifier
         for key in keys:
             if key.verify(data=data, signature=signature):
                 # matched!
                 return True
         # signature not match
         # TODO: check whether visa is expired, query new document for this contact
 
     # Override
-    def encrypt(self, data: bytes) -> bytes:
+    async def encrypt(self, data: bytes) -> bytes:
         barrack = self.data_source
-        assert isinstance(barrack, UserDataSource), 'user data source error: %s' % barrack
+        assert isinstance(barrack, UserDataSource), 'user delegate error: %s' % barrack
         # NOTICE: meta.key will never changed, so use visa.key to encrypt message
         #         is the better way
-        key = barrack.public_key_for_encryption(identifier=self.identifier)
+        key = await barrack.public_key_for_encryption(identifier=self.identifier)
         assert key is not None, 'failed to get encrypt key for user: %s' % self.identifier
         return key.encrypt(data=data, extra={})
 
     # Override
-    def sign(self, data: bytes) -> bytes:
+    async def sign(self, data: bytes) -> bytes:
         barrack = self.data_source
-        assert barrack is not None, 'user data source not set yet'
-        key = barrack.private_key_for_signature(identifier=self.identifier)
+        assert isinstance(barrack, UserDataSource), 'user delegate error: %s' % barrack
+        key = await barrack.private_key_for_signature(identifier=self.identifier)
         assert key is not None, 'failed to get sign key for user: %s' % self.identifier
         return key.sign(data=data)
 
     # Override
-    def decrypt(self, data: bytes) -> Optional[bytes]:
+    async def decrypt(self, data: bytes) -> Optional[bytes]:
         barrack = self.data_source
-        assert isinstance(barrack, UserDataSource), 'user data source error: %s' % barrack
+        assert isinstance(barrack, UserDataSource), 'user delegate error: %s' % barrack
         # NOTICE: if you provide a public key in visa document for encryption,
         #         here you should return the private key paired with visa.key
-        keys = barrack.private_keys_for_decryption(identifier=self.identifier)
+        keys = await barrack.private_keys_for_decryption(identifier=self.identifier)
         assert len(keys) > 0, 'failed to get decrypt keys: %s' % self.identifier
         for key in keys:
             # try decrypting it with each private key
             plaintext = key.decrypt(data=data, params={})
             if plaintext is not None:
                 # OK!
                 return plaintext
         # decryption failed
         # TODO: check whether my visa key is changed, push new visa to this contact
 
     # Override
-    def sign_visa(self, visa: Visa) -> Optional[Visa]:
+    async def sign_visa(self, visa: Visa) -> Optional[Visa]:
         assert self.identifier == visa.identifier, 'visa ID not match: %s, %s' % (self.identifier, visa)
         barrack = self.data_source
-        assert barrack is not None, 'user data source not set yet'
+        assert isinstance(barrack, UserDataSource), 'user delegate error: %s' % barrack
         # NOTICE: only sign visa with the private key paired with your meta.key
-        key = barrack.private_key_for_visa_signature(identifier=self.identifier)
+        key = await barrack.private_key_for_visa_signature(identifier=self.identifier)
         assert key is not None, 'failed to get sign key for visa: %s' % self.identifier
         if visa.sign(private_key=key) is None:
             assert False, 'failed to sign visa: %s, %s' % (self.identifier, visa)
         else:
             return visa
 
     # Override
-    def verify_visa(self, visa: Visa) -> bool:
+    async def verify_visa(self, visa: Visa) -> bool:
         # NOTICE: only verify visa with meta.key
         #         (if meta not exists, user won't be created)
         if self.identifier != visa.identifier:
             # visa ID not match
             return False
-        key = self.meta.public_key
+        meta = await self.meta
+        key = meta.public_key
         assert key is not None, 'failed to get meta key for visa: %s' % self.identifier
         return visa.verify(public_key=key)
```

### Comparing `dimp-1.0.3/dimp/msg/__init__.py` & `dimp-2.0.0/dimp/msg/__init__.py`

 * *Files identical despite different names*

### Comparing `dimp-1.0.3/dimp/msg/base.py` & `dimp-2.0.0/dimp/msg/base.py`

 * *Files identical despite different names*

### Comparing `dimp-1.0.3/dimp/msg/envelope.py` & `dimp-2.0.0/dimp/msg/envelope.py`

 * *Files identical despite different names*

### Comparing `dimp-1.0.3/dimp/msg/instant.py` & `dimp-2.0.0/dimp/msg/instant.py`

 * *Files identical despite different names*

### Comparing `dimp-1.0.3/dimp/msg/reliable.py` & `dimp-2.0.0/dimp/msg/reliable.py`

 * *Files identical despite different names*

### Comparing `dimp-1.0.3/dimp/msg/secure.py` & `dimp-2.0.0/dimp/msg/secure.py`

 * *Files identical despite different names*

### Comparing `dimp-1.0.3/dimp/packer.py` & `dimp-2.0.0/dimp/packer.py`

 * *Files 3% similar despite different names*

```diff
@@ -40,69 +40,69 @@
 class Packer(ABC):
 
     #
     #   InstantMessage -> SecureMessage -> ReliableMessage -> Data
     #
 
     @abstractmethod
-    def encrypt_message(self, msg: InstantMessage) -> Optional[SecureMessage]:
+    async def encrypt_message(self, msg: InstantMessage) -> Optional[SecureMessage]:
         """
         Encrypt message content
 
         :param msg: plain message
         :return: encrypted message
         """
         raise NotImplemented
 
     @abstractmethod
-    def sign_message(self, msg: SecureMessage) -> Optional[ReliableMessage]:
+    async def sign_message(self, msg: SecureMessage) -> Optional[ReliableMessage]:
         """
         Sign content data
 
         :param msg: encrypted message
         :return: network message
         """
         raise NotImplemented
 
     @abstractmethod
-    def serialize_message(self, msg: ReliableMessage) -> Optional[bytes]:
+    async def serialize_message(self, msg: ReliableMessage) -> Optional[bytes]:
         """
         Serialize network message
 
         :param msg: network message
         :return: data package
         """
         raise NotImplemented
 
     #
     #   Data -> ReliableMessage -> SecureMessage -> InstantMessage
     #
 
     @abstractmethod
-    def deserialize_message(self, data: bytes) -> Optional[ReliableMessage]:
+    async def deserialize_message(self, data: bytes) -> Optional[ReliableMessage]:
         """
         Deserialize network message
 
         :param data: data package
         :return: network message
         """
         raise NotImplemented
 
     @abstractmethod
-    def verify_message(self, msg: ReliableMessage) -> Optional[SecureMessage]:
+    async def verify_message(self, msg: ReliableMessage) -> Optional[SecureMessage]:
         """
         Verify encrypted content data
 
         :param msg: network message
         :return: encrypted message
         """
         raise NotImplemented
 
     @abstractmethod
-    def decrypt_message(self, msg: SecureMessage) -> Optional[InstantMessage]:
+    async def decrypt_message(self, msg: SecureMessage) -> Optional[InstantMessage]:
         """
         Decrypt message content
 
         :param msg: encrypted message
         :return: plain message
         """
         raise NotImplemented
```

### Comparing `dimp-1.0.3/dimp/processor.py` & `dimp-2.0.0/dimp/processor.py`

 * *Files 10% similar despite different names*

```diff
@@ -36,57 +36,57 @@
 
 #
 #   Message Processor
 #
 class Processor(ABC):
 
     @abstractmethod
-    def process_package(self, data: bytes) -> List[bytes]:
+    async def process_package(self, data: bytes) -> List[bytes]:
         """
         Process data package
 
         :param data: data to be processed
         :return: responses
         """
         raise NotImplemented
 
     @abstractmethod
-    def process_reliable_message(self, msg: ReliableMessage) -> List[ReliableMessage]:
+    async def process_reliable_message(self, msg: ReliableMessage) -> List[ReliableMessage]:
         """
         Process network message
 
         :param msg: message to be processed
         :return: response messages
         """
         raise NotImplemented
 
     @abstractmethod
-    def process_secure_message(self, msg: SecureMessage, r_msg: ReliableMessage) -> List[SecureMessage]:
+    async def process_secure_message(self, msg: SecureMessage, r_msg: ReliableMessage) -> List[SecureMessage]:
         """
         Process encrypted message
 
         :param msg:   message to be processed
         :param r_msg: message received
         :return: response messages
         """
         raise NotImplemented
 
     @abstractmethod
-    def process_instant_message(self, msg: InstantMessage, r_msg: ReliableMessage) -> List[InstantMessage]:
+    async def process_instant_message(self, msg: InstantMessage, r_msg: ReliableMessage) -> List[InstantMessage]:
         """
         Process plain message
 
         :param msg:   message to be processed
         :param r_msg: message received
         :return: response messages
         """
         raise NotImplemented
 
     @abstractmethod
-    def process_content(self, content: Content, r_msg: ReliableMessage) -> List[Content]:
+    async def process_content(self, content: Content, r_msg: ReliableMessage) -> List[Content]:
         """
         Process message content
 
         :param content: content to be processed
         :param r_msg: message received
         :return: response contents
         """
```

### Comparing `dimp-1.0.3/dimp/protocol/__init__.py` & `dimp-2.0.0/dimp/protocol/__init__.py`

 * *Files identical despite different names*

### Comparing `dimp-1.0.3/dimp/protocol/commands.py` & `dimp-2.0.0/dimp/protocol/commands.py`

 * *Files identical despite different names*

### Comparing `dimp-1.0.3/dimp/protocol/contents.py` & `dimp-2.0.0/dimp/protocol/contents.py`

 * *Files 11% similar despite different names*

```diff
@@ -25,18 +25,18 @@
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 # ==============================================================================
 
 from abc import ABC, abstractmethod
-from typing import Optional, Union, List, Dict, Any
+from typing import Optional, List, Dict, Any
 
 from mkm.types import URI
-from mkm.format import PortableNetworkFile, TransportableData
+from mkm.format import PortableNetworkFile
 from mkm import ID
 from dkd import Content, ReliableMessage
 
 
 class TextContent(Content, ABC):
     """
         Text Message Content
@@ -172,16 +172,16 @@
         ~~~~~~~~~~~~~~~~
 
         data format: {
             type : 0x20,
             sn   : 123,
 
             title : "...",                // Web title
-            icon  : "...",                // base64_encode(icon)
             desc  : "...",
+            icon  : "data:image/x-icon;base64,...",
 
             URL   : "https://github.com/moky/dimp",
 
             HTML      : "...",            // Web content
             mime_type : "text/html",      // Content-Type
             encoding  : "utf8",
             base      : "about:blank"     // Base URL
@@ -204,20 +204,20 @@
 
     #
     #   Fav Icon
     #
 
     @property
     @abstractmethod
-    def icon(self) -> Optional[bytes]:
+    def icon(self) -> Optional[URI]:
         raise NotImplemented
 
     @icon.setter
     @abstractmethod
-    def icon(self, image: bytes):
+    def icon(self, base64: URI):
         raise NotImplemented
 
     #
     #   Description
     #
 
     @property
@@ -259,37 +259,25 @@
         raise NotImplemented
 
     #
     #   Factory methods
     #
     @classmethod
     def create(cls, url: Optional[URI], html: Optional[str], title: str,
-               desc: Optional[str], icon: Optional[TransportableData]):
+               desc: Optional[str], icon: Optional[URI]):
         from ..dkd import WebPageContent
         return WebPageContent(url=url, html=html, title=title, desc=desc, icon=icon)
 
     @classmethod
-    def create_with_url(cls, url: URI, title: str, desc: Optional[str], icon: Union[bytes, str, None]):
-        if isinstance(icon, bytes):
-            ted = TransportableData.create(data=icon)
-        elif isinstance(icon, str):
-            ted = TransportableData.parse(icon)
-        else:
-            ted = None
-        return cls.create(url=url, html=None, title=title, desc=desc, icon=ted)
+    def create_with_url(cls, url: URI, title: str, desc: Optional[str], icon: Optional[URI]):
+        return cls.create(url=url, html=None, title=title, desc=desc, icon=icon)
 
     @classmethod
-    def create_with_html(cls, html: str, title: str, desc: Optional[str], icon: Union[bytes, str, None]):
-        if isinstance(icon, bytes):
-            ted = TransportableData.create(data=icon)
-        elif isinstance(icon, str):
-            ted = TransportableData.parse(icon)
-        else:
-            ted = None
-        return cls.create(url=None, html=html, title=title, desc=desc, icon=ted)
+    def create_with_html(cls, html: str, title: str, desc: Optional[str], icon: Optional[URI]):
+        return cls.create(url=None, html=html, title=title, desc=desc, icon=icon)
 
 
 class NameCard(Content, ABC):
     """
         Name Card Content
         ~~~~~~~~~~~~~~~~~
```

### Comparing `dimp-1.0.3/dimp/protocol/customized.py` & `dimp-2.0.0/dimp/protocol/customized.py`

 * *Files identical despite different names*

### Comparing `dimp-1.0.3/dimp/protocol/docs.py` & `dimp-2.0.0/dimp/protocol/docs.py`

 * *Files identical despite different names*

### Comparing `dimp-1.0.3/dimp/protocol/groups.py` & `dimp-2.0.0/dimp/protocol/groups.py`

 * *Files identical despite different names*

### Comparing `dimp-1.0.3/dimp/protocol/money.py` & `dimp-2.0.0/dimp/protocol/money.py`

 * *Files identical despite different names*

### Comparing `dimp-1.0.3/dimp/protocol/receipt.py` & `dimp-2.0.0/dimp/protocol/receipt.py`

 * *Files identical despite different names*

### Comparing `dimp-1.0.3/dimp/transceiver.py` & `dimp-2.0.0/dimp/transceiver.py`

 * *Files 9% similar despite different names*

```diff
@@ -59,86 +59,86 @@
         raise NotImplemented
 
     #
     #   InstantMessageDelegate
     #
 
     # Override
-    def serialize_content(self, content: Content, key: SymmetricKey, msg: InstantMessage) -> bytes:
+    async def serialize_content(self, content: Content, key: SymmetricKey, msg: InstantMessage) -> bytes:
         # NOTICE: check attachment for File/Image/Audio/Video message content
         #         before serialize content, this job should be do in subclass
         js = json_encode(obj=content.dictionary)
         return utf8_encode(string=js)
 
     # Override
-    def encrypt_content(self, data: bytes, key: SymmetricKey, msg: InstantMessage) -> bytes:
+    async def encrypt_content(self, data: bytes, key: SymmetricKey, msg: InstantMessage) -> bytes:
         # store 'IV' in msg for AES encryption
         return key.encrypt(data=data, extra=msg.dictionary)
 
     # # Override
-    # def encode_data(self, data: bytes, msg: InstantMessage) -> Any:
+    # async def encode_data(self, data: bytes, msg: InstantMessage) -> Any:
     #     if BaseMessage.is_broadcast(msg=msg):
     #         # broadcast message content will not be encrypted (just encoded to JsON),
     #         # so no need to encode to Base64 here
     #         return utf8_decode(data=data)
     #     # message content had been encrypted by a symmetric key,
     #     # so the data should be encoded here (with algorithm 'base64' as default).
     #     return TransportableData.encode(data=data)
 
     # Override
-    def serialize_key(self, key: SymmetricKey, msg: InstantMessage) -> Optional[bytes]:
+    async def serialize_key(self, key: SymmetricKey, msg: InstantMessage) -> Optional[bytes]:
         if BaseMessage.is_broadcast(msg=msg):
             # broadcast message has no key
             return None
         js = json_encode(obj=key.dictionary)
         return utf8_encode(string=js)
 
     # Override
-    def encrypt_key(self, data: bytes, receiver: ID, msg: InstantMessage) -> Optional[bytes]:
+    async def encrypt_key(self, data: bytes, receiver: ID, msg: InstantMessage) -> Optional[bytes]:
         assert not BaseMessage.is_broadcast(msg=msg), 'broadcast message has no key: %s' % msg
         assert receiver.is_user, 'receiver error: %s' % receiver
         # TODO: make sure the receiver's public key exists
-        contact = self.barrack.user(identifier=receiver)
+        contact = await self.barrack.get_user(identifier=receiver)
         if contact is None:
             assert False, 'failed to encrypt message key for receiver: %s' % receiver
         else:
             # encrypt with public key of the receiver (or group member)
-            return contact.encrypt(data=data)
+            return await contact.encrypt(data=data)
 
     # # Override
-    # def encode_key(self, data: bytes, msg: InstantMessage) -> Any:
+    # async def encode_key(self, data: bytes, msg: InstantMessage) -> Any:
     #     assert not BaseMessage.is_broadcast(msg=msg), 'broadcast message has no key: %s' % msg
     #     # message key had been encrypted by a public key,
     #     # so the data should be encode here (with algorithm 'base64' as default).
     #     return TransportableData.encode(data=data)
 
     #
     #   SecureMessageDelegate
     #
 
     # # Override
-    # def decode_key(self, key: Any, msg: SecureMessage) -> Optional[bytes]:
+    # async def decode_key(self, key: Any, msg: SecureMessage) -> Optional[bytes]:
     #     assert not BaseMessage.is_broadcast(msg=msg), 'broadcast message has no key: %s' % msg
     #     return TransportableData.decode(key)
 
     # Override
-    def decrypt_key(self, data: bytes, receiver: ID, msg: SecureMessage) -> Optional[bytes]:
+    async def decrypt_key(self, data: bytes, receiver: ID, msg: SecureMessage) -> Optional[bytes]:
         # NOTICE: the receiver must be a member ID
         #         if it's a group message
         assert not BaseMessage.is_broadcast(msg=msg), 'broadcast message has no key'
         assert receiver.is_user, 'receiver error: %s' % receiver
-        user = self.barrack.user(identifier=receiver)
+        user = await self.barrack.get_user(identifier=receiver)
         if user is None:
             assert False, 'failed to create local user: %s' % msg.receiver
         else:
             # decrypt with private key of the receiver (or group member)
-            return user.decrypt(data=data)
+            return await user.decrypt(data=data)
 
     # Override
-    def deserialize_key(self, data: Optional[bytes], msg: SecureMessage) -> Optional[SymmetricKey]:
+    async def deserialize_key(self, data: Optional[bytes], msg: SecureMessage) -> Optional[SymmetricKey]:
         assert not BaseMessage.is_broadcast(msg=msg), 'broadcast message has no key: %s' % msg
         if data is None:
             # assert False, 'reused key? get it from cache: %s => %s, %s' % (msg.sender, msg.receiver, msg.group)
             return None
         js = utf8_decode(data=data)
         if js is None:
             # assert False, 'message key data error: %s' % data
@@ -149,70 +149,70 @@
         #       'D' -> 'data'
         #       'V' -> 'iv'
         #       'M' -> 'mode'
         #       'P' -> 'padding'
         return SymmetricKey.parse(key=dictionary)
 
     # # Override
-    # def decode_data(self, data: Any, msg: SecureMessage) -> Optional[bytes]:
+    # async def decode_data(self, data: Any, msg: SecureMessage) -> Optional[bytes]:
     #     if BaseMessage.is_broadcast(msg=msg):
     #         # broadcast message content will not be encrypted (just encoded to JsON),
     #         # so return the string data directly
     #         if isinstance(data, str):
     #             return utf8_encode(string=data)
     #         else:
     #             # assert False, 'content data error: %s' % data
     #             return None
     #     else:
     #         # message content had been encrypted by a symmetric key,
     #         # so the data should be encoded here (with algorithm 'base64' as default).
     #         return TransportableData.decode(data)
 
     # Override
-    def decrypt_content(self, data: bytes, key: SymmetricKey, msg: SecureMessage) -> Optional[bytes]:
+    async def decrypt_content(self, data: bytes, key: SymmetricKey, msg: SecureMessage) -> Optional[bytes]:
         # check 'IV' in msg for AES decryption
         return key.decrypt(data=data, params=msg.dictionary)
 
     # Override
-    def deserialize_content(self, data: bytes, key: SymmetricKey, msg: SecureMessage) -> Optional[Content]:
+    async def deserialize_content(self, data: bytes, key: SymmetricKey, msg: SecureMessage) -> Optional[Content]:
         js = utf8_decode(data=data)
         if js is None:
             # assert False, 'content data error: %s' % data
             return None
         dictionary = json_decode(string=js)
         # TODO: translate short keys
         #       'T' -> 'type'
         #       'N' -> 'sn'
         #       'W' -> 'time'
         #       'G' -> 'group'
         return Content.parse(content=dictionary)
 
     # Override
     # noinspection PyUnusedLocal
-    def sign_data(self, data: bytes, msg: SecureMessage) -> bytes:
+    async def sign_data(self, data: bytes, msg: SecureMessage) -> bytes:
         sender = msg.sender
-        user = self.barrack.user(identifier=sender)
+        user = await self.barrack.get_user(identifier=sender)
         if user is None:
             assert False, 'failed to sign message data for sender: %s' % sender
         else:
-            return user.sign(data)
+            return await user.sign(data)
 
     # # Override
-    # def encode_signature(self, signature: bytes, msg: SecureMessage) -> str:
+    # async def encode_signature(self, signature: bytes, msg: SecureMessage) -> str:
     #     return TransportableData.encode(data=signature)
 
     #
     #   ReliableMessageDelegate
     #
 
     # # Override
-    # def decode_signature(self, signature: Any, msg: ReliableMessage) -> Optional[bytes]:
+    # async def decode_signature(self, signature: Any, msg: ReliableMessage) -> Optional[bytes]:
     #     return TransportableData.decode(signature)
 
     # Override
-    def verify_data_signature(self, data: bytes, signature: bytes, msg: ReliableMessage) -> bool:
+    async def verify_data_signature(self, data: bytes, signature: bytes, msg: ReliableMessage) -> bool:
         sender = msg.sender
-        contact = self.barrack.user(identifier=sender)
+        contact = await self.barrack.get_user(identifier=sender)
         if contact is None:
             assert False, 'failed to verify signature for sender: %s' % sender
         else:
-            return contact.verify(data=data, signature=signature)
+            return await contact.verify(data=data, signature=signature)
```

### Comparing `dimp-1.0.3/dimp.egg-info/PKG-INFO` & `dimp-2.0.0/dimp.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dimp
-Version: 1.0.3
+Version: 2.0.0
 Summary: Decentralized Instant Messaging Protocol
 Home-page: https://github.com/dimchat/core-py
 Author: Albert Moky
 Author-email: albert.moky@gmail.com
 License: MIT
 Description: # Decentralized Instant Messaging Protocol (Python)
```

### Comparing `dimp-1.0.3/dimp.egg-info/SOURCES.txt` & `dimp-2.0.0/dimp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dimp-1.0.3/setup.py` & `dimp-2.0.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     communications between accounts safely by end-to-end encryption.
 """
 
 import io
 
 from setuptools import setup, find_packages
 
-__version__ = '1.0.3'
+__version__ = '2.0.0'
 __author__ = 'Albert Moky'
 __contact__ = 'albert.moky@gmail.com'
 
 with io.open('README.md', 'r', encoding='utf-8') as fh:
     readme = fh.read()
 
 setup(
@@ -34,11 +34,11 @@
     packages=find_packages(),
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
     ],
     install_requires=[
-        'dkd>=1.0.2',
-        'mkm>=1.0.2',
+        'dkd>=2.0.0',
+        'mkm>=2.0.0',
     ]
 )
```

