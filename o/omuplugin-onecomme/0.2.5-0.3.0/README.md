# Comparing `tmp/omuplugin_onecomme-0.2.5.tar.gz` & `tmp/omuplugin_onecomme-0.3.0.tar.gz`

## Comparing `omuplugin_onecomme-0.2.5.tar` & `omuplugin_onecomme-0.3.0.tar`

### file list

```diff
@@ -1,6 +1,8 @@
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 omuplugin_onecomme-0.2.5/src/omuplugin_onecomme/__init__.py
--rw-r--r--   0        0        0     5934 2020-02-02 00:00:00.000000 omuplugin_onecomme-0.2.5/src/omuplugin_onecomme/plugin.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 omuplugin_onecomme-0.2.5/.gitignore
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 omuplugin_onecomme-0.2.5/README.md
--rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 omuplugin_onecomme-0.2.5/pyproject.toml
--rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 omuplugin_onecomme-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 omuplugin_onecomme-0.3.0/src/omuplugin_onecomme/__init__.py
+-rw-r--r--   0        0        0      904 2020-02-02 00:00:00.000000 omuplugin_onecomme-0.3.0/src/omuplugin_onecomme/onecomme.py
+-rw-r--r--   0        0        0     5524 2020-02-02 00:00:00.000000 omuplugin_onecomme-0.3.0/src/omuplugin_onecomme/plugin.py
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 omuplugin_onecomme-0.3.0/src/omuplugin_onecomme/version.py
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 omuplugin_onecomme-0.3.0/.gitignore
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 omuplugin_onecomme-0.3.0/README.md
+-rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 omuplugin_onecomme-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 omuplugin_onecomme-0.3.0/PKG-INFO
```

### Comparing `omuplugin_onecomme-0.2.5/src/omuplugin_onecomme/plugin.py` & `omuplugin_onecomme-0.3.0/src/omuplugin_onecomme/plugin.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,107 +1,63 @@
 from __future__ import annotations
 
 import asyncio
-from typing import Dict, List, Set, TypedDict
+from html import escape
+from typing import TypedDict
 
 from aiohttp import web
 from loguru import logger
-from omu.identifier import Identifier
 from omuchat import App, Client, events, model
+from omuchat.model import content
+
+from .onecomme import Badge, Comment, CommentData, CommentServiceData
 
-IDENTIFIER = Identifier("cc.omuchat", "plugin-onesync")
 APP = App(
-    IDENTIFIER,
+    "cc.omuchat:onecomme/plugin",
     version="0.1.0",
 )
 client = Client(APP)
 app = web.Application()
 
 
-class Color(TypedDict):
-    r: int
-    g: int
-    b: int
-
-
-class Badge(TypedDict):
-    label: str
-    url: str
-
-
-class CommentData(TypedDict):
-    id: str
-    liveId: str
-    userId: str
-    name: str
-    screenName: str
-    hasGift: bool
-    isOwner: bool
-    isAnonymous: bool
-    profileImage: str
-    badges: List[Badge]
-    timestamp: str
-    comment: str
-    displayName: str
-    originalProfileImage: str
-    isFirstTime: bool
-
-
-class CommentMeta(TypedDict):
-    no: int
-    tc: int
-
-
-class CommentServiceData(TypedDict):
-    id: str
-    name: str
-    url: str
-    write: bool
-    speech: bool
-    options: Dict
-    enabled: bool
-    persist: bool
-    translate: List
-    color: Color
-
-
-class Comment(TypedDict):
-    id: str
-    service: str
-    name: str
-    url: str
-    color: Color
-    data: CommentData
-    meta: CommentMeta
-    serviceData: CommentServiceData
-
-
-def format_content(*components: model.content.Component | None) -> str:
-    if not components:
+def format_content(*components: content.Component | None) -> str:
+    if components is None:
+        return ""
+    if len(components) == 0:
         return ""
     parts = []
     stack = [*components]
     while stack:
         component = stack.pop(0)
-        if isinstance(component, model.content.Text):
-            parts.append(component.text)
-        elif isinstance(component, model.content.Image):
-            parts.append(f'<img src="{component.url}" alt="{component.id}" />')
-        elif isinstance(component, model.content.Link):
+        if isinstance(component, content.Text):
+            parts.append(escape(component.text))
+        elif isinstance(component, content.Image):
+            parts.append(
+                f'<img src="{escape(component.url)}" alt="{escape(component.id)}">'
+            )
+        elif isinstance(component, content.Link):
             parts.append(
                 f'<a href="{component.url}">{format_content(*component.children)}</a>'
             )
-        elif isinstance(component, model.content.Parent):
-            stack.extend(component.get_children())
+        elif isinstance(component, content.System):
+            parts.append(
+                f"<div><span>{format_content(*component.get_children())}</span></div>"
+            )
+        elif isinstance(component, content.Parent):
+            parts.append(f"<span>{format_content(*component.get_children())}</span>")
+        else:
+            raise ValueError(f"Unknown component type: {component}")
     return "".join(parts)
 
 
 async def to_comment(message: model.Message) -> Comment | None:
-    room = await client.chat.rooms.get(message.room_id)
-    author = message.author_id and await client.chat.authors.get(message.author_id)
+    room = await client.chat.rooms.get(message.room_id.key())
+    author: model.Author | None = None
+    if message.author_id:
+        author = await client.chat.authors.get(message.author_id.key())
     if not room or not author:
         return None
     metadata = room.metadata or {}
     badges = []
     for badge in author.roles:
         if badge.icon_url:
             badges.append(
@@ -146,18 +102,18 @@
             translate=[],
             color={"r": 190, "g": 44, "b": 255},
         ),
     )
 
 
 class CommentsData(TypedDict):
-    comments: List[Comment]
+    comments: list[Comment]
 
 
-sessions: Set[web.WebSocketResponse] = set()
+sessions: set[web.WebSocketResponse] = set()
 
 
 async def handle(request: web.Request) -> web.WebSocketResponse:
     ws = web.WebSocketResponse()
     await ws.prepare(request)
     messages = [
         await to_comment(message)
```

### Comparing `omuplugin_onecomme-0.2.5/pyproject.toml` & `omuplugin_onecomme-0.3.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [project]
 name = "omuplugin_onecomme"
-version = "0.2.5"
+version = "0.3.0"
 description = "Add your description here"
 authors = [
     { name = "am230", email = "111672334+am230@users.noreply.github.com" },
 ]
-dependencies = ["omuchat>=0.1.9"]
+dependencies = ["loguru>=0.7.2", "omuchat>=0.1.9"]
 readme = "README.md"
 requires-python = ">= 3.12"
 
 [project.entry-points."omu.plugins"]
 plugin = "omuplugin_onecomme:plugin"
 
 [build-system]
```

