# Comparing `tmp/lavalink-5.3.0.tar.gz` & `tmp/lavalink-5.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lavalink-5.3.0.tar", last modified: Fri Mar  8 20:15:22 2024, max compression
+gzip compressed data, was "lavalink-5.4.0.tar", last modified: Fri May 10 21:36:44 2024, max compression
```

## Comparing `lavalink-5.3.0.tar` & `lavalink-5.4.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxrwx   0        0        0        0 2024-03-08 20:15:22.366772 lavalink-5.3.0/
--rw-rw-rw-   0        0        0     1093 2022-08-21 12:42:47.000000 lavalink-5.3.0/LICENSE
--rw-rw-rw-   0        0        0      419 2024-03-08 20:15:22.365770 lavalink-5.3.0/PKG-INFO
--rw-rw-rw-   0        0        0     4148 2023-12-08 20:14:28.000000 lavalink-5.3.0/README.md
-drwxrwxrwx   0        0        0        0 2024-03-08 20:15:22.358770 lavalink-5.3.0/lavalink/
--rw-rw-rw-   0        0        0     2540 2024-03-08 20:15:17.000000 lavalink-5.3.0/lavalink/__init__.py
--rw-rw-rw-   0        0        0    15707 2024-02-17 14:22:46.000000 lavalink-5.3.0/lavalink/__main__.py
--rw-rw-rw-   0        0        0    14172 2024-03-08 20:15:17.000000 lavalink-5.3.0/lavalink/abc.py
--rw-rw-rw-   0        0        0    18488 2024-03-08 20:15:17.000000 lavalink-5.3.0/lavalink/client.py
--rw-rw-rw-   0        0        0     1254 2024-02-17 14:22:46.000000 lavalink-5.3.0/lavalink/common.py
--rw-rw-rw-   0        0        0     4224 2024-03-08 20:15:17.000000 lavalink-5.3.0/lavalink/dataio.py
--rw-rw-rw-   0        0        0     2886 2024-02-17 14:22:46.000000 lavalink-5.3.0/lavalink/errors.py
--rw-rw-rw-   0        0        0    12258 2024-02-28 16:18:32.000000 lavalink-5.3.0/lavalink/events.py
--rw-rw-rw-   0        0        0    18738 2024-03-08 20:15:17.000000 lavalink-5.3.0/lavalink/filters.py
--rw-rw-rw-   0        0        0    24225 2024-02-17 14:22:46.000000 lavalink-5.3.0/lavalink/node.py
--rw-rw-rw-   0        0        0    10207 2024-02-17 14:22:46.000000 lavalink-5.3.0/lavalink/nodemanager.py
--rw-rw-rw-   0        0        0    24124 2024-03-08 20:15:17.000000 lavalink-5.3.0/lavalink/player.py
--rw-rw-rw-   0        0        0     9157 2024-03-08 20:15:17.000000 lavalink-5.3.0/lavalink/playermanager.py
--rw-rw-rw-   0        0        0    13509 2024-03-08 20:15:17.000000 lavalink-5.3.0/lavalink/server.py
--rw-rw-rw-   0        0        0     2293 2024-03-08 20:15:17.000000 lavalink-5.3.0/lavalink/source_decoders.py
--rw-rw-rw-   0        0        0     6296 2023-12-08 20:14:28.000000 lavalink-5.3.0/lavalink/stats.py
--rw-rw-rw-   0        0        0    16312 2024-03-08 20:15:17.000000 lavalink-5.3.0/lavalink/transport.py
--rw-rw-rw-   0        0        0     2852 2024-02-17 14:22:46.000000 lavalink-5.3.0/lavalink/utfm_codec.py
--rw-rw-rw-   0        0        0     9918 2024-03-08 20:15:17.000000 lavalink-5.3.0/lavalink/utils.py
-drwxrwxrwx   0        0        0        0 2024-03-08 20:15:22.364771 lavalink-5.3.0/lavalink.egg-info/
--rw-rw-rw-   0        0        0      419 2024-03-08 20:15:22.000000 lavalink-5.3.0/lavalink.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      607 2024-03-08 20:15:22.000000 lavalink-5.3.0/lavalink.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-08 20:15:22.000000 lavalink-5.3.0/lavalink.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2024-03-08 20:15:22.000000 lavalink-5.3.0/lavalink.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      121 2024-03-08 20:15:22.000000 lavalink-5.3.0/lavalink.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-03-08 20:15:22.000000 lavalink-5.3.0/lavalink.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-03-08 20:15:22.366772 lavalink-5.3.0/setup.cfg
--rw-rw-rw-   0        0        0     1196 2023-12-16 16:52:11.000000 lavalink-5.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-10 21:36:44.224819 lavalink-5.4.0/
+-rw-rw-rw-   0        0        0     1093 2022-08-21 12:42:47.000000 lavalink-5.4.0/LICENSE
+-rw-rw-rw-   0        0        0      419 2024-05-10 21:36:44.223819 lavalink-5.4.0/PKG-INFO
+-rw-rw-rw-   0        0        0     4148 2023-12-08 20:14:28.000000 lavalink-5.4.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-10 21:36:44.216825 lavalink-5.4.0/lavalink/
+-rw-rw-rw-   0        0        0     2540 2024-03-28 21:25:38.000000 lavalink-5.4.0/lavalink/__init__.py
+-rw-rw-rw-   0        0        0    15707 2024-02-17 14:22:46.000000 lavalink-5.4.0/lavalink/__main__.py
+-rw-rw-rw-   0        0        0    14401 2024-03-20 22:19:57.000000 lavalink-5.4.0/lavalink/abc.py
+-rw-rw-rw-   0        0        0    18761 2024-03-28 21:33:24.000000 lavalink-5.4.0/lavalink/client.py
+-rw-rw-rw-   0        0        0     1254 2024-02-17 14:22:46.000000 lavalink-5.4.0/lavalink/common.py
+-rw-rw-rw-   0        0        0     7374 2024-03-20 22:12:23.000000 lavalink-5.4.0/lavalink/dataio.py
+-rw-rw-rw-   0        0        0     2886 2024-02-17 14:22:46.000000 lavalink-5.4.0/lavalink/errors.py
+-rw-rw-rw-   0        0        0    13042 2024-03-20 22:18:16.000000 lavalink-5.4.0/lavalink/events.py
+-rw-rw-rw-   0        0        0    18738 2024-03-08 20:15:17.000000 lavalink-5.4.0/lavalink/filters.py
+-rw-rw-rw-   0        0        0    25136 2024-05-10 21:36:40.000000 lavalink-5.4.0/lavalink/node.py
+-rw-rw-rw-   0        0        0    10226 2024-03-28 21:32:58.000000 lavalink-5.4.0/lavalink/nodemanager.py
+-rw-rw-rw-   0        0        0    24801 2024-03-28 21:25:39.000000 lavalink-5.4.0/lavalink/player.py
+-rw-rw-rw-   0        0        0     9077 2024-03-20 22:12:23.000000 lavalink-5.4.0/lavalink/playermanager.py
+-rw-rw-rw-   0        0        0    13509 2024-03-08 20:15:17.000000 lavalink-5.4.0/lavalink/server.py
+-rw-rw-rw-   0        0        0     2293 2024-03-08 20:15:17.000000 lavalink-5.4.0/lavalink/source_decoders.py
+-rw-rw-rw-   0        0        0     6296 2023-12-08 20:14:28.000000 lavalink-5.4.0/lavalink/stats.py
+-rw-rw-rw-   0        0        0    16817 2024-05-10 21:36:40.000000 lavalink-5.4.0/lavalink/transport.py
+-rw-rw-rw-   0        0        0     2852 2024-02-17 14:22:46.000000 lavalink-5.4.0/lavalink/utfm_codec.py
+-rw-rw-rw-   0        0        0    11040 2024-03-28 21:25:38.000000 lavalink-5.4.0/lavalink/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-10 21:36:44.222818 lavalink-5.4.0/lavalink.egg-info/
+-rw-rw-rw-   0        0        0      419 2024-05-10 21:36:44.000000 lavalink-5.4.0/lavalink.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      607 2024-05-10 21:36:44.000000 lavalink-5.4.0/lavalink.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-10 21:36:44.000000 lavalink-5.4.0/lavalink.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2024-05-10 21:36:44.000000 lavalink-5.4.0/lavalink.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      121 2024-05-10 21:36:44.000000 lavalink-5.4.0/lavalink.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-05-10 21:36:44.000000 lavalink-5.4.0/lavalink.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-10 21:36:44.224819 lavalink-5.4.0/setup.cfg
+-rw-rw-rw-   0        0        0     1196 2023-12-16 16:52:11.000000 lavalink-5.4.0/setup.py
```

### Comparing `lavalink-5.3.0/LICENSE` & `lavalink-5.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lavalink-5.3.0/README.md` & `lavalink-5.4.0/README.md`

 * *Files identical despite different names*

### Comparing `lavalink-5.3.0/lavalink/__init__.py` & `lavalink-5.4.0/lavalink/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # flake8: noqa
 
 __title__ = 'Lavalink'
 __author__ = 'Devoxin'
 __license__ = 'MIT'
 __copyright__ = 'Copyright 2017-present Devoxin'
-__version__ = '5.3.0'
+__version__ = '5.4.0'
 
 
 from typing import Type
 
 from .abc import BasePlayer, DeferredAudioTrack, Source
 from .client import Client
 from .dataio import DataReader, DataWriter
```

### Comparing `lavalink-5.3.0/lavalink/__main__.py` & `lavalink-5.4.0/lavalink/__main__.py`

 * *Files identical despite different names*

### Comparing `lavalink-5.3.0/lavalink/abc.py` & `lavalink-5.4.0/lavalink/abc.py`

 * *Files 1% similar despite different names*

```diff
@@ -109,14 +109,19 @@
                          **kwargs) -> Optional[Dict[str, Any]]:
         """|coro|
 
         .. _player object: https://lavalink.dev/api/rest.html#Player
 
         Plays the given track.
 
+        Warning
+        -------
+        Multiple calls to this method within a short timeframe could cause issues with the player's
+        internal state, which can cause errors when processing a :class:`TrackStartEvent`.
+
         Parameters
         ----------
         track: Union[:class:`AudioTrack`, :class:`DeferredAudioTrack`]
             The track to play.
         start_time: :class:`int`
             The number of milliseconds to offset the track by.
             If left unspecified or ``None`` is provided, the track will start from the beginning.
```

### Comparing `lavalink-5.3.0/lavalink/client.py` & `lavalink-5.4.0/lavalink/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -261,15 +261,15 @@
         Optional[:class:`Source`]
             The source with the matching name. May be ``None`` if
             the name didn't match any of those in the registered sources.
         """
         return next((source for source in self.sources if source.name == source_name), None)
 
     def add_node(self, host: str, port: int, password: str, region: str, name: Optional[str] = None,
-                 ssl: bool = False, session_id: Optional[str] = None) -> Node:
+                 ssl: bool = False, session_id: Optional[str] = None, connect: bool = True) -> Node:
         """
         Shortcut for :func:`NodeManager.add_node`.
 
         Adds a node to Lavalink's node manager.
 
         Parameters
         ----------
@@ -279,28 +279,32 @@
             The port to use for websocket and REST connections.
         password: :class:`str`
             The password used for authentication.
         region: :class:`str`
             The region to assign this node to.
         name: Optional[:class:`str`]
             An identifier for the node that will show in logs. Defaults to ``None``.
-        ssl: Optional[:class:`bool`]
+        ssl: :class:`bool`
             Whether to use SSL for the node. SSL will use ``wss`` and ``https``, instead of ``ws`` and ``http``,
             respectively. Your node should support SSL if you intend to enable this, either via reverse proxy or
             other methods. Only enable this if you know what you're doing.
         session_id: Optional[:class:`str`]
             The ID of the session to resume. Defaults to ``None``.
             Only specify this if you have the ID of the session you want to resume.
+        connect: :class:`bool`
+            Whether to immediately connect to the node after creating it.
+            If ``False``, you must call :func:`Node.connect` if you require WebSocket functionality.
 
         Returns
         -------
         :class:`Node`
             The created Node instance.
         """
-        return self.node_manager.add_node(host, port, password, region, name, ssl, session_id)
+        return self.node_manager.add_node(host, port, password, region, name, ssl,
+                                          session_id, connect)
 
     async def get_local_tracks(self, query: str) -> LoadResult:
         """|coro|
 
         Searches :attr:`sources` registered to this client for the given query.
 
         Parameters
```

### Comparing `lavalink-5.3.0/lavalink/common.py` & `lavalink-5.4.0/lavalink/common.py`

 * *Files identical despite different names*

### Comparing `lavalink-5.3.0/lavalink/errors.py` & `lavalink-5.4.0/lavalink/errors.py`

 * *Files identical despite different names*

### Comparing `lavalink-5.3.0/lavalink/events.py` & `lavalink-5.4.0/lavalink/events.py`

 * *Files 3% similar despite different names*

```diff
@@ -54,14 +54,19 @@
 
 
 class TrackStuckEvent(Event):
     """
     This event is emitted when the currently playing track is stuck (i.e. has not provided any audio).
     This is typically a fault of the track's underlying audio stream, and not Lavalink itself.
 
+    Note
+    ----
+    You do not need to manually trigger the start of the next track in the queue within
+    this event when using the :class:`DefaultPlayer`. This is handled for you.
+
     Attributes
     ----------
     player: :class:`BasePlayer`
         The player associated with the stuck track.
     track: :class:`AudioTrack`
         The stuck track.
     threshold: :class:`int`
@@ -76,14 +81,19 @@
         self.threshold: int = threshold
 
 
 class TrackExceptionEvent(Event):
     """
     This event is emitted when a track encounters an exception during playback.
 
+    Note
+    ----
+    You do not need to manually trigger the start of the next track in the queue within
+    this event when using the :class:`DefaultPlayer`. This is handled for you.
+
     Attributes
     ----------
     player: :class:`BasePlayer`
         The player that had the exception occur while playing a track.
     track: :class:`AudioTrack`
         The track that had the exception while playing.
     message: Optional[:class:`str`]
@@ -104,14 +114,19 @@
         self.cause: str = cause
 
 
 class TrackEndEvent(Event):
     """
     This event is emitted when the player finished playing a track.
 
+    Note
+    ----
+    You do not need to manually trigger the start of the next track in the queue within
+    this event when using the :class:`DefaultPlayer`. This is handled for you.
+
     Attributes
     ----------
     player: :class:`BasePlayer`
         The player that finished playing a track.
     track: Optional[:class:`AudioTrack`]
         The track that finished playing.
         This could be ``None`` if Lavalink fails to encode the track.
@@ -128,14 +143,19 @@
 
 class TrackLoadFailedEvent(Event):
     """
     This is a custom event, emitted when a deferred audio track fails to
     produce a playable track. The player will not do anything by itself,
     so it is up to you to skip the broken track.
 
+    Note
+    ----
+    This event will not automatically trigger the start of the next track in the queue,
+    so you must ensure that you do this if you want the player to continue playing from the queue.
+
     Attributes
     ----------
     player: :class:`BasePlayer`
         The player responsible for playing the track.
     track: :class:`DeferredAudioTrack`
         The track that failed to produce a playable track.
     original: Optional[:class:`Exception`]
```

### Comparing `lavalink-5.3.0/lavalink/filters.py` & `lavalink-5.4.0/lavalink/filters.py`

 * *Files identical despite different names*

### Comparing `lavalink-5.3.0/lavalink/node.py` & `lavalink-5.4.0/lavalink/node.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 """
+from asyncio import Task
 from collections import defaultdict
 from time import time
 from typing import (TYPE_CHECKING, Any, Dict, List, Optional, Type, TypeVar,
                     Union, overload)
 
 from .abc import BasePlayer, Filter
 from .common import MISSING
@@ -58,18 +59,18 @@
         The name the :class:`Node` is identified by.
     stats: :class:`Stats`
         The statistics of how the :class:`Node` is performing.
     """
     __slots__ = ('client', 'manager', '_transport', 'region', 'name', 'stats')
 
     def __init__(self, manager, host: str, port: int, password: str, region: str, name: Optional[str] = None,
-                 ssl: bool = False, session_id: Optional[str] = None):
+                 ssl: bool = False, session_id: Optional[str] = None, connect: bool = True):
         self.client: 'Client' = manager.client
         self.manager: 'NodeManager' = manager
-        self._transport = Transport(self, host, port, password, ssl, session_id)
+        self._transport = Transport(self, host, port, password, ssl, session_id, connect)
 
         self.region: str = region
         self.name: str = name or f'{region}-{host}:{port}'
         self.stats: Stats = Stats.empty(self)
 
     @property
     def session_id(self) -> Optional[str]:
@@ -135,14 +136,40 @@
         try:
             await self.get_version()
         except (AuthenticationError, ClientError, RequestError):
             return -1
 
         return (time() - start) * 1000
 
+    async def connect(self, force: bool = False) -> Optional[Task]:
+        """|coro|
+
+        Initiates a WebSocket connection to this node.
+        If a connection already exists, and ``force`` is ``False``, this will not do anything.
+
+        Parameters
+        ----------
+        force: :class:`bool`
+            Whether to close any existing WebSocket connections and re-establish a connection to
+            the node.
+
+        Returns
+        -------
+        Optional[:class:`asyncio.Task`]
+            The WebSocket connection task, or ``None`` if a WebSocket connection already exists and force
+            is ``False``.
+        """
+        if self._transport.ws_connected:
+            if not force:
+                return None
+
+            await self._transport.close()
+
+        return self._transport.connect()
+
     async def destroy(self):
         """|coro|
 
         Destroys the transport and any underlying connections for this node.
         This will also cleanly close the websocket.
         """
         await self._transport.destroy()
@@ -572,19 +599,19 @@
 
         if not json:
             return None
 
         return await self.request('PATCH', f'sessions/{session_id}', json=json)  # type: ignore
 
     @overload
-    async def request(self, method: str, path: str, *, to: Type[T], trace: bool = ..., versioned: bool = ..., **kwargs) -> T:
+    async def request(self, method: str, path: str, *, to: Type[str], trace: bool = ..., versioned: bool = ..., **kwargs) -> str:
         ...
 
     @overload
-    async def request(self, method: str, path: str, *, to: str, trace: bool = ..., versioned: bool = ..., **kwargs) -> str:
+    async def request(self, method: str, path: str, *, to: Type[T], trace: bool = ..., versioned: bool = ..., **kwargs) -> T:
         ...
 
     @overload
     async def request(self, method: str, path: str, *, trace: bool = ..., versioned: bool = ...,
                       **kwargs) -> Union[Dict[Any, Any], List[Any], bool]:
         ...
```

### Comparing `lavalink-5.3.0/lavalink/nodemanager.py` & `lavalink-5.4.0/lavalink/nodemanager.py`

 * *Files 5% similar despite different names*

```diff
@@ -64,31 +64,30 @@
         self.nodes: List[Node] = []
         self.regions: Dict[str, Tuple[str]] = regions or DEFAULT_REGIONS
 
     def __len__(self) -> int:
         return len(self.nodes)
 
     def __iter__(self) -> Iterator[Node]:
-        for node in self.nodes:
-            yield node
+        yield from self.nodes
 
     @property
     def available_nodes(self) -> List[Node]:
         """
         Returns a list of available nodes.
 
         .. deprecated:: 5.0.0
             As of Lavalink server 4.0.0, a WebSocket connection is no longer required to operate a
             node. As a result, this property is no longer considered useful as all nodes are considered
             available.
         """
         return [n for n in self.nodes if n.available]
 
     def add_node(self, host: str, port: int, password: str, region: str, name: Optional[str] = None,
-                 ssl: bool = False, session_id: Optional[str] = None) -> Node:
+                 ssl: bool = False, session_id: Optional[str] = None, connect: bool = True) -> Node:
         """
         Adds a node to this node manager.
 
         Parameters
         ----------
         host: :class:`str`
             The address of the Lavalink node.
@@ -96,31 +95,32 @@
             The port to use for websocket and REST connections.
         password: :class:`str`
             The password used for authentication.
         region: :class:`str`
             The region to assign this node to.
         name: Optional[:class:`str`]
             An identifier for the node that will show in logs. Defaults to ``None``.
-        reconnect_attempts: Optional[:class:`int`]
-            The amount of times connection with the node will be reattempted before giving up.
-            Set to `-1` for infinite. Defaults to ``3``.
-        ssl: Optional[:class:`bool`]
+        ssl: :class:`bool`
             Whether to use SSL for the node. SSL will use ``wss`` and ``https``, instead of ``ws`` and ``http``,
             respectively. Your node should support SSL if you intend to enable this, either via reverse proxy or
             other methods. Only enable this if you know what you're doing.
         session_id: Optional[:class:`str`]
             The ID of the session to resume. Defaults to ``None``.
             Only specify this if you have the ID of the session you want to resume.
+        connect: :class:`bool`
+            Whether to immediately connect to the node after creating it.
+            If ``False``, you must call :func:`Node.connect` if you require WebSocket functionality.
 
         Returns
         -------
         :class:`Node`
             The created Node instance.
         """
-        node = Node(self, host, port, password, region, name, ssl, session_id)
+        node = Node(self, host, port, password, region, name, ssl,
+                    session_id, connect)
         self.nodes.append(node)
         return node
 
     def remove_node(self, node: Node):
         """
         Removes a node.
```

### Comparing `lavalink-5.3.0/lavalink/player.py` & `lavalink-5.4.0/lavalink/player.py`

 * *Files 4% similar despite different names*

```diff
@@ -227,14 +227,19 @@
         """|coro|
 
         Plays the given track.
 
         This method differs from :func:`BasePlayer.play_track` in that it contains additional logic
         to handle certain attributes, such as ``loop``, ``shuffle``, and loading a base64 string from :class:`DeferredAudioTrack`.
 
+        Warning
+        -------
+        Multiple calls to this method within a short timeframe could cause issues with the player's
+        internal state, which can cause errors when processing a :class:`TrackStartEvent`.
+
         Parameters
         ----------
         track: Optional[Union[:class:`DeferredAudioTrack`, :class:`AudioTrack`, Dict[str, Union[Optional[str], bool, int]]]]
             The track to play. If left unspecified, this will default to the first track in the queue. Defaults to ``None``
             which plays the next song in queue. Accepts either an AudioTrack or a dict representing a track
             returned from Lavalink.
         start_time: :class:`int`
@@ -317,14 +322,19 @@
         await self.node.update_player(guild_id=self._internal_id, encoded_track=None)
         self.current = None
 
     async def skip(self):
         """|coro|
 
         Plays the next track in the queue, if any.
+
+        Warning
+        -------
+        Multiple calls to this method within a short timeframe could cause issues with the player's
+        internal state, which can cause errors when processing a :class:`TrackStartEvent`.
         """
         await self.play()
 
     def set_loop(self, loop: int):
         """
         Sets whether the player loops between a single track, queue or none.
 
@@ -627,44 +637,49 @@
 
     async def node_unavailable(self):
         """|coro|
 
         Called when a player's node becomes unavailable.
         Useful for changing player state before it's moved to another node.
         """
+        self._last_position = self.position
         self._internal_pause = True
 
     async def change_node(self, node: 'Node'):
         """|coro|
 
         Changes the player's node
 
         Parameters
         ----------
         node: :class:`Node`
             The node the player is changed to.
         """
+        old_node = self.node
+        self.node = node
+
+        last_position = self.position
+
         try:
             await self.node.destroy_player(self._internal_id)
         except (ClientError, RequestError):
             pass
 
-        old_node = self.node
-        self.node = node
-
         if self._voice_state:
             await self._dispatch_voice_update()
 
         if self.current:
             playable_track = self.current.track
 
             if isinstance(self.current, DeferredAudioTrack) and playable_track is None:
                 playable_track = await self.current.load(self.client)
 
-            await self.node.update_player(guild_id=self._internal_id, encoded_track=playable_track, position=self.position,
+            self._last_position = last_position  # Ensure that _last_position is correctly set, in case a node sends us bad data.
+
+            await self.node.update_player(guild_id=self._internal_id, encoded_track=playable_track, position=last_position,
                                           paused=self.paused, volume=self.volume)
             self._last_update = int(time() * 1000)
 
         self._internal_pause = False
 
         if self.filters:
             await self._apply_filters()
```

### Comparing `lavalink-5.3.0/lavalink/playermanager.py` & `lavalink-5.4.0/lavalink/playermanager.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,21 +65,19 @@
         self.players: Dict[int, PlayerT] = {}
 
     def __len__(self) -> int:
         return len(self.players)
 
     def __iter__(self) -> Iterator[Tuple[int, PlayerT]]:
         """ Returns an iterator that yields a tuple of (guild_id, player). """
-        for guild_id, player in self.players.items():
-            yield guild_id, player
+        yield from self.players.items()
 
     def values(self) -> Iterator[PlayerT]:
         """ Returns an iterator that yields only values. """
-        for player in self.players.values():
-            yield player
+        yield from self.players.values()
 
     def find_all(self, predicate: Optional[Callable[[PlayerT], bool]] = None):
         """
         Returns a list of players that match the given predicate.
 
         Parameters
         ----------
```

### Comparing `lavalink-5.3.0/lavalink/server.py` & `lavalink-5.4.0/lavalink/server.py`

 * *Files identical despite different names*

### Comparing `lavalink-5.3.0/lavalink/source_decoders.py` & `lavalink-5.4.0/lavalink/source_decoders.py`

 * *Files identical despite different names*

### Comparing `lavalink-5.3.0/lavalink/stats.py` & `lavalink-5.4.0/lavalink/stats.py`

 * *Files identical despite different names*

### Comparing `lavalink-5.3.0/lavalink/transport.py` & `lavalink-5.4.0/lavalink/transport.py`

 * *Files 6% similar despite different names*

```diff
@@ -32,33 +32,34 @@
                      NodeDisconnectedEvent, NodeReadyEvent, PlayerUpdateEvent,
                      TrackEndEvent, TrackExceptionEvent, TrackStartEvent,
                      TrackStuckEvent, WebSocketClosedEvent)
 from .server import EndReason, Severity
 from .stats import Stats
 
 if TYPE_CHECKING:
+    from .abc import BasePlayer
     from .client import Client
     from .node import Node
 
 _log = logging.getLogger(__name__)
 CLOSE_TYPES = (
     aiohttp.WSMsgType.CLOSE,
     aiohttp.WSMsgType.CLOSING,
     aiohttp.WSMsgType.CLOSED
 )
 MESSAGE_QUEUE_MAX_SIZE = 25
 LAVALINK_API_VERSION = 'v4'
 
 
 class Transport:
-    """ The class responsible for dealing with connections to Lavalink. """
+    """ The class responsible for handling connections to a Lavalink server. """
     __slots__ = ('client', '_node', '_session', '_ws', '_message_queue', 'trace_requests',
                  '_host', '_port', '_password', '_ssl', 'session_id', '_destroyed')
 
-    def __init__(self, node, host: str, port: int, password: str, ssl: bool, session_id: Optional[str]):
+    def __init__(self, node, host: str, port: int, password: str, ssl: bool, session_id: Optional[str], connect: bool = True):
         self.client: 'Client' = node.client
         self._node: 'Node' = node
 
         self._session: aiohttp.ClientSession = self.client._session
         self._ws: Optional[aiohttp.ClientWebSocketResponse] = None
         self._message_queue = []
         self.trace_requests = False
@@ -67,15 +68,16 @@
         self._port: int = port
         self._password: str = password
         self._ssl: bool = ssl
 
         self.session_id: Optional[str] = session_id
         self._destroyed: bool = False
 
-        self.connect()
+        if connect:
+            self.connect()
 
     @property
     def ws_connected(self):
         """ Returns whether the websocket is connected to Lavalink. """
         return self._ws is not None and not self._ws.closed
 
     @property
@@ -237,20 +239,25 @@
 
         if op == 'ready':
             self.session_id = data['sessionId']
             await self._node.manager._handle_node_ready(self._node)
             await self.client._dispatch_event(NodeReadyEvent(self._node, data['sessionId'], data['resumed']))
         elif op == 'playerUpdate':
             guild_id = int(data['guildId'])
-            player = self.client.player_manager.get(guild_id)
+            player: 'BasePlayer' = self.client.player_manager.get(guild_id)  # type: ignore
 
             if not player:
                 _log.debug('[Node:%s] Received playerUpdate for non-existent player! GuildId: %d', self._node.name, guild_id)
                 return
 
+            if player.node != self._node:
+                _log.debug('[Node:%s] Received playerUpdate for a player that doesn\'t belong to this node (player is moving?) GuildId: %d',
+                           self._node.name, guild_id)
+                return
+
             state = data['state']
             await player.update_state(state)
             await self.client._dispatch_event(PlayerUpdateEvent(player, state))
         elif op == 'stats':
             self._node.stats = Stats(self._node, data)
         elif op == 'event':
             await self._handle_event(data)
@@ -262,15 +269,15 @@
         Handles the event from Lavalink.
 
         Parameters
         ----------
         data: :class:`dict`
             The data given from Lavalink.
         """
-        player = self.client.player_manager.get(int(data['guildId']))
+        player: 'BasePlayer' = self.client.player_manager.get(int(data['guildId']))  # type: ignore
         event_type = data['type']
 
         if not player:
             if event_type not in ('TrackEndEvent', 'WebSocketClosedEvent'):  # Player was most likely destroyed if it's any of these.
                 _log.warning('[Node:%s] Received event type %s for non-existent player! GuildId: %s', self._node.name, event_type, data['guildId'])
 
             return
@@ -368,11 +375,11 @@
                     return json if to is None else to.from_dict(json)
 
                 if res.status == 204:
                     return True
 
                 raise RequestError('An invalid response was received from the node.',
                                    status=res.status, response=await res.json(), params=kwargs.get('params', {}))
-        except RequestError:
-            raise
+        except (AuthenticationError, RequestError):
+            raise  # Pass the caught errors back to the caller in their 'original' form.
         except Exception as original:  # It's not pretty but aiohttp doesn't specify what exceptions can be thrown.
             raise ClientError from original
```

### Comparing `lavalink-5.3.0/lavalink/utfm_codec.py` & `lavalink-5.4.0/lavalink/utfm_codec.py`

 * *Files identical despite different names*

### Comparing `lavalink-5.3.0/lavalink/utils.py` & `lavalink-5.4.0/lavalink/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -19,24 +19,24 @@
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 """
 import struct
 from base64 import b64encode
-from typing import Any, Callable, Dict, Mapping, Optional, Tuple, Union
+from typing import Any, Callable, Dict, Mapping, Optional, Tuple
 
 from .common import MISSING
 from .dataio import DataReader, DataWriter
 from .errors import InvalidTrack
 from .player import AudioTrack
 from .source_decoders import DEFAULT_DECODER_MAPPING
 
 V2_KEYSET = {'title', 'author', 'length', 'identifier', 'isStream', 'uri', 'sourceName', 'position'}
-V3_KEYSET = {'title', 'author', 'length', 'identifier', 'isStream', 'uri', 'artworkUrl', 'isrc', 'sourceName', 'position'}
+V3_KEYSET = V2_KEYSET | {'artworkUrl', 'isrc'}
 
 
 def timestamp_to_millis(timestamp: str) -> int:
     """
     Converts a timestamp such as 03:28 or 02:15:53 to milliseconds.
 
     Example
@@ -136,15 +136,15 @@
     length = reader.read_long()
     identifier = reader.read_utf().decode()
     is_stream = reader.read_boolean()
     uri = reader.read_nullable_utf()
     return (title, author, length, identifier, is_stream, uri)
 
 
-def _write_track_common(track: Dict[str, Union[Optional[str], bool, int]], writer: DataWriter):
+def _write_track_common(track: Dict[str, Any], writer: DataWriter):
     writer.write_utf(track['title'])
     writer.write_utf(track['author'])
     writer.write_long(track['length'])
     writer.write_utf(track['identifier'])
     writer.write_boolean(track['isStream'])
     writer.write_nullable_utf(track['uri'])
 
@@ -156,15 +156,15 @@
 
     Parameters
     ----------
     track: :class:`str`
         The base64 track string.
     source_decoders: Mapping[:class:`str`, Callable[[:class:`DataReader`], Dict[:class:`str`, Any]]]
         A mapping of source-specific decoders to use.
-        Some Lavaplayer sources have additional fields encoded on a per-sourcemanager basis, so you can
+        Some Lavaplayer sources have additional fields encoded on a per-source manager basis, so you can
         specify a mapping of decoders that will handle decoding these additional fields. You can find some
         example decoders within the ``source_decoders`` file. This isn't required for all sources, so ensure
         that you need them before specifying.
 
         To overwrite library-provided decoders, just specify them within the mapping and the new decoders will
         be used.
 
@@ -212,28 +212,38 @@
         }
     }
 
     return AudioTrack(track_object, 0, position=position, encoder_version=version,
                       source_specific=source_specific_fields)
 
 
-def encode_track(track: Dict[str, Union[Optional[str], int, bool]]) -> Tuple[int, str]:
+def encode_track(track: Dict[str, Any],
+                 source_encoders: Mapping[str, Callable[[DataWriter, Dict[str, Any]], None]] = MISSING) -> Tuple[int, str]:
     """
     Encodes a track dict into a base64 string, readable by the Lavalink server.
 
     A track should have *at least* the following keys:
     ``title``, ``author``, ``length``, ``identifier``, ``isStream``, ``uri``, ``sourceName`` and ``position``.
 
     If the track is a v3 track, it should have the following additional fields:
     ``artworkUrl`` and ``isrc``. isrc can be ``None`` if not applicable.
 
     Parameters
     ----------
     track: Dict[str, Union[Optional[str], int, bool]]
         The track dict to serialize.
+    source_encoders: Mapping[:class:`str`, Callable[[:class:`DataWriter`]]
+        A mapping of source-specific encoders to use.
+        Some Lavaplayer sources have additional fields encoded on a per-source manager basis, so you can
+        specify a mapping of encoders that will handle encoding these additional fields. This isn't required
+        for all sources, so ensure that you need them before specifying.
+
+        The mapping must be in the format of something like ``{'http': http_encoder_function}``, where the
+        key ``str`` is the name of the source. These functions will only be called if track's ``sourceName``
+        field matches.
 
     Raises
     ------
     :class:`InvalidTrack`
         If the track has unexpected, or missing keys, possibly due to an incompatible version or another reason.
 
     Returns
@@ -246,41 +256,51 @@
 
     if not V2_KEYSET <= track_keys:  # V2_KEYSET contains the minimum number of fields required to successfully encode a track.
         missing_keys = [k for k in V2_KEYSET if k not in track]
 
         raise InvalidTrack(f'Track object is missing keys required for serialization: {", ".join(missing_keys)}')
 
     if V3_KEYSET <= track_keys:
-        return (3, encode_track_v3(track))
+        return (3, encode_track_v3(track, source_encoders))
 
-    return (2, encode_track_v2(track))
+    return (2, encode_track_v2(track, source_encoders))
 
 
-def encode_track_v2(track: Dict[str, Union[Optional[str], bool, int]]) -> str:
+def encode_track_v2(track: Dict[str, Any],
+                    source_encoders: Mapping[str, Callable[[DataWriter, Dict[str, Any]], None]] = MISSING) -> str:
     assert V2_KEYSET <= track.keys()
 
     writer = DataWriter()
 
     version = struct.pack('B', 2)
     writer.write_byte(version)
     _write_track_common(track, writer)
     writer.write_utf(track['sourceName'])
+
+    if source_encoders is not MISSING and track['sourceName'] in source_encoders:
+        source_encoders[track['sourceName']](writer, track)
+
     writer.write_long(track['position'])
 
     enc = writer.finish()
     return b64encode(enc).decode()
 
 
-def encode_track_v3(track: Dict[str, Union[Optional[str], bool, int]]) -> str:
+def encode_track_v3(track: Dict[str, Any],
+                    source_encoders: Mapping[str, Callable[[DataWriter, Dict[str, Any]], None]] = MISSING) -> str:
     assert V3_KEYSET <= track.keys()
 
     writer = DataWriter()
     version = struct.pack('B', 3)
     writer.write_byte(version)
     _write_track_common(track, writer)
     writer.write_nullable_utf(track['artworkUrl'])
     writer.write_nullable_utf(track['isrc'])
     writer.write_utf(track['sourceName'])
+
+    if source_encoders is not MISSING and track['sourceName'] in source_encoders:
+        source_encoders[track['sourceName']](writer, track)
+
     writer.write_long(track['position'])
 
     enc = writer.finish()
     return b64encode(enc).decode()
```

### Comparing `lavalink-5.3.0/lavalink.egg-info/SOURCES.txt` & `lavalink-5.4.0/lavalink.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lavalink-5.3.0/setup.py` & `lavalink-5.4.0/setup.py`

 * *Files identical despite different names*

