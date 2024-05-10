# Comparing `tmp/redis-hashring-0.3.4.tar.gz` & `tmp/redis_hashring-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redis-hashring-0.3.4.tar", last modified: Tue Feb 20 07:38:27 2024, max compression
+gzip compressed data, was "redis_hashring-0.4.0.tar", last modified: Fri May 10 15:01:47 2024, max compression
```

## Comparing `redis-hashring-0.3.4.tar` & `redis_hashring-0.4.0.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxr-xr-x   0 jpmelos    (501) staff       (20)        0 2024-02-20 07:38:27.774886 redis-hashring-0.3.4/
--rw-r--r--   0 jpmelos    (501) staff       (20)     1089 2024-02-19 10:33:28.000000 redis-hashring-0.3.4/LICENSE
--rw-r--r--   0 jpmelos    (501) staff       (20)      837 2024-02-20 07:38:27.774714 redis-hashring-0.3.4/PKG-INFO
--rw-r--r--   0 jpmelos    (501) staff       (20)     9992 2024-02-19 10:33:28.000000 redis-hashring-0.3.4/README.rst
-drwxr-xr-x   0 jpmelos    (501) staff       (20)        0 2024-02-20 07:38:27.773586 redis-hashring-0.3.4/redis_hashring/
--rw-r--r--   0 jpmelos    (501) staff       (20)    12753 2024-02-19 18:17:20.000000 redis-hashring-0.3.4/redis_hashring/__init__.py
-drwxr-xr-x   0 jpmelos    (501) staff       (20)        0 2024-02-20 07:38:27.774547 redis-hashring-0.3.4/redis_hashring.egg-info/
--rw-r--r--   0 jpmelos    (501) staff       (20)      837 2024-02-20 07:38:27.000000 redis-hashring-0.3.4/redis_hashring.egg-info/PKG-INFO
--rw-r--r--   0 jpmelos    (501) staff       (20)      243 2024-02-20 07:38:27.000000 redis-hashring-0.3.4/redis_hashring.egg-info/SOURCES.txt
--rw-r--r--   0 jpmelos    (501) staff       (20)        1 2024-02-20 07:38:27.000000 redis-hashring-0.3.4/redis_hashring.egg-info/dependency_links.txt
--rw-r--r--   0 jpmelos    (501) staff       (20)       12 2024-02-20 07:38:27.000000 redis-hashring-0.3.4/redis_hashring.egg-info/requires.txt
--rw-r--r--   0 jpmelos    (501) staff       (20)       15 2024-02-20 07:38:27.000000 redis-hashring-0.3.4/redis_hashring.egg-info/top_level.txt
--rw-r--r--   0 jpmelos    (501) staff       (20)       38 2024-02-20 07:38:27.774919 redis-hashring-0.3.4/setup.cfg
--rw-r--r--   0 jpmelos    (501) staff       (20)      969 2024-02-20 07:37:03.000000 redis-hashring-0.3.4/setup.py
+drwxr-xr-x   0 jpmelos    (501) staff       (20)        0 2024-05-10 15:01:47.595848 redis_hashring-0.4.0/
+-rw-r--r--   0 jpmelos    (501) staff       (20)     1091 2024-05-10 09:49:50.000000 redis_hashring-0.4.0/LICENSE
+-rw-r--r--   0 jpmelos    (501) staff       (20)      938 2024-05-10 15:01:47.595600 redis_hashring-0.4.0/PKG-INFO
+-rw-r--r--   0 jpmelos    (501) staff       (20)     9992 2024-02-19 10:33:28.000000 redis_hashring-0.4.0/README.rst
+-rw-r--r--   0 jpmelos    (501) staff       (20)     1197 2024-05-10 09:53:40.000000 redis_hashring-0.4.0/pyproject.toml
+drwxr-xr-x   0 jpmelos    (501) staff       (20)        0 2024-05-10 15:01:47.594425 redis_hashring-0.4.0/redis_hashring/
+-rw-r--r--   0 jpmelos    (501) staff       (20)    13110 2024-05-10 10:05:36.000000 redis_hashring-0.4.0/redis_hashring/__init__.py
+drwxr-xr-x   0 jpmelos    (501) staff       (20)        0 2024-05-10 15:01:47.595367 redis_hashring-0.4.0/redis_hashring.egg-info/
+-rw-r--r--   0 jpmelos    (501) staff       (20)      938 2024-05-10 15:01:47.000000 redis_hashring-0.4.0/redis_hashring.egg-info/PKG-INFO
+-rw-r--r--   0 jpmelos    (501) staff       (20)      258 2024-05-10 15:01:47.000000 redis_hashring-0.4.0/redis_hashring.egg-info/SOURCES.txt
+-rw-r--r--   0 jpmelos    (501) staff       (20)        1 2024-05-10 15:01:47.000000 redis_hashring-0.4.0/redis_hashring.egg-info/dependency_links.txt
+-rw-r--r--   0 jpmelos    (501) staff       (20)        9 2024-05-10 15:01:47.000000 redis_hashring-0.4.0/redis_hashring.egg-info/requires.txt
+-rw-r--r--   0 jpmelos    (501) staff       (20)       15 2024-05-10 15:01:47.000000 redis_hashring-0.4.0/redis_hashring.egg-info/top_level.txt
+-rw-r--r--   0 jpmelos    (501) staff       (20)       38 2024-05-10 15:01:47.595898 redis_hashring-0.4.0/setup.cfg
+-rw-r--r--   0 jpmelos    (501) staff       (20)     1053 2024-05-10 14:59:55.000000 redis_hashring-0.4.0/setup.py
```

### Comparing `redis-hashring-0.3.4/LICENSE` & `redis_hashring-0.4.0/LICENSE`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 The MIT License (MIT)
 
-Copyright (c) 2015 Elastic Inc. (Close.io)
+Copyright (c) 2015-2024 Elastic Inc. (Close)
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `redis-hashring-0.3.4/PKG-INFO` & `redis_hashring-0.4.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 Metadata-Version: 2.1
 Name: redis-hashring
-Version: 0.3.4
+Version: 0.4.0
 Summary: Python library for distributed applications using a Redis hash ring
-Home-page: http://github.com/closeio/redis-hashring
+Home-page: https://github.com/closeio/redis-hashring
 Author: Close Engineering
 Author-email: engineering@close.com
 License: MIT
 Platform: any
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 License-File: LICENSE
-Requires-Dist: redis<5,>=3
+Requires-Dist: redis>=3
```

### Comparing `redis-hashring-0.3.4/README.rst` & `redis_hashring-0.4.0/README.rst`

 * *Files identical despite different names*

### Comparing `redis-hashring-0.3.4/redis_hashring/__init__.py` & `redis_hashring-0.4.0/redis_hashring/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,355 +1,379 @@
 import binascii
 import collections
-import socket
-import time
-import random
 import operator
 import os
+import random
 import select
+import socket
 import threading
+import time
 
 # Amount of points on the ring. Must not be higher than 2**32 because we're
 # using CRC32 to compute the checksum.
-RING_SIZE = 2 ** 32
+RING_SIZE = 2**32
 
-# Default amount of replicas per node
+# Default amount of replicas per node.
 RING_REPLICAS = 16
 
-# How often to update a node's heartbeat
+# How often to update a node's heartbeat.
 POLL_INTERVAL = 10
 
-# After how much time a node is considered to be dead
+# After how much time a node is considered to be dead.
 NODE_TIMEOUT = 60
 
-# How often expired nodes are cleaned up from the ring
+# How often expired nodes are cleaned up from the ring.
 CLEANUP_INTERVAL = 120
 
 
 def _decode(data):
-    # Compatibility with different redis-py decode_responses settings
+    # Compatibility with different redis-py `decode_responses` settings.
     if isinstance(data, bytes):
         return data.decode()
     else:
         return data
 
 
 class RingNode(object):
     """
-    Represents a node in a Redis hash ring. Each node may have multiple
-    replicas on the ring for more balanced hashing.
+    A node in a Redis hash ring.
+
+    Each node may have multiple replicas on the ring for more balanced hashing.
 
     The ring is stored as follows in Redis:
 
     ZSET <key>
     Represents the ring in Redis. The keys of this ZSET represent
-    "start:replica_name", where start is the start of the range for which
-    the replica is responsible.
+    "start:replica_name", where start is the start of the range for which the
+    replica is responsible.
 
     CHANNEL <key>
-    Represents a pubsub channel in Redis which receives a message every
-    time the ring structure has changed.
+    Represents a pubsub channel in Redis which receives a message every time
+    the ring structure has changed.
 
     Simple usage example for a distributed threads-based application:
 
     ```
     node = RingNode(redis, key)
     node.start()
 
     while is_running:
-        # Only process items this node is responsible for.
+        # Only process items this node is responsible for. `item` should be an
+        # object that can be encoded to bytes by calling `item.encode()` on it,
+        # like a `str`.
         items = [item for item in get_items() if node.contains(item)]
         process_items(items)
 
     node.stop()
     ```
 
     Simple usage example for a distributed gevent-based application:
 
     ```
     node = RingNode(redis, key)
     node.gevent_start()
 
     while is_running:
-        # Only process items this node is responsible for.
+        # Only process items this node is responsible for. `item` should be an
+        # object that can be encoded to bytes by calling `item.encode()` on it,
+        # like a `str`.
         items = [item for item in get_items() if node.contains(item)]
         process_items(items)
 
     node.gevent_stop()
     ```
     """
 
     def __init__(self, conn, key, n_replicas=RING_REPLICAS):
         """
-        Initializes a Redis hash ring node, given the Redis connection, a key
-        and the number of replicas.
+        Initializes a Redis hash ring node.
+
+        Args:
+            conn: The Redis connection to use.
+            key: A key to use for this node.
+            n_replicas: Number of replicas this node should have on the ring.
         """
         self._polling_thread = None
         self._polling_greenlet = None
         self._stop_polling_fd_r = None
         self._stop_polling_fd_w = None
 
-        self.conn = conn
-        self.key = key
-
+        self._conn = conn
+        self._key = key
         host = socket.gethostname()
         pid = os.getpid()
-        # Create unique identifiers for the replicas
-        self.replicas = [
+
+        # Create unique identifiers for the replicas.
+        self._replicas = [
             (
-                random.randrange(2 ** 32),
-                '{host}:{pid}:{rand}'.format(
-                    host=host, pid=pid, rand=binascii.hexlify(os.urandom(4)).decode()
+                random.randrange(2**32),
+                "{host}:{pid}:{id_}".format(
+                    host=host,
+                    pid=pid,
+                    id_=binascii.hexlify(os.urandom(4)).decode(),
                 ),
             )
-            for n in range(n_replicas)
+            for _ in range(n_replicas)
         ]
 
+        # Number of nodes currently active in the ring.
+        self._node_count = 0
         # List of tuples of ranges this node is responsible for, where a tuple
         # (a, b) includes any N matching a <= N < b.
-        self.ranges = []
+        self._ranges = []
 
         self._select = select.select
 
-    def _fetch(self):
-        """
-        Internal helper that fetches the ring from Redis, including only active
-        nodes/replicas. Returns a list of tuples (start, replica) (see
-        _fetch_all docs for more details).
+    def _fetch_ring(self):
         """
-        now = time.time()
-        expiry_time = now - NODE_TIMEOUT
+        Fetch the ring from Redis.
 
-        data = self.conn.zrangebyscore(self.key, expiry_time, 'INF')
+        The fetched ring only includes active nodes. Returns a list of tuples
+        (start, replica) (see _fetch_all docs for more details).
+        """
+        expiry_time = time.time() - NODE_TIMEOUT
+        data = self._conn.zrangebyscore(self._key, expiry_time, "INF")
 
         ring = []
-
-        for node_data in data:
-            start, replica = _decode(node_data).split(':', 1)
+        for replica_data in data:
+            start, replica = _decode(replica_data).split(":", 1)
             ring.append((int(start), replica))
+        return sorted(ring, key=operator.itemgetter(0))
 
-        ring = sorted(ring, key=operator.itemgetter(0))
-
-        return ring
-
-    def _fetch_all(self):
+    def _fetch_ring_all(self):
         """
-        Internal helper that fetches the ring from Redis, including any
-        inactive nodes/replicas. Returns a list of tuples (start, replica,
-        heartbeat, expired), where
-        * start: start of the range for which the replica is responsible
-        * replica: name of the replica
-        * heartbeat: unix time stamp of the last heartbeat
-        * expired: boolean denoting whether this replica is inactive
-        """
-        now = time.time()
-        expiry_time = now - NODE_TIMEOUT
+        Fetch the ring from Redis.
 
-        data = self.conn.zrange(self.key, 0, -1, withscores=True)
+        The fetched ring will include inactive nodes. Returns a list of tuples
+        (start, replica, heartbeat, expired), where:
+        * start: start of the range for which the replica is responsible.
+        * replica: name of the replica.
+        * heartbeat: timestamp of the last heartbeat.
+        * expired: boolean denoting whether this replica is inactive.
+        """
+        expiry_time = time.time() - NODE_TIMEOUT
+        data = self._conn.zrange(self._key, 0, -1, withscores=True)
 
         ring = []
-
-        for node_data, heartbeat in data:
-            start, replica = _decode(node_data).split(':', 1)
-            ring.append((int(start), replica, heartbeat, heartbeat < expiry_time))
-
-        ring = sorted(ring, key=operator.itemgetter(0))
-
-        return ring
+        for replica_data, heartbeat in data:
+            start, replica = _decode(replica_data).split(":", 1)
+            ring.append(
+                (int(start), replica, heartbeat, heartbeat < expiry_time)
+            )
+        return sorted(ring, key=operator.itemgetter(0))
 
     def debug_print(self):
         """
         Prints the ring for debugging purposes.
         """
-        ring = self._fetch_all()
+        ring = self._fetch_ring_all()
 
-        print('Hash ring "{key}" replicas:'.format(key=self.key))
+        print('Hash ring "{key}" replicas:'.format(key=self._key))
 
         now = time.time()
+
         n_replicas = len(ring)
         if ring:
-            print('{:10} {:6} {:7} {}'.format('Start', 'Range', 'Delay', 'Node'))
+            print(
+                "{:10} {:6} {:7} {}".format("Start", "Range", "Delay", "Node")
+            )
         else:
-            print('(no replicas)')
+            print("(no replicas)")
 
         nodes = collections.defaultdict(list)
 
         for n, (start, replica, heartbeat, expired) in enumerate(ring):
-            hostname, pid, rnd = replica.split(':')
-            node = ':'.join([hostname, pid])
+            hostname, pid, _ = replica.split(":")
+            node = ":".join([hostname, pid])
 
             abs_size = (ring[(n + 1) % n_replicas][0] - ring[n][0]) % RING_SIZE
             size = 100.0 / RING_SIZE * abs_size
             delay = int(now - heartbeat)
+            expired_str = "(EXPIRED)" if expired else ""
 
             nodes[node].append((hostname, pid, abs_size, delay, expired))
 
             print(
-                '{start:10} {size:5.2f}% {delay:6}s {replica}{extra}'.format(
-                    start=start,
-                    replica=replica,
-                    delay=delay,
-                    size=size,
-                    extra=' (EXPIRED)' if expired else '',
-                )
+                f"{start:10} {size:5.2f}% {delay:6}s {replica} {expired_str}"
             )
 
         print()
-        print('Hash ring "{key}" nodes:'.format(key=self.key))
+        print('Hash ring "{key}" nodes:'.format(key=self._key))
 
         if nodes:
             print(
-                '{:8} {:8} {:7} {:20} {:5}'.format(
-                    'Range', 'Replicas', 'Delay', 'Hostname', 'PID'
+                "{:8} {:8} {:7} {:20} {:5}".format(
+                    "Range", "Replicas", "Delay", "Hostname", "PID"
                 )
             )
         else:
-            print('(no nodes)')
+            print("(no nodes)")
 
-        for k, v in nodes.items():
+        for _, v in nodes.items():
             hostname, pid = v[0][0], v[0][1]
             abs_size = sum(replica[2] for replica in v)
             size = 100.0 / RING_SIZE * abs_size
             delay = max(replica[3] for replica in v)
             expired = any(replica[4] for replica in v)
             count = len(v)
+            expired_str = "(EXPIRED)" if expired else ""
             print(
-                '{size:5.2f}% {count:8} {delay:6}s {hostname:20} {pid:5}{extra}'.format(
-                    start=start,
-                    count=count,
-                    hostname=hostname,
-                    pid=pid,
-                    delay=delay,
-                    size=size,
-                    extra=' (EXPIRED)' if expired else '',
-                )
+                f"{size:5.2f}% {count:8} {delay:6}s {hostname:20} {pid:5}"
+                f" {expired_str}"
             )
 
     def heartbeat(self):
         """
-        Add/update the node in Redis. Needs to be called regularly by the
-        client.
+        Add/update the node in Redis.
+
+        Needs to be called regularly by the node.
         """
-        pipeline = self.conn.pipeline()
+        pipeline = self._conn.pipeline()
+
         now = time.time()
-        for replica in self.replicas:
-            pipeline.zadd(
-                self.key,
-                {
-                    '{start}:{name}'.format(start=replica[0], name=replica[1]): now,
-                },
-            )
+
+        for replica in self._replicas:
+            pipeline.zadd(self._key, {f"{replica[0]}:{replica[1]}": now})
         ret = pipeline.execute()
 
         # Only notify the other nodes if we're not in the ring yet.
         if any(ret):
             self._notify()
 
     def remove(self):
         """
-        Call this to remove the node/replicas from the ring.
+        Remove the node from the ring.
         """
-        pipeline = self.conn.pipeline()
-        for replica in self.replicas:
-            pipeline.zrem(
-                self.key, '{start}:{name}'.format(start=replica[0], name=replica[1])
-            )
+        pipeline = self._conn.pipeline()
+
+        for replica in self._replicas:
+            pipeline.zrem(self._key, f"{replica[0]}:{replica[1]}")
         pipeline.execute()
+
+        # Make sure this node won't contain any items.
+        self._node_count = 0
+        self._ranges = []
+
         self._notify()
 
     def _notify(self):
         """
-        Internal helper method which publishes an update to the ring's
-        activity channel.
+        Publish an update to the ring's activity channel.
         """
-        # Publish a dummy message on the activity channel
-        self.conn.publish(self.key, '*')
+        self._conn.publish(self._key, "*")
 
     def cleanup(self):
         """
-        Removes expired nodes/replicas from the ring.
+        Removes expired nodes from the ring.
         """
-        now = time.time()
-        expired = now - NODE_TIMEOUT
-        if self.conn.zremrangebyscore(self.key, 0, expired):
+        expired = time.time() - NODE_TIMEOUT
+
+        if self._conn.zremrangebyscore(self._key, 0, expired):
             self._notify()
 
     def update(self):
         """
         Fetches the updated ring from Redis and updates the current ranges.
         """
-        ring = self._fetch()
+        ring = self._fetch_ring()
+        nodes = set()
         n_replicas = len(ring)
-        replica_set = set([r[1] for r in self.replicas])
-        self.ranges = []
+
+        own_replicas = {r[1] for r in self._replicas}
+
+        self._ranges = []
         for n, (start, replica) in enumerate(ring):
-            if replica in replica_set:
+            host, pid, _ = replica.split(":")
+            node = ":".join([host, pid])
+            nodes.add(node)
+
+            if replica in own_replicas:
                 end = ring[(n + 1) % n_replicas][0] % RING_SIZE
                 if start < end:
-                    self.ranges.append((start, end))
+                    self._ranges.append((start, end))
                 elif end < start:
-                    self.ranges.append((start, RING_SIZE))
-                    self.ranges.append((0, end))
+                    self._ranges.append((start, RING_SIZE))
+                    self._ranges.append((0, end))
                 else:
-                    self.ranges.append((0, RING_SIZE))
+                    self._ranges.append((0, RING_SIZE))
+
+        self._node_count = len(nodes)
+
+    def get_ranges(self):
+        """
+        Return the hash ring ranges that this node owns.
+        """
+        return self._ranges
+
+    def get_node_count(self):
+        """
+        Return the number of active nodes in the ring.
+        """
+        return self._node_count
 
     def contains(self, key):
         """
-        Returns a boolean indicating if this node is responsible for handling
-        the given key.
+        Check whether this node is responsible for the item.
         """
-        return self.contains_ring_point(self.key_as_ring_point(key))
+        return self._contains_ring_point(self.key_as_ring_point(key))
 
     def key_as_ring_point(self, key):
         """Turn a key into a point on a hash ring."""
         return binascii.crc32(key.encode()) % RING_SIZE
 
-    def contains_ring_point(self, n):
+    def _contains_ring_point(self, n):
         """
-        Returns a boolean indicating if this node is responsible for handling
-        the given point on a hash ring.
+        Check whether this node is responsible for the ring point.
         """
-        for start, end in self.ranges:
+        for start, end in self._ranges:
             if start <= n < end:
                 return True
         return False
 
     def poll(self):
         """
-        Main loop which maintains the node in the hash ring. Can be run in a
-        greenlet or separate thread. This takes care of:
+        Keep a node in the hash ring.
 
-        * Updating the heartbeat
-        * Checking for ring updates
-        * Cleaning up expired nodes periodically
-        """
-        pubsub = self.conn.pubsub()
-        pubsub.subscribe(self.key)
+        This should be kept running for as long as the node needs to stay in
+        the ring. Can be run in a separate thread or in a greenlet. This takes
+        care of:
+        * Updating the heartbeat.
+        * Checking for ring updates.
+        * Cleaning up expired nodes periodically.
+        """
+        pubsub = self._conn.pubsub()
+        pubsub.subscribe(self._key)
+        pubsub_fd = pubsub.connection._sock.fileno()
 
         last_heartbeat = time.time()
         self.heartbeat()
 
         last_cleanup = time.time()
         self.cleanup()
 
         self._stop_polling_fd_r, self._stop_polling_fd_w = os.pipe()
 
         try:
             while True:
-                # Since Redis' listen method blocks, we use select to inspect the
-                # underlying socket to see if there is activity.
-                pubsub_fd = pubsub.connection._sock.fileno()
-                timeout = max(0, POLL_INTERVAL - (time.time() - last_heartbeat))
-                r, w, x = self._select([self._stop_polling_fd_r, pubsub_fd], [], [], timeout)
+                # Since Redis' `listen` method blocks, we use `select` to
+                # inspect the underlying socket to see if there is activity.
+                timeout = max(
+                    0.0, POLL_INTERVAL - (time.time() - last_heartbeat)
+                )
+                r, _, _ = self._select(
+                    [self._stop_polling_fd_r, pubsub_fd], [], [], timeout
+                )
+
                 if self._stop_polling_fd_r in r:
                     os.close(self._stop_polling_fd_r)
                     os.close(self._stop_polling_fd_w)
                     self._stop_polling_fd_r = None
                     self._stop_polling_fd_w = None
                     break
+
                 if pubsub_fd in r:
                     while pubsub.get_message():
                         pass
                     self.update()
 
                 last_heartbeat = time.time()
                 self.heartbeat()
@@ -359,52 +383,50 @@
                     last_cleanup = now
                     self.cleanup()
         finally:
             pubsub.close()
 
     def start(self):
         """
-        Helper method to start the node for threads-based applications.
+        Start the node for threads-based applications.
         """
         self._polling_thread = threading.Thread(target=self.poll, daemon=True)
         self._polling_thread.start()
 
     def stop(self):
         """
-        Helper method to stop the node for threads-based applications.
+        Stop the node for threads-based applications.
         """
         if self._polling_thread:
             while not self._stop_polling_fd_w:
                 # Let's give the thread some time to create the fd.
                 time.sleep(0.1)
-            os.write(self._stop_polling_fd_w, b'1')
+            os.write(self._stop_polling_fd_w, b"1")
             self._polling_thread.join()
             self._polling_thread = None
         self.remove()
 
     def gevent_start(self):
         """
-        Helper method to start the node for gevent-based applications.
+        Start the node for gevent-based applications.
         """
         import gevent
         import gevent.select
 
         self._select = gevent.select.select
         self._polling_greenlet = gevent.spawn(self.poll)
         self.heartbeat()
         self.update()
 
     def gevent_stop(self):
         """
-        Helper method to stop the node for gevent-based applications.
+        Stop the node for gevent-based applications.
         """
-        import gevent
-
         if self._polling_greenlet:
             while not self._stop_polling_fd_w:
                 # Let's give the greenlet some time to create the fd.
                 time.sleep(0.1)
-            os.write(self._stop_polling_fd_w, b'1')
+            os.write(self._stop_polling_fd_w, b"1")
             self._polling_greenlet.join()
             self._polling_greenlet = None
         self.remove()
         self._select = select.select
```

### Comparing `redis-hashring-0.3.4/redis_hashring.egg-info/PKG-INFO` & `redis_hashring-0.4.0/redis_hashring.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 Metadata-Version: 2.1
 Name: redis-hashring
-Version: 0.3.4
+Version: 0.4.0
 Summary: Python library for distributed applications using a Redis hash ring
-Home-page: http://github.com/closeio/redis-hashring
+Home-page: https://github.com/closeio/redis-hashring
 Author: Close Engineering
 Author-email: engineering@close.com
 License: MIT
 Platform: any
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 License-File: LICENSE
-Requires-Dist: redis<5,>=3
+Requires-Dist: redis>=3
```

