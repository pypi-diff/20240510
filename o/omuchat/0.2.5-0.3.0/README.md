# Comparing `tmp/omuchat-0.2.5.tar.gz` & `tmp/omuchat-0.3.0.tar.gz`

## Comparing `omuchat-0.2.5.tar` & `omuchat-0.3.0.tar`

### file list

```diff
@@ -1,20 +1,23 @@
--rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 omuchat-0.2.5/src/omuchat/__init__.py
--rw-r--r--   0        0        0     1449 2020-02-02 00:00:00.000000 omuchat-0.2.5/src/omuchat/chat.py
--rw-r--r--   0        0        0     1133 2020-02-02 00:00:00.000000 omuchat-0.2.5/src/omuchat/client.py
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 omuchat-0.2.5/src/omuchat/event/__init__.py
--rw-r--r--   0        0        0     4129 2020-02-02 00:00:00.000000 omuchat-0.2.5/src/omuchat/event/event.py
--rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 omuchat-0.2.5/src/omuchat/event/event_types.py
--rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 omuchat-0.2.5/src/omuchat/model/__init__.py
--rw-r--r--   0        0        0     2106 2020-02-02 00:00:00.000000 omuchat-0.2.5/src/omuchat/model/author.py
--rw-r--r--   0        0        0     1571 2020-02-02 00:00:00.000000 omuchat-0.2.5/src/omuchat/model/channel.py
--rw-r--r--   0        0        0     6862 2020-02-02 00:00:00.000000 omuchat-0.2.5/src/omuchat/model/content.py
--rw-r--r--   0        0        0     1345 2020-02-02 00:00:00.000000 omuchat-0.2.5/src/omuchat/model/gift.py
--rw-r--r--   0        0        0     2345 2020-02-02 00:00:00.000000 omuchat-0.2.5/src/omuchat/model/message.py
--rw-r--r--   0        0        0      856 2020-02-02 00:00:00.000000 omuchat-0.2.5/src/omuchat/model/paid.py
--rw-r--r--   0        0        0     1546 2020-02-02 00:00:00.000000 omuchat-0.2.5/src/omuchat/model/provider.py
--rw-r--r--   0        0        0     1796 2020-02-02 00:00:00.000000 omuchat-0.2.5/src/omuchat/model/role.py
--rw-r--r--   0        0        0     2547 2020-02-02 00:00:00.000000 omuchat-0.2.5/src/omuchat/model/room.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 omuchat-0.2.5/.gitignore
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 omuchat-0.2.5/README.md
--rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 omuchat-0.2.5/pyproject.toml
--rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 omuchat-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 omuchat-0.3.0/src/omuchat/__init__.py
+-rw-r--r--   0        0        0     2473 2020-02-02 00:00:00.000000 omuchat-0.3.0/src/omuchat/chat.py
+-rw-r--r--   0        0        0      818 2020-02-02 00:00:00.000000 omuchat-0.3.0/src/omuchat/client.py
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 omuchat-0.3.0/src/omuchat/const.py
+-rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 omuchat-0.3.0/src/omuchat/permissions.py
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 omuchat-0.3.0/src/omuchat/version.py
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 omuchat-0.3.0/src/omuchat/event/__init__.py
+-rw-r--r--   0        0        0     3272 2020-02-02 00:00:00.000000 omuchat-0.3.0/src/omuchat/event/event.py
+-rw-r--r--   0        0        0      536 2020-02-02 00:00:00.000000 omuchat-0.3.0/src/omuchat/event/event_types.py
+-rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 omuchat-0.3.0/src/omuchat/model/__init__.py
+-rw-r--r--   0        0        0     2188 2020-02-02 00:00:00.000000 omuchat-0.3.0/src/omuchat/model/author.py
+-rw-r--r--   0        0        0     1658 2020-02-02 00:00:00.000000 omuchat-0.3.0/src/omuchat/model/channel.py
+-rw-r--r--   0        0        0     7442 2020-02-02 00:00:00.000000 omuchat-0.3.0/src/omuchat/model/content.py
+-rw-r--r--   0        0        0     1033 2020-02-02 00:00:00.000000 omuchat-0.3.0/src/omuchat/model/gift.py
+-rw-r--r--   0        0        0     2467 2020-02-02 00:00:00.000000 omuchat-0.3.0/src/omuchat/model/message.py
+-rw-r--r--   0        0        0      856 2020-02-02 00:00:00.000000 omuchat-0.3.0/src/omuchat/model/paid.py
+-rw-r--r--   0        0        0     1546 2020-02-02 00:00:00.000000 omuchat-0.3.0/src/omuchat/model/provider.py
+-rw-r--r--   0        0        0     1796 2020-02-02 00:00:00.000000 omuchat-0.3.0/src/omuchat/model/role.py
+-rw-r--r--   0        0        0     2574 2020-02-02 00:00:00.000000 omuchat-0.3.0/src/omuchat/model/room.py
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 omuchat-0.3.0/.gitignore
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 omuchat-0.3.0/README.md
+-rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 omuchat-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 omuchat-0.3.0/PKG-INFO
```

### Comparing `omuchat-0.2.5/src/omuchat/client.py` & `omuchat-0.3.0/src/omuchat/client.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,13 +1,12 @@
-from typing import Callable
+from collections.abc import Callable
 
 from omu import Address, App, OmuClient
 
-from omuchat.event import EventRegistry, EventSource
-from omuchat.event.event import EventHandler
+from omuchat.event import EventHandler, EventRegistry, EventSource
 
 from .chat import Chat
 
 
 class Client(OmuClient):
     def __init__(
         self,
@@ -26,16 +25,7 @@
         self, event: EventSource[P]
     ) -> Callable[[EventHandler[P]], EventHandler[P]]:
         def decorator(listener: EventHandler[P]) -> EventHandler[P]:
             self.event_registry.register(event, listener)
             return listener
 
         return decorator
-
-    def off[**P](
-        self, event: EventSource[P]
-    ) -> Callable[[EventHandler[P]], EventHandler[P]]:
-        def decorator(listener: EventHandler[P]) -> EventHandler[P]:
-            self.event_registry.unregister(event, listener)
-            return listener
-
-        return decorator
```

### Comparing `omuchat-0.2.5/src/omuchat/event/event.py` & `omuchat-0.3.0/src/omuchat/event/event.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,76 +1,67 @@
 from __future__ import annotations
 
+from collections.abc import Callable, Coroutine, Mapping
 from dataclasses import dataclass
-from typing import TYPE_CHECKING, Callable, Coroutine, Dict, Mapping
+from typing import TYPE_CHECKING
 
-from omu.event_emitter import EventEmitter
+from omu.event_emitter import EventEmitter, Unlisten
+from omu.extension.table import Table
 
 if TYPE_CHECKING:
-    from omu.extension.table import Table
-
     from omuchat.client import Client
 
 type EventHandler[**P] = Callable[P, Coroutine[None, None, None]]
 
 
 @dataclass(frozen=True)
 class EventSource[**P]:
-    subscribe: Callable[[EventHandler[P], Client], None]
-    unsubscribe: Callable[[EventHandler[P], Client], None]
+    listen: Callable[[EventHandler[P], Client], Unlisten]
 
 
 class ListenerEvent[**P](EventSource[P]):
     def __init__(self, get_listener: Callable[[Client], EventEmitter[P]]):
-        super().__init__(self._subscribe, self._unsubscribe)
+        super().__init__(self._subscribe)
         self.get_listener = get_listener
 
     def _subscribe(
         self,
         emit: EventHandler[P],
         client: Client,
     ):
         listener = self.get_listener(client)
-        listener += emit
-
-    def _unsubscribe(
-        self,
-        emit: EventHandler[P],
-        client: Client,
-    ):
-        listener = self.get_listener(client)
-        listener -= emit
+        return listener.listen(emit)
 
 
 class TableEvent[T](ListenerEvent[Mapping[str, T]]):
     def __init__(self, get_table: Callable[[Client], Table[T]]):
         self.get_table = get_table
         super().__init__(
-            lambda client: get_table(client).listeners.cache_update,
+            lambda client: get_table(client).event.cache_update,
         )
         self.add_batch = ListenerEvent(
-            lambda client: get_table(client).listeners.add,
+            lambda client: get_table(client).event.add,
         )
         self.update_batch = ListenerEvent(
-            lambda client: get_table(client).listeners.update,
+            lambda client: get_table(client).event.update,
         )
         self.remove_batch = ListenerEvent(
-            lambda client: get_table(client).listeners.remove,
+            lambda client: get_table(client).event.remove,
         )
         self.add = self._create_batch_subscriber(
-            lambda table: table.listeners.add,
+            lambda table: table.event.add,
         )
         self.update = self._create_batch_subscriber(
-            lambda table: table.listeners.update,
+            lambda table: table.event.update,
         )
         self.remove = self._create_batch_subscriber(
-            lambda table: table.listeners.remove,
+            lambda table: table.event.remove,
         )
         self.clear = ListenerEvent(
-            lambda client: get_table(client).listeners.clear,
+            lambda client: get_table(client).event.clear,
         )
         self.wrappers = {}
 
     @staticmethod
     def _create_batch_wrapper(emit: EventHandler[[T]]):
         async def wrapper(items: Mapping[str, T]):
             for item in items.values():
@@ -83,46 +74,32 @@
     ):
         batch_wrapper: EventHandler[Mapping[str, T]] | None = None
 
         def subscribe(emit: EventHandler[T], client: Client):
             listener = get_listener(self.get_table(client))
             nonlocal batch_wrapper
             batch_wrapper = self._create_batch_wrapper(emit)
-            listener += batch_wrapper
-
-        def unsubscribe(emit: EventHandler[T], client: Client):
-            if batch_wrapper is None:
-                raise ValueError("Listener not subscribed")
-            listener = get_listener(self.get_table(client))
-            listener -= batch_wrapper
+            return listener.listen(batch_wrapper)
 
-        return EventSource(subscribe, unsubscribe)
+        return EventSource(subscribe)
 
 
 @dataclass(frozen=True)
 class Entry[**P]:
     source: EventSource[P]
     listeners: EventEmitter[P]
 
 
 class EventRegistry:
     def __init__(self, client: Client):
         self.client = client
-        self.events: Dict[int, Entry] = {}
+        self.events: dict[int, Entry] = {}
 
-    def register[**P](self, event: EventSource[P], listener: EventHandler[P]):
+    def register[**P](
+        self, event: EventSource[P], listener: EventHandler[P]
+    ) -> Unlisten:
         event_id = id(event)
         if event_id not in self.events:
             entry = Entry[P](event, EventEmitter[P]())
-            event.subscribe(entry.listeners.emit, self.client)
+            event.listen(entry.listeners.emit, self.client)
             self.events[event_id] = entry  # type: ignore
-        self.events[event_id].listeners.subscribe(listener)
-
-    def unregister[**P](self, event: EventSource[P], listener: EventHandler[P]):
-        event_id = id(event)
-        if event_id not in self.events:
-            return
-        entry = self.events[event_id]
-        entry.listeners.unsubscribe(listener)
-        if entry.listeners.empty:
-            entry.source.unsubscribe(entry.listeners.emit, self.client)
-            del entry
+        return self.events[event_id].listeners.listen(listener)
```

### Comparing `omuchat-0.2.5/src/omuchat/event/event_types.py` & `omuchat-0.3.0/src/omuchat/event/event_types.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from omuchat.model import Author, Channel, Message, Provider, Room
 
 from .event import ListenerEvent, TableEvent
 
 
 class events:
-    ready = ListenerEvent(lambda client: client.listeners.ready)
+    ready = ListenerEvent(lambda client: client.event.ready)
     message = TableEvent[Message](lambda client: client.chat.messages)
     author = TableEvent[Author](lambda client: client.chat.authors)
     channel = TableEvent[Channel](lambda client: client.chat.channels)
     provider = TableEvent[Provider](lambda client: client.chat.providers)
     room = TableEvent[Room](lambda client: client.chat.rooms)
```

### Comparing `omuchat-0.2.5/src/omuchat/model/__init__.py` & `omuchat-0.3.0/src/omuchat/model/__init__.py`

 * *Files identical despite different names*

### Comparing `omuchat-0.2.5/src/omuchat/model/author.py` & `omuchat-0.3.0/src/omuchat/model/author.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,76 +1,77 @@
 from __future__ import annotations
 
-from typing import List, NotRequired, TypedDict
+from typing import NotRequired, TypedDict
 
 from omu.helper import map_optional
+from omu.identifier import Identifier
 from omu.interface import Keyable
 from omu.model import Model
 
 from .role import Role, RoleJson
 
 
 class AuthorMetadata(TypedDict):
     url: NotRequired[str | None]
     screen_id: NotRequired[str | None]
     avatar_url: NotRequired[str | None]
     description: NotRequired[str | None]
-    links: NotRequired[List[str] | None]
+    links: NotRequired[list[str] | None]
 
 
 class AuthorJson(TypedDict):
     provider_id: str
     id: str
     name: NotRequired[str] | None
     avatar_url: NotRequired[str] | None
-    roles: NotRequired[List[RoleJson]] | None
+    roles: NotRequired[list[RoleJson]] | None
     metadata: NotRequired[AuthorMetadata] | None
 
 
 class Author(Keyable, Model[AuthorJson]):
     def __init__(
         self,
         *,
-        provider_id: str,
-        id: str,
+        provider_id: Identifier,
+        id: Identifier,
         name: str | None = None,
         avatar_url: str | None = None,
-        roles: List[Role] | None = None,
+        roles: list[Role] | None = None,
         metadata: AuthorMetadata | None = None,
     ) -> None:
         self.provider_id = provider_id
         self.id = id
         self.name = name
         self.avatar_url = avatar_url
         self.roles = roles or []
         self.metadata = metadata
 
     def to_json(self) -> AuthorJson:
         return {
-            "provider_id": self.provider_id,
-            "id": self.id,
+            "provider_id": self.provider_id.key(),
+            "id": self.id.key(),
             "name": self.name,
             "avatar_url": self.avatar_url,
             "roles": [role.to_json() for role in self.roles],
             "metadata": self.metadata,
         }
 
     @classmethod
     def from_json(cls, json: AuthorJson) -> Author:
         return cls(
-            provider_id=json["provider_id"],
-            id=json["id"],
+            provider_id=Identifier.from_key(json["provider_id"]),
+            id=Identifier.from_key(json["id"]),
             name=json["name"],
             avatar_url=json.get("avatar_url"),
             roles=map_optional(
                 json.get("roles"),
                 lambda roles: list(map(Role.from_json, roles)),
                 [],
             ),
             metadata=json.get("metadata"),
         )
 
     def key(self) -> str:
-        return f"{self.provider_id}:{self.id}"
+        return self.id.key()
 
     def __str__(self) -> str:
         return f"Author(id={self.id}, name={self.name})"
```

### Comparing `omuchat-0.2.5/src/omuchat/model/channel.py` & `omuchat-0.3.0/src/omuchat/model/channel.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from __future__ import annotations
 
 from typing import TypedDict
 
+from omu.identifier import Identifier
 from omu.interface import Keyable
 from omu.model import Model
 
 
 class ChannelJson(TypedDict):
     provider_id: str
     id: str
@@ -16,16 +17,16 @@
     icon_url: str
 
 
 class Channel(Keyable, Model[ChannelJson]):
     def __init__(
         self,
         *,
-        provider_id: str,
-        id: str,
+        provider_id: Identifier,
+        id: Identifier,
         url: str,
         name: str,
         description: str,
         active: bool,
         icon_url: str,
     ) -> None:
         self.provider_id = provider_id
@@ -35,32 +36,32 @@
         self.description = description
         self.active = active
         self.icon_url = icon_url
 
     @classmethod
     def from_json(cls, json: ChannelJson) -> Channel:
         return cls(
-            provider_id=json["provider_id"],
-            id=json["id"],
+            provider_id=Identifier.from_key(json["provider_id"]),
+            id=Identifier.from_key(json["id"]),
             url=json["url"],
             name=json["name"],
             description=json["description"],
             active=json["active"],
             icon_url=json["icon_url"],
         )
 
     def to_json(self) -> ChannelJson:
         return ChannelJson(
-            provider_id=self.provider_id,
-            id=self.id,
+            provider_id=self.provider_id.key(),
+            id=self.id.key(),
             url=self.url,
             name=self.name,
             description=self.description,
             active=self.active,
             icon_url=self.icon_url,
         )
 
     def key(self) -> str:
-        return f"{self.provider_id}:{self.url}"
+        return self.id.key()
 
     def __repr__(self):
         return f"Channel({self.provider_id}, {self.url}, {self.name})"
```

### Comparing `omuchat-0.2.5/src/omuchat/model/content.py` & `omuchat-0.3.0/src/omuchat/model/content.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 from __future__ import annotations
 
 import abc
+from collections.abc import Callable, Iterable
 from typing import (
-    Callable,
-    Iterable,
-    List,
     Literal,
     LiteralString,
     Protocol,
+    Self,
     TypedDict,
 )
 
 type Primitive = dict[str | int, Primitive] | list | str | int | float | bool | None
 
 
 class ComponentJson(TypedDict):
@@ -27,41 +26,44 @@
     @staticmethod
     @abc.abstractmethod
     def from_json(json: D) -> Component: ...
 
     @abc.abstractmethod
     def to_json(self) -> D: ...
 
+    @abc.abstractmethod
+    def copy(self) -> Self: ...
+
     def walk(self, cb: Callable[[Component], None]) -> None:
-        stack: List[Component] = [self]
+        stack: list[Component] = [self]
         while stack:
             component = stack.pop()
             if not component:
                 continue
             cb(component)
             if isinstance(component, Parent):
                 stack.extend(component.get_children())
 
     def iter(self) -> Iterable[Component]:
-        stack: List[Component] = [self]
+        stack: list[Component] = [self]
         while stack:
             component = stack.pop()
             if not component:
                 continue
             yield component
             if isinstance(component, Parent):
                 stack.extend(component.get_children())
 
 
 class Parent(abc.ABC):
     @abc.abstractmethod
-    def get_children(self) -> List[Component]: ...
+    def get_children(self) -> list[Component]: ...
 
     @abc.abstractmethod
-    def set_children(self, children: List[Component]) -> None: ...
+    def set_children(self, children: list[Component]) -> None: ...
 
 
 class ComponentType[D, C: Component](Protocol):
     @classmethod
     def type(cls) -> str: ...
 
     @staticmethod
@@ -90,36 +92,39 @@
 ):
     type = component_type.type()
     if type in component_types:
         raise ValueError(f"Component type already registered: {type}")
     component_types[type] = component_type
 
 
-type RootData = List[ComponentJson]
+type RootData = list[ComponentJson]
 
 
 class Root(Component[Literal["root"], RootData], Parent):
-    def __init__(self, children: List[Component] | None = None):
+    def __init__(self, children: list[Component] | None = None):
         self.children = children or []
 
     @classmethod
     def type(cls):
         return "root"
 
     @staticmethod
     def from_json(json: RootData) -> Root:
         return Root([deserialize(child) for child in json])
 
     def to_json(self) -> RootData:
         return [serialize(child) for child in self.children]
 
-    def get_children(self) -> List[Component]:
+    def copy(self) -> Root:
+        return Root([child.copy() for child in self.children])
+
+    def get_children(self) -> list[Component]:
         return self.children
 
-    def set_children(self, children: List[Component]) -> None:
+    def set_children(self, children: list[Component]) -> None:
         self.children = children
 
     def add(self, component: Component):
         if not self.children:
             self.children = []
         self.children.append(component)
 
@@ -145,14 +150,17 @@
     @staticmethod
     def from_json(json: TextData) -> Text:
         return Text(json)
 
     def to_json(self) -> TextData:
         return self.text
 
+    def copy(self) -> Text:
+        return Text(self.text)
+
     @classmethod
     def of(cls, text: str) -> Text:
         return cls(text)
 
 
 class ImageData(TypedDict):
     url: str
@@ -177,26 +185,29 @@
     def to_json(self) -> ImageData:
         return {
             "url": self.url,
             "id": self.id,
             "name": self.name,
         }
 
+    def copy(self) -> Image:
+        return Image(self.url, self.id, self.name)
+
     @classmethod
     def of(cls, *, url: str, id: str, name: str | None = None) -> Image:
         return cls(url, id, name)
 
 
 class LinkData(TypedDict):
     url: str
-    children: List[ComponentJson]
+    children: list[ComponentJson]
 
 
 class Link(Component[Literal["link"], LinkData], Parent):
-    def __init__(self, url: str, children: List[Component]):
+    def __init__(self, url: str, children: list[Component]):
         self.url = url
         self.children = children
 
     @classmethod
     def type(cls):
         return "link"
 
@@ -210,23 +221,26 @@
 
     def to_json(self) -> LinkData:
         return {
             "url": self.url,
             "children": [serialize(child) for child in self.children],
         }
 
-    def get_children(self) -> List[Component]:
+    def copy(self) -> Link:
+        return Link(self.url, [child.copy() for child in self.children])
+
+    def get_children(self) -> list[Component]:
         return self.children
 
-    def set_children(self, children: List[Component]) -> None:
+    def set_children(self, children: list[Component]) -> None:
         self.children = children
 
 
 class System(Component[Literal["system"], RootData], Parent):
-    def __init__(self, children: List[Component]):
+    def __init__(self, children: list[Component]):
         self.children = children
 
     @classmethod
     def type(cls):
         return "system"
 
     @classmethod
@@ -236,18 +250,21 @@
     @staticmethod
     def from_json(json: RootData) -> System:
         return System([deserialize(child) for child in json])
 
     def to_json(self) -> RootData:
         return [serialize(child) for child in self.children]
 
-    def get_children(self) -> List[Component]:
+    def copy(self) -> System:
+        return System([child.copy() for child in self.children])
+
+    def get_children(self) -> list[Component]:
         return self.children
 
-    def set_children(self, children: List[Component]) -> None:
+    def set_children(self, children: list[Component]) -> None:
         self.children = children
 
 
 type LogLevel = Literal["info", "warning", "error"]
 
 
 class LogData(TypedDict):
@@ -274,10 +291,13 @@
 
     def to_json(self) -> LogData:
         return {
             "level": self.level,
             "message": self.message,
         }
 
+    def copy(self) -> Log:
+        return Log(self.level, self.message)
+
 
 for component_type in {Root, Text, Image, Link, System, Log}:
     register(component_type)
```

### Comparing `omuchat-0.2.5/src/omuchat/model/gift.py` & `omuchat-0.3.0/src/omuchat/model/gift.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,37 +1,30 @@
 from __future__ import annotations
 
+from dataclasses import dataclass
 from typing import NotRequired, TypedDict
 
 from omu.model import Model
 
 
 class GiftJson(TypedDict):
     id: str
     name: NotRequired[str] | None
     amount: NotRequired[int] | None
     is_paid: NotRequired[bool] | None
     image_url: NotRequired[str] | None
 
 
+@dataclass
 class Gift(Model[GiftJson]):
-    def __init__(
-        self,
-        *,
-        id: str,
-        name: str | None = None,
-        amount: int | None = None,
-        is_paid: bool | None = None,
-        image_url: str | None = None,
-    ) -> None:
-        self.id = id
-        self.name = name
-        self.amount = amount
-        self.is_paid = is_paid
-        self.image_url = image_url
+    id: str
+    name: str | None = None
+    amount: int | None = None
+    is_paid: bool | None = None
+    image_url: str | None = None
 
     @classmethod
     def from_json(cls, json: GiftJson) -> Gift:
         return cls(
             id=json["id"],
             name=json["name"],
             amount=json["amount"],
@@ -43,10 +36,7 @@
         return {
             "id": self.id,
             "name": self.name,
             "amount": self.amount,
             "is_paid": self.is_paid,
             "image_url": self.image_url,
         }
-
-    def __repr__(self) -> str:
-        return f"Gift(id={self.id}, name={self.name}, amount={self.amount}, is_paid={self.is_paid})"
```

### Comparing `omuchat-0.2.5/src/omuchat/model/message.py` & `omuchat-0.3.0/src/omuchat/model/message.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import annotations
 
 from dataclasses import dataclass
 from datetime import datetime
-from typing import List, NotRequired, TypedDict
+from typing import NotRequired, TypedDict
 
 from omu.helper import map_optional
 from omu.identifier import Identifier
 from omu.interface import Keyable
 from omu.model import Model
 
 from . import content
@@ -16,57 +16,59 @@
 
 class MessageJson(TypedDict):
     room_id: str
     id: str
     author_id: NotRequired[str] | None
     content: NotRequired[content.ComponentJson] | None
     paid: NotRequired[PaidJson] | None
-    gifts: NotRequired[List[GiftJson]] | None
+    gifts: NotRequired[list[GiftJson]] | None
     created_at: NotRequired[str] | None  # ISO 8601 date string
 
 
 @dataclass
 class Message(Keyable, Model[MessageJson]):
-    room_id: str
+    room_id: Identifier
     id: Identifier
-    author_id: str | None = None
+    author_id: Identifier | None = None
     content: content.Component | None = None
     paid: Paid | None = None
-    gifts: List[Gift] | None = None
+    gifts: list[Gift] | None = None
     created_at: datetime | None = None
 
     @classmethod
     def from_json(cls, json: MessageJson) -> Message:
         created_at = None
         if json.get("created_at") and json["created_at"]:
             created_at = datetime.fromisoformat(json["created_at"])
 
         return cls(
-            room_id=json["room_id"],
+            room_id=Identifier.from_key(json["room_id"]),
             id=Identifier.from_key(json["id"]),
-            author_id=json.get("author_id"),
+            author_id=map_optional(json.get("author_id"), Identifier.from_key),
             content=map_optional(json.get("content"), content.deserialize),
             paid=map_optional(json.get("paid"), Paid.from_json),
             gifts=map_optional(
                 json.get("gifts"),
                 lambda gifts: list(map(Gift.from_json, gifts)),
                 [],
             ),
             created_at=created_at,
         )
 
     def to_json(self) -> MessageJson:
         return MessageJson(
-            room_id=self.room_id,
+            room_id=self.room_id.key(),
             id=self.id.key(),
-            author_id=self.author_id,
-            content=content.serialize(self.content) if self.content else None,
-            paid=self.paid.to_json() if self.paid else None,
-            gifts=[gift.to_json() for gift in self.gifts] if self.gifts else None,
-            created_at=self.created_at.isoformat() if self.created_at else None,
+            author_id=map_optional(self.author_id, Identifier.key),
+            content=map_optional(self.content, content.serialize),
+            paid=map_optional(self.paid, Paid.to_json),
+            gifts=map_optional(
+                self.gifts, lambda gifts: [gift.to_json() for gift in gifts]
+            ),
+            created_at=map_optional(self.created_at, lambda x: x.isoformat()),
         )
 
     @property
     def text(self) -> str:
         if not self.content:
             return ""
         return str(self.content)
```

### Comparing `omuchat-0.2.5/src/omuchat/model/paid.py` & `omuchat-0.3.0/src/omuchat/model/paid.py`

 * *Files identical despite different names*

### Comparing `omuchat-0.2.5/src/omuchat/model/provider.py` & `omuchat-0.3.0/src/omuchat/model/provider.py`

 * *Files identical despite different names*

### Comparing `omuchat-0.2.5/src/omuchat/model/role.py` & `omuchat-0.3.0/src/omuchat/model/role.py`

 * *Files identical despite different names*

### Comparing `omuchat-0.2.5/src/omuchat/model/room.py` & `omuchat-0.3.0/src/omuchat/model/room.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from __future__ import annotations
 
+from collections.abc import Hashable
 from datetime import datetime
-from typing import Hashable, Literal, NotRequired, TypedDict
+from typing import Literal, NotRequired, TypedDict
 
 from omu.helper import map_optional
 from omu.identifier import Identifier
 from omu.interface import Keyable
 from omu.model import Model
```

