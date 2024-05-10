# Comparing `tmp/omuchatprovider-0.2.5.tar.gz` & `tmp/omuchatprovider-0.3.0.tar.gz`

## Comparing `omuchatprovider-0.2.5.tar` & `omuchatprovider-0.3.0.tar`

### file list

```diff
@@ -1,35 +1,36 @@
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 omuchatprovider-0.2.5/src/omuchatprovider/__init__.py
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 omuchatprovider-0.2.5/src/omuchatprovider/__main__.py
--rw-r--r--   0        0        0     4042 2020-02-02 00:00:00.000000 omuchatprovider-0.2.5/src/omuchatprovider/chatprovider.py
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 omuchatprovider-0.2.5/src/omuchatprovider/errors.py
--rw-r--r--   0        0        0     2718 2020-02-02 00:00:00.000000 omuchatprovider-0.2.5/src/omuchatprovider/helper.py
--rw-r--r--   0        0        0     1008 2020-02-02 00:00:00.000000 omuchatprovider-0.2.5/src/omuchatprovider/tasks.py
--rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 omuchatprovider-0.2.5/src/omuchatprovider/throttle.py
--rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 omuchatprovider-0.2.5/src/omuchatprovider/services/__init__.py
--rw-r--r--   0        0        0      969 2020-02-02 00:00:00.000000 omuchatprovider-0.2.5/src/omuchatprovider/services/service.py
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 omuchatprovider-0.2.5/src/omuchatprovider/services/youtube/__init__.py
--rw-r--r--   0        0        0    22986 2020-02-02 00:00:00.000000 omuchatprovider-0.2.5/src/omuchatprovider/services/youtube/chat.py
--rw-r--r--   0        0        0     1451 2020-02-02 00:00:00.000000 omuchatprovider-0.2.5/src/omuchatprovider/services/youtube/const.py
--rw-r--r--   0        0        0     1612 2020-02-02 00:00:00.000000 omuchatprovider-0.2.5/src/omuchatprovider/services/youtube/youtube.py
--rw-r--r--   0        0        0     8167 2020-02-02 00:00:00.000000 omuchatprovider-0.2.5/src/omuchatprovider/services/youtube/youtubeapi.py
--rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 omuchatprovider-0.2.5/src/omuchatprovider/services/youtube/types/__init__.py
--rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 omuchatprovider-0.2.5/src/omuchatprovider/services/youtube/types/accessibility.py
--rw-r--r--   0        0        0     8239 2020-02-02 00:00:00.000000 omuchatprovider-0.2.5/src/omuchatprovider/services/youtube/types/chatactions.py
--rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 omuchatprovider-0.2.5/src/omuchatprovider/services/youtube/types/contents.py
--rw-r--r--   0        0        0      657 2020-02-02 00:00:00.000000 omuchatprovider-0.2.5/src/omuchatprovider/services/youtube/types/continuations.py
--rw-r--r--   0        0        0     2352 2020-02-02 00:00:00.000000 omuchatprovider-0.2.5/src/omuchatprovider/services/youtube/types/frameworkupdates.py
--rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 omuchatprovider-0.2.5/src/omuchatprovider/services/youtube/types/image.py
--rw-r--r--   0        0        0      442 2020-02-02 00:00:00.000000 omuchatprovider-0.2.5/src/omuchatprovider/services/youtube/types/live_chat.py
--rw-r--r--   0        0        0      967 2020-02-02 00:00:00.000000 omuchatprovider-0.2.5/src/omuchatprovider/services/youtube/types/metadataactions.py
--rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 omuchatprovider-0.2.5/src/omuchatprovider/services/youtube/types/responsecontext.py
--rw-r--r--   0        0        0     1828 2020-02-02 00:00:00.000000 omuchatprovider-0.2.5/src/omuchatprovider/services/youtube/types/runs.py
--rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 omuchatprovider-0.2.5/src/omuchatprovider/services/youtube/types/simpletext.py
--rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 omuchatprovider-0.2.5/src/omuchatprovider/services/youtube/types/updated_metadata.py
--rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 omuchatprovider-0.2.5/src/omuchatprovider/services/youtube/types/urlendpoint.py
--rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 omuchatprovider-0.2.5/src/omuchatprovider/services/youtube/types/youtuberesponse.py
--rw-r--r--   0        0        0    40286 2020-02-02 00:00:00.000000 omuchatprovider-0.2.5/src/omuchatprovider/services/youtube/types/ytcfg.py
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 omuchatprovider-0.2.5/src/omuchatprovider/services/youtube/types/ytinitialdata.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 omuchatprovider-0.2.5/.gitignore
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 omuchatprovider-0.2.5/README.md
--rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 omuchatprovider-0.2.5/pyproject.toml
--rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 omuchatprovider-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 omuchatprovider-0.3.0/src/omuchatprovider/__init__.py
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 omuchatprovider-0.3.0/src/omuchatprovider/__main__.py
+-rw-r--r--   0        0        0     4041 2020-02-02 00:00:00.000000 omuchatprovider-0.3.0/src/omuchatprovider/chatprovider.py
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 omuchatprovider-0.3.0/src/omuchatprovider/errors.py
+-rw-r--r--   0        0        0     2837 2020-02-02 00:00:00.000000 omuchatprovider-0.3.0/src/omuchatprovider/helper.py
+-rw-r--r--   0        0        0      978 2020-02-02 00:00:00.000000 omuchatprovider-0.3.0/src/omuchatprovider/tasks.py
+-rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 omuchatprovider-0.3.0/src/omuchatprovider/throttle.py
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 omuchatprovider-0.3.0/src/omuchatprovider/version.py
+-rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 omuchatprovider-0.3.0/src/omuchatprovider/services/__init__.py
+-rw-r--r--   0        0        0      948 2020-02-02 00:00:00.000000 omuchatprovider-0.3.0/src/omuchatprovider/services/service.py
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 omuchatprovider-0.3.0/src/omuchatprovider/services/youtube/__init__.py
+-rw-r--r--   0        0        0    23543 2020-02-02 00:00:00.000000 omuchatprovider-0.3.0/src/omuchatprovider/services/youtube/chat.py
+-rw-r--r--   0        0        0     2008 2020-02-02 00:00:00.000000 omuchatprovider-0.3.0/src/omuchatprovider/services/youtube/const.py
+-rw-r--r--   0        0        0     1751 2020-02-02 00:00:00.000000 omuchatprovider-0.3.0/src/omuchatprovider/services/youtube/youtube.py
+-rw-r--r--   0        0        0     8155 2020-02-02 00:00:00.000000 omuchatprovider-0.3.0/src/omuchatprovider/services/youtube/youtubeapi.py
+-rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 omuchatprovider-0.3.0/src/omuchatprovider/services/youtube/types/__init__.py
+-rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 omuchatprovider-0.3.0/src/omuchatprovider/services/youtube/types/accessibility.py
+-rw-r--r--   0        0        0     8175 2020-02-02 00:00:00.000000 omuchatprovider-0.3.0/src/omuchatprovider/services/youtube/types/chatactions.py
+-rw-r--r--   0        0        0      685 2020-02-02 00:00:00.000000 omuchatprovider-0.3.0/src/omuchatprovider/services/youtube/types/contents.py
+-rw-r--r--   0        0        0      651 2020-02-02 00:00:00.000000 omuchatprovider-0.3.0/src/omuchatprovider/services/youtube/types/continuations.py
+-rw-r--r--   0        0        0     2346 2020-02-02 00:00:00.000000 omuchatprovider-0.3.0/src/omuchatprovider/services/youtube/types/frameworkupdates.py
+-rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 omuchatprovider-0.3.0/src/omuchatprovider/services/youtube/types/image.py
+-rw-r--r--   0        0        0      442 2020-02-02 00:00:00.000000 omuchatprovider-0.3.0/src/omuchatprovider/services/youtube/types/live_chat.py
+-rw-r--r--   0        0        0      961 2020-02-02 00:00:00.000000 omuchatprovider-0.3.0/src/omuchatprovider/services/youtube/types/metadataactions.py
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 omuchatprovider-0.3.0/src/omuchatprovider/services/youtube/types/responsecontext.py
+-rw-r--r--   0        0        0     1810 2020-02-02 00:00:00.000000 omuchatprovider-0.3.0/src/omuchatprovider/services/youtube/types/runs.py
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 omuchatprovider-0.3.0/src/omuchatprovider/services/youtube/types/simpletext.py
+-rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 omuchatprovider-0.3.0/src/omuchatprovider/services/youtube/types/updated_metadata.py
+-rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 omuchatprovider-0.3.0/src/omuchatprovider/services/youtube/types/urlendpoint.py
+-rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 omuchatprovider-0.3.0/src/omuchatprovider/services/youtube/types/youtuberesponse.py
+-rw-r--r--   0        0        0    40280 2020-02-02 00:00:00.000000 omuchatprovider-0.3.0/src/omuchatprovider/services/youtube/types/ytcfg.py
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 omuchatprovider-0.3.0/src/omuchatprovider/services/youtube/types/ytinitialdata.py
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 omuchatprovider-0.3.0/.gitignore
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 omuchatprovider-0.3.0/README.md
+-rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 omuchatprovider-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      416 2020-02-02 00:00:00.000000 omuchatprovider-0.3.0/PKG-INFO
```

### Comparing `omuchatprovider-0.2.5/src/omuchatprovider/chatprovider.py` & `omuchatprovider-0.3.0/src/omuchatprovider/chatprovider.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,36 +1,37 @@
 import asyncio
 import time
-from typing import Dict
 
 from loguru import logger
 from omu.identifier import Identifier
 from omuchat import App, Channel, Client, Message, Room, events
 
 from omuchatprovider.errors import ProviderError
 
 from .services import ChatService, ProviderService, get_services
 
 BASE_PROVIDER_IDENTIFIER = Identifier("cc.omuchat", "chatprovider")
 APP = App(
-    identifier=BASE_PROVIDER_IDENTIFIER,
+    id=BASE_PROVIDER_IDENTIFIER,
     version="0.1.0",
 )
 
 
 client = Client(APP)
 
-services: Dict[str, ProviderService] = {}
-chat_services: Dict[Identifier, ChatService] = {}
+services: dict[Identifier, ProviderService] = {}
+chat_services: dict[Identifier, ChatService] = {}
+
+for service_class in get_services():
+    service = service_class(client)
+    services[service.provider.id] = service
 
 
 async def register_services():
-    for service_class in get_services():
-        service = service_class(client)
-        services[service.provider.key()] = service
+    for service in services.values():
         await client.chat.providers.add(service.provider)
 
 
 async def update_channel(channel: Channel, service: ProviderService):
     try:
         if not channel.active:
             return
```

### Comparing `omuchatprovider-0.2.5/src/omuchatprovider/helper.py` & `omuchatprovider-0.3.0/src/omuchatprovider/helper.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,25 @@
 from __future__ import annotations
 
 import json
 import re
 import time
-from typing import Callable, Coroutine
+from collections.abc import Callable, Coroutine
 
 import aiohttp
 from loguru import logger
 from omuchat import Provider
 
 HTTP_REGEX = r"(https?://)?(www\.)?"
-URL_NORMALIZE_REGEX = r"(?P<protocol>https?)?:?\/?\/?(?P<domain>[^.]+\.[^\/]+)(?P<path>[^?#]+)?(?P<query>.+)?"
+URL_NORMALIZE_REGEX = (
+    r"(?P<protocol>https?)?:?\/?\/?"
+    r"(?P<domain>[^.]+\.[^\/]+)"
+    r"(?P<path>[^?#]+)?"
+    r"(?P<query>.+)?"
+)
 
 
 def get_session(provider: Provider) -> aiohttp.ClientSession:
     user_agent = json.dumps(
         [
             "OmuChat",
             {
@@ -28,15 +33,19 @@
     return session
 
 
 def normalize_url(url: str) -> str:
     match = re.match(URL_NORMALIZE_REGEX, url)
     if match is None:
         raise ValueError(f"Invalid URL: {url}")
-    return f"{match.group('protocol') or 'https'}://{match.group('domain')}{match.group('path') or ''}{match.group('query') or ''}"
+    protocol = match.group("protocol") or "https"
+    domain = match.group("domain")
+    path = match.group("path") or ""
+    query = match.group("query") or ""
+    return f"{protocol}://{domain}{path}{query}"
 
 
 def assert_none[T](value: T | None, message: str) -> T:
     if value is None:
         raise ValueError(message)
     return value
```

### Comparing `omuchatprovider-0.2.5/src/omuchatprovider/tasks.py` & `omuchatprovider-0.3.0/src/omuchatprovider/tasks.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 import asyncio
 import time
 import traceback
 import typing
-from typing import Dict, List
 
 
 class Tasks:
     def __init__(self, loop: asyncio.AbstractEventLoop) -> None:
         self.loop = loop
-        self.tasks: List[asyncio.Task] = []
-        self.times: Dict[str, float] = {}
-        self.times_max: Dict[str, float] = {}
+        self.tasks: list[asyncio.Task] = []
+        self.times: dict[str, float] = {}
+        self.times_max: dict[str, float] = {}
 
     def terminate(self):
         for task in self.tasks:
             task.cancel()
 
     def create_task(self, coro: typing.Coroutine):
         name = coro.__name__
```

### Comparing `omuchatprovider-0.2.5/src/omuchatprovider/throttle.py` & `omuchatprovider-0.3.0/src/omuchatprovider/throttle.py`

 * *Files identical despite different names*

### Comparing `omuchatprovider-0.2.5/src/omuchatprovider/services/service.py` & `omuchatprovider-0.3.0/src/omuchatprovider/services/service.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from __future__ import annotations
 
 import abc
-import typing
 from dataclasses import dataclass
 
 from omu.helper import Coro
 from omuchat import Channel, Client, Provider, Room
 
 type ChatServiceFactory = Coro[[], ChatService]
 
@@ -21,15 +20,15 @@
     def __init__(self, client: Client): ...
 
     @property
     @abc.abstractmethod
     def provider(self) -> Provider: ...
 
     @abc.abstractmethod
-    async def fetch_rooms(self, channel: Channel) -> typing.List[FetchedRoom]: ...
+    async def fetch_rooms(self, channel: Channel) -> list[FetchedRoom]: ...
 
     @abc.abstractmethod
     async def is_online(self, room: Room) -> bool: ...
 
 
 class ChatService(abc.ABC):
     @property
```

### Comparing `omuchatprovider-0.2.5/src/omuchatprovider/services/youtube/chat.py` & `omuchatprovider-0.3.0/src/omuchatprovider/services/youtube/chat.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 import asyncio
 import json
 import re
 import urllib.parse
 from collections import Counter
 from dataclasses import dataclass
 from datetime import datetime
-from typing import TYPE_CHECKING, Dict, List, Tuple
+from typing import TYPE_CHECKING
 
 import bs4
-from iwashi.visitors.youtube import Youtube
+from iwashi.service import Youtube
 from loguru import logger
 from omu.helper import map_optional
 from omuchat.client import Client
 from omuchat.model import (
     MODERATOR,
     OWNER,
     VERIFIED,
@@ -105,15 +105,15 @@
             .map(lambda x: x[0])
             .map(lambda x: x.get("invalidationContinuationData"))
             .map(lambda x: x.get("continuation"))
             .get()
         )
 
     @classmethod
-    def extract_script(cls, soup: bs4.BeautifulSoup, startswith: str) -> Dict | None:
+    def extract_script(cls, soup: bs4.BeautifulSoup, startswith: str) -> dict | None:
         for script in soup.select("script"):
             script_text = script.text.strip()
             if script_text.startswith(startswith):
                 break
         else:
             return None
         if "{" not in script_text or "}" not in script_text:
@@ -177,17 +177,17 @@
         data = await self.api.updated_metadata(
             video_id=self.video_id,
             key=self.api_key,
             continuation=self.metadata_continuation,
         )
         self.metadata_continuation = (
             traverse(data)
-            .map(lambda x: x["continuation"])
-            .map(lambda x: x["timedContinuationData"])
-            .map(lambda x: x["continuation"])
+            .map(lambda x: x.get("continuation"))
+            .map(lambda x: x.get("timedContinuationData"))
+            .map(lambda x: x.get("continuation"))
             .get()
         )
         viewer_count: int | None = None
         title: content.Component | None = None
         description: content.Component | None = None
         for action in data.get("actions", []):
             if "updateViewershipAction" in action:
@@ -227,27 +227,32 @@
         chat: YoutubeChat,
     ):
         self.youtube = youtube_service
         self.client = client
         self._room = room
         self.chat = chat
         self.tasks = Tasks(client.loop)
-        self.author_fetch_queue: List[Author] = []
+        self.author_fetch_queue: list[Author] = []
         self._closed = False
 
     @property
     def room(self) -> Room:
         return self._room
 
     @property
     def closed(self) -> bool:
         return self._closed
 
     @classmethod
-    async def create(cls, youtube_service: YoutubeService, client: Client, room: Room):
+    async def create(
+        cls,
+        youtube_service: YoutubeService,
+        client: Client,
+        room: Room,
+    ):
         await client.chat.rooms.update(room)
         video_id = room.id.path[-1]
         chat = await YoutubeChat.from_video_id(
             youtube_service.extractor,
             video_id,
         )
         room.metadata = RoomMetadata(
@@ -277,121 +282,139 @@
                     self.room.metadata = metadata
                     await self.client.chat.rooms.update(self.room)
                 count += 1
         finally:
             await self.stop()
 
     async def process_chat_data(self, chat_data: ChatData):
-        messages: List[Message] = []
-        authors: List[Author] = []
+        messages: list[Message] = []
+        authors: list[Author] = []
         for action in chat_data.chat_actions:
             if "addChatItemAction" in action:
-                message, author = await self.process_message_item(
-                    action["addChatItemAction"]["item"]
+                await self.process_message_item(
+                    action["addChatItemAction"]["item"],
+                    messages,
+                    authors,
                 )
-                if message:
-                    messages.append(message)
-                if author:
-                    authors.append(author)
+            elif "addLiveChatTickerItemAction" in action:
+                pass
             elif "markChatItemAsDeletedAction" in action:
                 await self.process_deleted_item(action["markChatItemAsDeletedAction"])
             elif "removeChatItemAction" in action:
                 await self.process_deleted_item(action["removeChatItemAction"])
+            elif "removeChatItemByAuthorAction" in action:
+                pass
             else:
                 logger.warning(f"Unknown chat action: {action}")
         if len(authors) > 0:
-            added_authors: List[Author] = []
+            added_authors: list[Author] = []
             for author in authors:
                 if author.key() in self.client.chat.authors.cache:
                     continue
                 added_authors.append(author)
             await self.client.chat.authors.add(*added_authors)
             self.author_fetch_queue.extend(added_authors)
         if len(messages) > 0:
             await self.client.chat.messages.add(*messages)
         await self.process_reactions(chat_data)
 
     async def fetch_authors_task(self):
-        while not self._closed:
-            if len(self.author_fetch_queue) == 0:
-                await asyncio.sleep(1)
-                continue
-            for author in self.author_fetch_queue:
-                await asyncio.sleep(3)
-                author_channel = await YOUTUBE_VISITOR.visit_url(
-                    f"{YOUTUBE_URL}/channel/{author.id}", self.youtube.session
-                )
-                if author_channel is None:
+        try:
+            while not self._closed:
+                if len(self.author_fetch_queue) == 0:
+                    await asyncio.sleep(1)
                     continue
-                metadata: AuthorMetadata = author.metadata or {}
-                metadata["avatar_url"] = author_channel.profile_picture
-                metadata["url"] = author_channel.url
-                metadata["links"] = list(author_channel.links)
-                if "@" in author_channel.url:
-                    metadata["screen_id"] = author_channel.url.split("@")[-1]
-                author.metadata = metadata
-                await self.client.chat.authors.update(author)
+                for author in self.author_fetch_queue:
+                    await asyncio.sleep(3)
+                    new_metadata = await self.fetch_author_metadata(author)
+                    metadata = author.metadata or {}
+                    metadata |= new_metadata
+                    author.metadata = metadata
+                    await self.client.chat.authors.update(author)
+        except asyncio.CancelledError:
+            return
+
+    async def fetch_author_metadata(self, author: Author) -> AuthorMetadata:
+        author_channel = await YOUTUBE_VISITOR.visit_url(
+            self.youtube.session,
+            f"https://youtube.com/channel/{author.id.path[-1]}",
+        )
+        if author_channel is None:
+            return {}
+        new_metadata: AuthorMetadata = {}
+        new_metadata["avatar_url"] = author_channel.profile_picture
+        new_metadata["url"] = author_channel.url
+        new_metadata["links"] = list(author_channel.links)
+        new_metadata["screen_id"] = author_channel.id
+        return new_metadata
 
     async def process_message_item(
-        self, item: AddChatItemActionItem
-    ) -> Tuple[Message | None, Author | None]:
+        self,
+        item: AddChatItemActionItem,
+        messages: list[Message],
+        authors: list[Author],
+    ) -> None:
         if "liveChatTextMessageRenderer" in item:
             data = item["liveChatTextMessageRenderer"]
             author = self._parse_author(data)
             message = _parse_runs(data["message"])
             created_at = self._parse_created_at(data)
             message = Message(
                 id=self.room.id / data["id"],
-                room_id=self._room.key(),
-                author_id=author.key(),
+                room_id=self._room.id,
+                author_id=author.id,
                 content=message,
                 created_at=created_at,
             )
-            return message, author
+            messages.append(message)
+            authors.append(author)
         elif "liveChatPaidMessageRenderer" in item:
             data = item["liveChatPaidMessageRenderer"]
             author = self._parse_author(data)
             message = map_optional(data.get("message"), _parse_runs)
             paid = self._parse_paid(data)
             created_at = self._parse_created_at(data)
             message = Message(
                 id=self.room.id / data["id"],
-                room_id=self._room.key(),
-                author_id=author.key(),
+                room_id=self._room.id,
+                author_id=author.id,
                 content=message,
                 paid=paid,
                 created_at=created_at,
             )
-            return message, author
+            messages.append(message)
+            authors.append(author)
         elif "liveChatMembershipItemRenderer" in item:
             data = item["liveChatMembershipItemRenderer"]
             author = self._parse_author(data)
             created_at = self._parse_created_at(data)
             component = content.System.of(_parse_runs(data["headerSubtext"]))
             message = Message(
                 id=self.room.id / data["id"],
-                room_id=self._room.key(),
-                author_id=author.key(),
+                room_id=self._room.id,
+                author_id=author.id,
                 content=component,
                 created_at=created_at,
             )
-            return message, author
+            messages.append(message)
+            authors.append(author)
         elif "liveChatSponsorshipsGiftRedemptionAnnouncementRenderer" in item:
             data = item["liveChatSponsorshipsGiftRedemptionAnnouncementRenderer"]
             author = self._parse_author(data)
             created_at = self._parse_created_at(data)
             component = content.System.of(_parse_runs(data["message"]))
             message = Message(
                 id=self.room.id / data["id"],
-                room_id=self._room.key(),
-                author_id=author.key(),
+                room_id=self._room.id,
+                author_id=author.id,
                 content=component,
                 created_at=created_at,
             )
-            return message, author
+            messages.append(message)
+            authors.append(author)
         elif "liveChatSponsorshipsGiftPurchaseAnnouncementRenderer" in item:
             data = item["liveChatSponsorshipsGiftPurchaseAnnouncementRenderer"]
             created_at = self._parse_created_at(data)
             header = data["header"]["liveChatSponsorshipsHeaderRenderer"]
             author = self._parse_author(header, id=data["authorExternalChannelId"])
             component = content.System.of(_parse_runs(header["primaryText"]))
 
@@ -403,21 +426,22 @@
                 name=gift_name,
                 amount=1,
                 is_paid=True,
                 image_url=image_url,
             )
             message = Message(
                 id=self.room.id / data["id"],
-                room_id=self._room.key(),
-                author_id=author.key(),
+                room_id=self._room.id,
+                author_id=author.id,
                 content=component,
                 created_at=created_at,
                 gifts=[gift],
             )
-            return message, author
+            messages.append(message)
+            authors.append(author)
         elif "liveChatPlaceholderItemRenderer" in item:
             """
             item["liveChatPlaceholderItemRenderer"] = {'id': 'ChwKGkNJdml3ZUg0aDRRREZSTEV3Z1FkWUlJTkNR', 'timestampUsec': '1706714981296711'}}
             """
         elif "liveChatPaidStickerRenderer" in item:
             data = item["liveChatPaidStickerRenderer"]
             author = self._parse_author(data)
@@ -430,23 +454,23 @@
                 name=sticker_name,
                 amount=1,
                 is_paid=True,
                 image_url=sticker_image,
             )
             message = Message(
                 id=self.room.id / data["id"],
-                room_id=self._room.key(),
-                author_id=author.key(),
+                room_id=self._room.id,
+                author_id=author.id,
                 gifts=[sticker],
                 created_at=created_at,
             )
-            return message, author
+            messages.append(message)
+            authors.append(author)
         else:
             raise ProviderError(f"Unknown message type: {list(item.keys())} {item=}")
-        return None, None
 
     async def process_deleted_item(self, item: MarkChatItemAsDeletedAction):
         id = self._room.id / item["targetItemId"]
         message = await self.client.chat.messages.get(id.key())
         if message:
             await self.client.chat.messages.remove(message)
 
@@ -468,15 +492,15 @@
                     {
                         reaction["unicodeEmojiId"]: reaction["reactionCount"]
                         for reaction in bucket.get("reactionsData", [])
                     }
                 )
         if not reaction_counts:
             return
-        await self.youtube.reaction_message.broadcast(
+        await self.youtube.reaction_signal.notify(
             {
                 "room_id": self._room.key(),
                 "reactions": dict(reaction_counts),
             },
         )
 
     def _parse_author(self, message: AuthorInfo, id: str | None = None) -> Author:
@@ -493,15 +517,15 @@
             traverse(message)
             .map(lambda x: x.get("authorPhoto"))
             .map(lambda x: x.get("thumbnails"))
             .map(lambda x: x[0])
             .map(lambda x: x.get("url"))
             .get()
         )
-        roles: List[Role] = []
+        roles: list[Role] = []
         for badge in message.get("authorBadges", []):
             if "icon" in badge["liveChatAuthorBadgeRenderer"]:
                 icon_type = badge["liveChatAuthorBadgeRenderer"]["icon"]["iconType"]
                 if icon_type == "MODERATOR":
                     roles.append(MODERATOR)
                 elif icon_type == "OWNER":
                     roles.append(OWNER)
@@ -520,16 +544,16 @@
                         icon_url=custom_thumbnail["thumbnails"][0]["url"],
                         is_owner=False,
                         is_moderator=False,
                     )
                 )
 
         return Author(
-            provider_id=self.youtube.provider.key(),
-            id=id,
+            provider_id=self.youtube.provider.id,
+            id=self.room.id / id,
             name=name,
             avatar_url=avatar_url,
             roles=roles,
         )
 
     def _parse_paid(self, message: LiveChatPaidMessageRenderer) -> Paid:
         currency_match = re.search(
@@ -571,15 +595,15 @@
 
 def _get_accessibility_label(data: Accessibility | None) -> str | None:
     if data is None:
         return None
     return data.get("accessibilityData", {}).get("label", None)
 
 
-def _get_best_thumbnail(thumbnails: List[Thumbnail]) -> str:
+def _get_best_thumbnail(thumbnails: list[Thumbnail]) -> str:
     if len(thumbnails) == 0:
         raise ProviderError("No thumbnails found")
     best = max(thumbnails, key=lambda x: x.get("width", 0) * x.get("height", 0))
     return normalize_yt_url(best["url"])
 
 
 def _parse_runs(runs: Runs | None) -> content.Component:
```

### Comparing `omuchatprovider-0.2.5/src/omuchatprovider/services/youtube/youtube.py` & `omuchatprovider-0.3.0/src/omuchatprovider/services/youtube/youtube.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,47 +1,55 @@
-from typing import List
-
 from omuchat.client import Client
 from omuchat.model.channel import Channel
 from omuchat.model.provider import Provider
 from omuchat.model.room import Room
 
 from omuchatprovider.helper import get_session
 from omuchatprovider.services import FetchedRoom, ProviderService
 
 from .chat import YoutubeChatService
-from .const import PROVIDER, REACTION_MESSAGE_TYPE, YOUTUBE_IDENTIFIER
+from .const import (
+    PROVIDER,
+    REACTION_PERMISSION_TYPE,
+    REACTION_SIGNAL_TYPE,
+    YOUTUBE_IDENTIFIER,
+)
 from .youtubeapi import YoutubeAPI
 
 
 class YoutubeService(ProviderService):
     def __init__(self, client: Client):
         self.client = client
         self.session = get_session(PROVIDER)
         self.extractor = YoutubeAPI(client, self.session)
-        self.reaction_message = client.message.get(REACTION_MESSAGE_TYPE)
+        self.reaction_signal = client.signal.get(REACTION_SIGNAL_TYPE)
+        client.permissions.register(REACTION_PERMISSION_TYPE)
 
     @property
     def provider(self) -> Provider:
         return PROVIDER
 
-    async def fetch_rooms(self, channel: Channel) -> List[FetchedRoom]:
+    async def fetch_rooms(self, channel: Channel) -> list[FetchedRoom]:
         videos = await self.extractor.fetch_online_videos(channel.url)
-        rooms: List[FetchedRoom] = []
+        rooms: list[FetchedRoom] = []
         for video_id in videos:
             room = Room(
                 provider_id=YOUTUBE_IDENTIFIER,
                 id=YOUTUBE_IDENTIFIER / video_id,
                 connected=False,
                 status="offline",
                 channel_id=channel.key(),
             )
+
+            def create(room=room):
+                return YoutubeChatService.create(self, self.client, room)
+
             rooms.append(
                 FetchedRoom(
                     room=room,
-                    create=lambda: YoutubeChatService.create(self, self.client, room),
+                    create=create,
                 )
             )
         return rooms
 
     async def is_online(self, room: Room) -> bool:
         return await self.extractor.is_online(video_id=room.id.path[-1])
```

### Comparing `omuchatprovider-0.2.5/src/omuchatprovider/services/youtube/youtubeapi.py` & `omuchatprovider-0.3.0/src/omuchatprovider/services/youtube/youtubeapi.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
 
 import json
 import re
 from datetime import timedelta
-from typing import Any, Dict, List
+from typing import Any
 
 import aiohttp
 import bs4
 from omuchat.client import Client
 
 from omuchatprovider.errors import ProviderError
 from omuchatprovider.helper import assert_none
@@ -72,25 +72,25 @@
         self.client = client
         self.session = session
         self.throttle = Throttle(timedelta(seconds=1 / 3))
 
     async def get(
         self,
         url: str,
-        params: Dict[str, str] | None = None,
+        params: dict[str, str] | None = None,
     ) -> YoutubePage:
         async with self.throttle:
             response = await self.session.get(
                 url,
                 params=params,
                 headers=BASE_HEADERS,
             )
         return await YoutubePage.from_response(response)
 
-    async def fetch_online_videos(self, url: str) -> List[str]:
+    async def fetch_online_videos(self, url: str) -> list[str]:
         match = assert_none(
             re.search(YOUTUBE_REGEX, url),
             "Could not match url",
         )
         options = match.groupdict()
 
         video_id = options.get("video_id") or options.get("video_id_short")
@@ -171,15 +171,15 @@
         continuation: str | None = None,
     ) -> types.live_chat:
         url = f"{YOUTUBE_URL}/youtubei/v1/live_chat/get_live_chat"
         params = {
             "v": video_id,
             "key": key,
         }
-        payload: Dict[str, Any] = {
+        payload: dict[str, Any] = {
             **BASE_PAYLOAD,
         }
         if continuation:
             payload["continuation"] = continuation
         async with self.throttle:
             response = await self.session.post(
                 url,
@@ -196,15 +196,15 @@
         key: str,
         continuation: str | None = None,
     ) -> types.updated_metadata:
         url = f"{YOUTUBE_URL}/youtubei/v1/updated_metadata"
         params = {
             "key": key,
         }
-        payload: Dict[str, Any] = {
+        payload: dict[str, Any] = {
             **BASE_PAYLOAD,
         }
         if continuation is not None:
             payload["continuation"] = continuation
         elif video_id is not None:
             payload["videoId"] = video_id
         else:
```

### Comparing `omuchatprovider-0.2.5/src/omuchatprovider/services/youtube/types/chatactions.py` & `omuchatprovider-0.3.0/src/omuchatprovider/services/youtube/types/chatactions.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import List, Literal, NotRequired, TypedDict
+from typing import Literal, NotRequired, TypedDict
 
 from .accessibility import Accessibility
 from .image import Image, Thumbnails
 from .runs import Runs
 from .simpletext import SimpleText
 from .urlendpoint import ContextMenuEndpoint
 
@@ -27,15 +27,15 @@
 
 
 class Source(TypedDict):
     clientResource: ClientResource
 
 
 class Sources(TypedDict):
-    sources: List[Source]
+    sources: list[Source]
 
 
 class ImageTint(TypedDict):
     color: int
 
 
 class BorderImageProcessor(TypedDict):
@@ -43,15 +43,15 @@
 
 
 class Processor(TypedDict):
     bprderImageProcessor: BorderImageProcessor
 
 
 class UnheartedIcon(TypedDict):
-    sources: List[Source]
+    sources: list[Source]
     processor: Processor
 
 
 class CreatorHeartViewModel(TypedDict):
     creatorThumbnail: Thumbnails
     heartedIcon: Sources
     unheartedIcon: UnheartedIcon
@@ -65,24 +65,21 @@
     creatorHeartViewModel: CreatorHeartViewModel
 
 
 class LiveChatRenderer(TypedDict):
     id: str
     timestampUsec: str
     authorExternalChannelId: str
-    # authorName: SimpleText
-    # authorPhoto: Thumbnails
-    # authorBadges: NotRequired[List[AuthorBadge]]
     message: Runs
 
 
 class AuthorInfo(TypedDict):
     authorName: SimpleText
     authorPhoto: Thumbnails
-    authorBadges: NotRequired[List[AuthorBadge]]
+    authorBadges: NotRequired[list[AuthorBadge]]
 
 
 class LiveChatTextMessageRenderer(LiveChatRenderer, AuthorInfo):
     contextMenuEndpoint: ContextMenuEndpoint
     contextMenuAccessibility: Accessibility
 
 
@@ -264,12 +261,13 @@
 class AddLiveChatTickerItemAction(TypedDict):
     item: AddLiveChatTickerItemActionItem
 
 
 class ChatActionsItem(TypedDict):
     clickTrackingParams: str
     addChatItemAction: NotRequired[AddChatItemAction]
+    removeChatItemByAuthorAction: NotRequired[dict]
     markChatItemAsDeletedAction: NotRequired[MarkChatItemAsDeletedAction]
     addLiveChatTickerItemAction: NotRequired[AddLiveChatTickerItemAction]
 
 
-type ChatActions = List[ChatActionsItem]
+type ChatActions = list[ChatActionsItem]
```

### Comparing `omuchatprovider-0.2.5/src/omuchatprovider/services/youtube/types/contents.py` & `omuchatprovider-0.3.0/src/omuchatprovider/services/youtube/types/contents.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import List, TypedDict
+from typing import TypedDict
 
 from .chatactions import ChatActions
 
 
 class InvalidationId(TypedDict):
     objectSource: int
     objectId: str
@@ -18,15 +18,15 @@
     clickTrackingParams: str
 
 
 class ContinuationItem(TypedDict):
     invalidationContinuationData: InvalidationContinuationData
 
 
-type Continuations = List[ContinuationItem]
+type Continuations = list[ContinuationItem]
 
 
 class LiveChatRenderer(TypedDict):
     continuations: Continuations
     actions: ChatActions
```

### Comparing `omuchatprovider-0.2.5/src/omuchatprovider/services/youtube/types/continuations.py` & `omuchatprovider-0.3.0/src/omuchatprovider/services/youtube/types/continuations.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import List, TypedDict
+from typing import TypedDict
 
 
 class InvalidationId(TypedDict):
     objectSource: int
     objectId: str
     topic: str
     subscribeToGcmTopics: bool
@@ -16,15 +16,15 @@
     clickTrackingParams: str
 
 
 class ContinuationsItem(TypedDict):
     invalidationContinuationData: InvalidationContinuationData
 
 
-type Continuations = List[ContinuationsItem]
+type Continuations = list[ContinuationsItem]
 
 
 class TimedContinuationData(TypedDict):
     timeoutMs: int
     continuation: str
```

### Comparing `omuchatprovider-0.2.5/src/omuchatprovider/services/youtube/types/frameworkupdates.py` & `omuchatprovider-0.3.0/src/omuchatprovider/services/youtube/types/frameworkupdates.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import List, Literal, NotRequired, TypedDict
+from typing import Literal, NotRequired, TypedDict
 
 
 class Content(TypedDict):
     content: str
 
 
 class LikeCountEntity1(TypedDict):
@@ -50,15 +50,15 @@
 
 class ReactionBucketsItem(TypedDict):
     totalReactions: int
     duration: Duration
     intensityScore: int
 
 
-type ReactionBuckets = List[ReactionBucketsItem]
+type ReactionBuckets = list[ReactionBucketsItem]
 
 
 class EmojiFountainDataEntity(TypedDict):
     key: str
     reactionBuckets: ReactionBuckets
     updateTimeUsec: str
 
@@ -83,15 +83,15 @@
         LikeCountEntityPayload
         | EngagementToolbarStateEntityPayloadPayload
         | EmojiFountainDataEntityPayload
         | BooleanEntityPayload
     )
 
 
-type Mutations = List[Mutation]
+type Mutations = list[Mutation]
 
 
 class Timestamp(TypedDict):
     seconds: str
     nanos: int
```

### Comparing `omuchatprovider-0.2.5/src/omuchatprovider/services/youtube/types/metadataactions.py` & `omuchatprovider-0.3.0/src/omuchatprovider/services/youtube/types/metadataactions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import List, NotRequired, TypedDict
+from typing import NotRequired, TypedDict
 
 from .chatactions import SimpleText
 from .runs import Runs
 
 
 class VideoViewCountRenderer(TypedDict):
     viewCount: SimpleText
@@ -35,8 +35,8 @@
 class MetadataActionsItem(TypedDict):
     updateViewershipAction: NotRequired[UpdateViewershipAction]
     updateDateTextAction: NotRequired[UpdateDateTextAction]
     updateTitleAction: NotRequired[UpdateTitleAction]
     updateDescriptionAction: NotRequired[UpdateDescriptionAction]
 
 
-type MetadataActions = List[MetadataActionsItem]
+type MetadataActions = list[MetadataActionsItem]
```

### Comparing `omuchatprovider-0.2.5/src/omuchatprovider/services/youtube/types/runs.py` & `omuchatprovider-0.3.0/src/omuchatprovider/services/youtube/types/runs.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-from typing import List, NotRequired, TypedDict, Union
+from typing import NotRequired, TypedDict
 
 from .image import Image
 from .urlendpoint import NavigationEndpoint
 
 
 class Emoji(TypedDict):
     emojiId: str
-    shortcuts: List[str]
-    searchTerms: List[str]
+    shortcuts: list[str]
+    searchTerms: list[str]
     image: Image
     isCustomEmoji: bool
 
 
 class TextRun(TypedDict):
     text: str
 
@@ -40,12 +40,12 @@
     navigationEndpoint: NotRequired[NavigationEndpoint]
 
 
 class EmojiRun(TypedDict):
     emoji: Emoji
 
 
-type RunsItem = Union[TextRun, LinkRun, EmojiRun]
+type RunsItem = TextRun | LinkRun | EmojiRun
 
 
 class Runs(TypedDict):
-    runs: List[RunsItem]
+    runs: list[RunsItem]
```

### Comparing `omuchatprovider-0.2.5/src/omuchatprovider/services/youtube/types/urlendpoint.py` & `omuchatprovider-0.3.0/src/omuchatprovider/services/youtube/types/urlendpoint.py`

 * *Files identical despite different names*

### Comparing `omuchatprovider-0.2.5/src/omuchatprovider/services/youtube/types/ytcfg.py` & `omuchatprovider-0.3.0/src/omuchatprovider/services/youtube/types/ytcfg.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from __future__ import annotations
 
-from typing import List, TypedDict
+from typing import TypedDict
 
 
 class ExperimentFlags(TypedDict):
     H5_enable_full_pacf_logging: bool
     H5_use_async_logging: bool
     PremiumClientSharedConfig__enable_att_context_processor: bool
     PremiumClientSharedConfig__enable_att_for_get_premium_on_web_client: bool
@@ -863,21 +863,21 @@
     web_client_version_override: str
     web_home_feed_reload_experience: str
     web_modern_subscribe_style: str
     web_shorts_expanded_overlay_type: str
     web_shorts_overlay_vertical_orientation: str
     yoodle_base_url: str
     yoodle_webp_base_url: str
-    conditional_lab_ids: List[int]
-    guide_business_info_countries: List[str]
-    guide_legal_footer_enabled_countries: List[str]
-    html5_profiler_trace_enums: List
-    kevlar_command_handler_command_banlist: List
-    kevlar_page_service_url_prefix_carveouts: List
-    web_op_signal_type_banlist: List
+    conditional_lab_ids: list[int]
+    guide_business_info_countries: list[str]
+    guide_legal_footer_enabled_countries: list[str]
+    html5_profiler_trace_enums: list
+    kevlar_command_handler_command_banlist: list
+    kevlar_page_service_url_prefix_carveouts: list
+    web_op_signal_type_banlist: list
 
 
 class GoogleFeedbackProductData(TypedDict):
     polymer: str
     polymer2: str
     accept_language: str
 
@@ -915,15 +915,15 @@
 
 class ConsistencytokenjarsItem(TypedDict):
     encryptedTokenJarContents: str
 
 
 class Request(TypedDict):
     useSsl: bool
-    consistencyTokenJars: List[ConsistencytokenjarsItem]
+    consistencyTokenJars: list[ConsistencytokenjarsItem]
 
 
 class Clicktracking(TypedDict):
     clickTrackingParams: str
 
 
 class InnertubeContext(TypedDict):
@@ -993,10 +993,10 @@
     SERIALIZED_CLIENT_CONFIG_DATA: str
     LIVE_CHAT_BASE_TANGO_CONFIG: LiveChatBaseTangoConfig
     LIVE_CHAT_SEND_MESSAGE_ACTION: str
     CLIENT_PROTOCOL: str
     CLIENT_TRANSPORT: str
     TIME_CREATED_MS: int
     LOGIN_INFO: str
-    VALID_SESSION_TEMPDATA_DOMAINS: List[str]
+    VALID_SESSION_TEMPDATA_DOMAINS: list[str]
     LIVE_CHAT_ALLOW_DARK_MODE: bool
     POST_TO_PARENT_DOMAIN: str
```

### Comparing `omuchatprovider-0.2.5/pyproject.toml` & `omuchatprovider-0.3.0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 [project]
 name = "omuchatprovider"
-version = "0.2.5"
+version = "0.3.0"
 description = "Add your description here"
 authors = [
     { name = "am230", email = "111672334+am230@users.noreply.github.com" },
 ]
 dependencies = [
+    "loguru>=0.7.2",
     "aiohttp>=3.9.1",
     "beautifulsoup4>=4.12.2",
     "lxml>=5.0.0",
-    "iwashi>=2.2.0",
-    "loguru>=0.7.2",
     "omuchat>=0.1.9",
 ]
 readme = "README.md"
 requires-python = ">= 3.12"
 
 [project.entry-points."omu.plugins"]
 plugin = "omuchatprovider:plugin"
@@ -23,16 +22,9 @@
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [tool.rye]
 managed = true
 dev-dependencies = []
 
-[tool.pylint]
-disable = [
-    "missing-module-docstring",
-    "missing-function-docstring",
-    "missing-class-docstring",
-]
-
 [tool.hatch.metadata]
 allow-direct-references = true
```

