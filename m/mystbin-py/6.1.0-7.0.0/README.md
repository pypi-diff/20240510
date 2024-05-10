# Comparing `tmp/mystbin_py-6.1.0.tar.gz` & `tmp/mystbin_py-7.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mystbin_py-6.1.0.tar", max compression
+gzip compressed data, was "mystbin_py-7.0.0.tar", max compression
```

## Comparing `mystbin_py-6.1.0.tar` & `mystbin_py-7.0.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rwxr-xr-x   0        0        0     1063 2024-01-11 15:01:07.418935 mystbin_py-6.1.0/LICENSE
--rwxr-xr-x   0        0        0     2886 2024-01-11 15:01:07.418935 mystbin_py-6.1.0/README.md
--rwxr-xr-x   0        0        0     1529 2024-01-11 15:29:11.527262 mystbin_py-6.1.0/mystbin/__init__.py
--rwxr-xr-x   0        0        0     7413 2024-01-11 17:45:47.343961 mystbin_py-6.1.0/mystbin/client.py
--rwxr-xr-x   0        0        0     1749 2024-01-11 15:17:00.191674 mystbin_py-6.1.0/mystbin/errors.py
--rwxr-xr-x   0        0        0    10917 2024-01-11 17:45:47.343961 mystbin_py-6.1.0/mystbin/http.py
--rwxr-xr-x   0        0        0     4855 2024-01-11 15:27:28.490755 mystbin_py-6.1.0/mystbin/paste.py
--rwxr-xr-x   0        0        0        0 2024-01-11 15:01:07.418935 mystbin_py-6.1.0/mystbin/py.typed
--rwxr-xr-x   0        0        0     1149 2024-01-11 15:01:07.418935 mystbin_py-6.1.0/mystbin/types/__init__.py
--rwxr-xr-x   0        0        0     1752 2024-01-11 15:16:18.795467 mystbin_py-6.1.0/mystbin/types/responses.py
--rwxr-xr-x   0        0        0     2262 2024-01-11 15:07:31.576841 mystbin_py-6.1.0/mystbin/utils.py
--rwxr-xr-x   0        0        0     3046 2024-01-11 17:36:37.677329 mystbin_py-6.1.0/pyproject.toml
--rw-r--r--   0        0        0     4269 1970-01-01 00:00:00.000000 mystbin_py-6.1.0/PKG-INFO
+-rwxr-xr-x   0        0        0     1063 2024-01-11 15:01:07.418935 mystbin_py-7.0.0/LICENSE
+-rwxr-xr-x   0        0        0     2886 2024-01-11 15:01:07.418935 mystbin_py-7.0.0/README.md
+-rwxr-xr-x   0        0        0     1567 2024-05-10 18:34:33.796132 mystbin_py-7.0.0/mystbin/__init__.py
+-rwxr-xr-x   0        0        0     4384 2024-05-10 18:24:40.008954 mystbin_py-7.0.0/mystbin/client.py
+-rwxr-xr-x   0        0        0     1750 2024-05-10 18:36:14.572675 mystbin_py-7.0.0/mystbin/errors.py
+-rwxr-xr-x   0        0        0     9753 2024-05-10 18:33:49.139891 mystbin_py-7.0.0/mystbin/http.py
+-rwxr-xr-x   0        0        0     5239 2024-05-10 18:21:46.436019 mystbin_py-7.0.0/mystbin/paste.py
+-rwxr-xr-x   0        0        0        0 2024-01-11 15:01:07.418935 mystbin_py-7.0.0/mystbin/py.typed
+-rwxr-xr-x   0        0        0     1149 2024-01-11 15:01:07.418935 mystbin_py-7.0.0/mystbin/types/__init__.py
+-rwxr-xr-x   0        0        0     1663 2024-05-10 18:05:26.194657 mystbin_py-7.0.0/mystbin/types/responses.py
+-rw-r--r--   0        0        0     1451 2024-05-10 18:13:19.229246 mystbin_py-7.0.0/mystbin/utils.py
+-rwxr-xr-x   0        0        0     3154 2024-05-10 18:36:19.088700 mystbin_py-7.0.0/pyproject.toml
+-rw-r--r--   0        0        0     4269 1970-01-01 00:00:00.000000 mystbin_py-7.0.0/PKG-INFO
```

### Comparing `mystbin_py-6.1.0/LICENSE` & `mystbin_py-7.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mystbin_py-6.1.0/README.md` & `mystbin_py-7.0.0/README.md`

 * *Files identical despite different names*

### Comparing `mystbin_py-6.1.0/mystbin/__init__.py` & `mystbin_py-7.0.0/mystbin/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
 FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 DEALINGS IN THE SOFTWARE.
 """
 
-__version__ = "6.1.0"
+__version__ = "7.0.0"
 
 from typing import Literal, NamedTuple
 
 from .client import Client as Client
 from .errors import *
 from .paste import File as File, Paste as Paste
 
@@ -35,8 +35,10 @@
     major: int
     minor: int
     micro: int
     releaselevel: Literal["alpha", "beta", "candidate", "final"]
     serial: int
 
 
-version_info: VersionInfo = VersionInfo(major=6, minor=1, micro=0, releaselevel="final", serial=0)
+version_info: VersionInfo = VersionInfo(major=7, minor=0, micro=0, releaselevel="final", serial=0)
+
+del NamedTuple, Literal, VersionInfo
```

### Comparing `mystbin_py-6.1.0/mystbin/errors.py` & `mystbin_py-7.0.0/mystbin/errors.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
 FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 DEALINGS IN THE SOFTWARE.
 """
+
 from aiohttp import ClientResponse
 
 __all__ = (
     "APIException",
     "AuthenticationRequired",
 )
```

### Comparing `mystbin_py-6.1.0/mystbin/http.py` & `mystbin_py-7.0.0/mystbin/http.py`

 * *Files 14% similar despite different names*

```diff
@@ -39,26 +39,26 @@
 )
 from urllib.parse import quote as _uriquote
 
 import aiohttp
 
 from . import __version__
 from .errors import APIException
-from .utils import MISSING
 
 if TYPE_CHECKING:
     from types import TracebackType
 
     from . import File
 
     T = TypeVar("T")
     Response = Coroutine[None, None, T]
     MU = TypeVar("MU", bound="MaybeUnlock")
     BE = TypeVar("BE", bound=BaseException)
-    from .types.responses import EditPasteResponse, PasteResponse
+    from .types.responses import CreatePasteResponse, GetPasteResponse
+
 
 SupportedHTTPVerb = Literal["GET", "POST", "PUT", "DELETE", "PATCH"]
 
 LOGGER: logging.Logger = logging.getLogger(__name__)
 
 __all__ = ("HTTPClient",)
 
@@ -108,15 +108,15 @@
 class Route:
     __slots__ = (
         "verb",
         "path",
         "url",
     )
 
-    API_BASE: ClassVar[str] = "https://api.mystb.in"
+    API_BASE: ClassVar[str] = "https://mystb.in/api"
 
     def __init__(self, verb: SupportedHTTPVerb, path: str, **params: Any) -> None:
         self.verb: SupportedHTTPVerb = verb
         self.path: str = path
         url = self.API_BASE + path
         if params:
             url = url.format_map({k: _uriquote(v) if isinstance(v, str) else v for k, v in params.items()})
@@ -129,16 +129,15 @@
         "_owns_session",
         "_async",
         "_token",
         "_locks",
         "user_agent",
     )
 
-    def __init__(self, *, token: str | None, session: aiohttp.ClientSession | None = None) -> None:
-        self._token: str | None = token
+    def __init__(self, *, session: aiohttp.ClientSession | None = None) -> None:
         self._session: aiohttp.ClientSession | None = session
         self._owns_session: bool = False
         self._locks: weakref.WeakValueDictionary[str, asyncio.Lock] = weakref.WeakValueDictionary()
         user_agent = "mystbin.py (https://github.com/PythonistaGuild/mystbin.py {0}) Python/{1[0]}.{1[1]} aiohttp/{2}"
         self.user_agent: str = user_agent.format(__version__, sys.version_info, aiohttp.__version__)
 
     async def close(self) -> None:
@@ -157,17 +156,14 @@
         bucket = route.path
         lock = self._locks.get(bucket)
         if lock is None:
             lock = asyncio.Lock()
             self._locks[bucket] = lock
 
         headers = kwargs.pop("headers", {})
-
-        if self._token is not None:
-            headers["Authorization"] = f"Bearer {self._token}"
         headers["User-Agent"] = self.user_agent
 
         if "json" in kwargs:
             headers["Content-Type"] = "application/json"
             kwargs["data"] = json.dumps(kwargs.pop("json"), separators=(",", ":"), ensure_ascii=True)
             LOGGER.debug("Current json body is: %s", str(kwargs["data"]))
 
@@ -218,14 +214,15 @@
 
                         if response.status in {500, 502, 503, 504}:
                             sleep_ = 1 + tries * 2
                             LOGGER.warning("Hit an API error, trying again in: %d", sleep_)
                             await asyncio.sleep(sleep_)
                             continue
 
+                        print(data)
                         assert isinstance(data, dict)
                         LOGGER.exception("Unhandled HTTP error occurred: %s -> %s", response.status, data)
                         raise APIException(
                             response=response,
                             status_code=response.status,
                         )
                 except (aiohttp.ServerDisconnectedError, aiohttp.ServerTimeoutError) as error:
@@ -240,68 +237,34 @@
                 raise APIException(response=response, status_code=response.status)
 
             raise RuntimeError("Unreachable code in HTTP handling.")
 
     def create_paste(
         self,
         *,
-        file: File | None = None,
-        files: Sequence[File] | None = None,
+        files: Sequence[File],
         password: str | None,
         expires: datetime.datetime | None,
-    ) -> Response[PasteResponse]:
-        route = Route("PUT", "/paste")
+    ) -> Response[CreatePasteResponse]:
+        route = Route("POST", "/paste")
 
         json_: dict[str, Any] = {}
-        if file:
-            json_["files"] = [file.to_dict()]
-        elif files:
-            json_["files"] = [f.to_dict() for f in files]
+        headers: dict[str, Any] = {}
+        json_["files"] = [f.to_dict() for f in files]
 
         if password:
-            json_["password"] = password
+            headers["password"] = password
         if expires:
             json_["expires"] = _clean_dt(expires)
 
-        return self.request(route=route, json=json_)
+        return self.request(route=route, json=json_, headers=headers)
 
-    def delete_paste(self, *, paste_id: str) -> Response[None]:
-        return self.delete_pastes(paste_ids=[paste_id])
+    def delete_paste(self, security_token: str, /) -> Response[bool]:
+        route = Route("GET", "/security/delete/{security_token}", security_token=security_token)
+        return self.request(route)
 
-    def delete_pastes(self, *, paste_ids: Sequence[str]) -> Response[None]:
-        route = Route("DELETE", "/paste")
-        return self.request(route=route, json={"pastes": paste_ids})
-
-    def get_paste(self, *, paste_id: str, password: str | None) -> Response[PasteResponse]:
+    def get_paste(self, *, paste_id: str, password: str | None) -> Response[GetPasteResponse]:
         route = Route("GET", "/paste/{paste_id}", paste_id=paste_id)
 
         if password:
             return self.request(route=route, params={"password": password})
         return self.request(route=route)
-
-    def edit_paste(
-        self,
-        paste_id: str,
-        *,
-        new_content: str = MISSING,
-        new_filename: str = MISSING,
-        new_expires: datetime.datetime = MISSING,
-    ) -> Response[EditPasteResponse]:
-        route = Route("PATCH", "/paste/{paste_id}", paste_id=paste_id)
-
-        json_: dict[str, Any] = {}
-
-        if new_content is not MISSING:
-            json_["new_content"] = new_content
-
-        if new_filename is not MISSING:
-            json_["new_filename"] = new_filename
-
-        if new_expires is not MISSING:
-            json_["new_expires"] = _clean_dt(new_expires)
-
-        return self.request(route, json=json_)
-
-    def get_my_pastes(self, *, limit: int) -> Response[Sequence[PasteResponse]]:
-        route = Route("GET", "/pastes/@me")
-
-        return self.request(route, params={limit: limit})
```

### Comparing `mystbin_py-6.1.0/mystbin/paste.py` & `mystbin_py-7.0.0/mystbin/paste.py`

 * *Files 12% similar despite different names*

```diff
@@ -22,81 +22,93 @@
 
 from __future__ import annotations
 
 import datetime
 from typing import TYPE_CHECKING, Any
 
 if TYPE_CHECKING:
+    from collections.abc import Sequence
+
     from typing_extensions import Self
 
-    from mystbin.types.responses import FileResponse, PasteResponse
+    from mystbin.types.responses import CreatePasteResponse, FileResponse, GetPasteResponse
+
 
 __all__ = (
     "File",
     "Paste",
 )
 
 
 class File:
     _lines_of_code: int
     _character_count: int
+    _parent_id: str
+    _annotation: str
 
     """Represents a single file within a mystb.in paste.
 
     Attributes
     -----------
     filename: :class:`str`
         The file's name.
     content: :class:`str`
         The file's contents.
     """
 
     __slots__ = (
         "filename",
         "content",
-        "attachment_url",
         "_lines_of_code",
         "_character_count",
+        "_parent_id",
+        "_annotation",
     )
 
-    def __init__(self, *, filename: str, content: str, attachment_url: str | None = None) -> None:
+    def __init__(self, *, filename: str, content: str) -> None:
         self.filename: str = filename
         self.content: str = content
-        self.attachment_url: str | None = attachment_url
 
     @property
     def lines_of_code(self) -> int:
         return self._lines_of_code
 
     @property
     def character_count(self) -> int:
         return self._character_count
 
+    @property
+    def annotation(self) -> str:
+        return self._annotation
+
+    @property
+    def parent_id(self) -> str:
+        return self._parent_id
+
     @classmethod
     def from_data(cls, payload: FileResponse, /) -> Self:
         self = cls(
             content=payload["content"],
             filename=payload["filename"],
-            attachment_url=payload["attachment"],
         )
         self._lines_of_code = payload["loc"]
         self._character_count = payload["charcount"]
+        self._annotation = payload["annotation"]
+        self._parent_id = payload["parent_id"]
 
         return self
 
     def to_dict(self) -> dict[str, Any]:
-        ret: dict[str, Any] = {"content": self.content, "filename": self.filename}
-
-        return ret
+        return {"content": self.content, "filename": self.filename}
 
 
 class Paste:
-    _last_edited: datetime.datetime | None
     _expires: datetime.datetime | None
     _views: int | None
+    _security: str | None
 
     """Represents a Paste object from mystb.in.
 
     Attributes
     -----------
     id: :class:`str`
         The ID of this paste.
@@ -107,64 +119,77 @@
     """
 
     __slots__ = (
         "id",
         "author_id",
         "created_at",
         "files",
-        "notice",
+        "_security",
         "_expires",
         "_views",
-        "_last_edited",
     )
 
-    def __init__(self, *, id: str, created_at: str, files: list[File], notice: str | None) -> None:
+    def __init__(self, *, id: str, created_at: str, files: Sequence[File]) -> None:
         self.id: str = id
         self.created_at: datetime.datetime = datetime.datetime.fromisoformat(created_at)
-        self.files: list[File] = files
-        self.notice: str | None = notice
+        self.files: Sequence[File] = files
 
     def __str__(self) -> str:
         return self.url
 
     def __repr__(self) -> str:
         return f"<Paste id={self.id!r} files={len(self.files)}>"
 
     @property
     def url(self) -> str:
         return f"https://mystb.in/{self.id}"
 
     @property
-    def last_edited(self) -> datetime.datetime | None:
-        return self._last_edited
-
-    @property
     def expires(self) -> datetime.datetime | None:
         return self._expires
 
     @property
     def views(self) -> int | None:
         return self._views
 
+    @property
+    def security_token(self) -> str | None:
+        return self._security
+
     @classmethod
-    def from_data(cls, payload: PasteResponse, /) -> Self:
+    def from_get(cls, payload: GetPasteResponse, /) -> Self:
         files = [File.from_data(data) for data in payload["files"]]
         self = cls(
             id=payload["id"],
             created_at=payload["created_at"],
             files=files,
-            notice=payload.get("notice"),
         )
-        self._views = payload.get("views")
-        last_edited = payload.get("last_edited")
-        if last_edited:
-            self._last_edited = datetime.datetime.fromisoformat(last_edited)
+        self._views = payload["views"]
+
+        expires = payload["expires"]
+        if expires:
+            self._expires = datetime.datetime.fromisoformat(expires)
         else:
-            self._last_edited = None
+            self._expires = None
+
+        self._security = None
+
+        return self
+
+    @classmethod
+    def from_create(cls, payload: CreatePasteResponse, files: Sequence[File]) -> Self:
+        self = cls(
+            id=payload["id"],
+            created_at=payload["created_at"],
+            files=files,
+        )
+        self._views = 0
 
         expires = payload["expires"]
         if expires:
             self._expires = datetime.datetime.fromisoformat(expires)
         else:
             self._expires = None
 
+        self._security = payload["safety"]
+
         return self
```

### Comparing `mystbin_py-6.1.0/mystbin/types/__init__.py` & `mystbin_py-7.0.0/mystbin/types/__init__.py`

 * *Files identical despite different names*

### Comparing `mystbin_py-6.1.0/mystbin/types/responses.py` & `mystbin_py-7.0.0/mystbin/utils.py`

 * *Files 19% similar despite different names*

```diff
@@ -16,44 +16,29 @@
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
 FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 DEALINGS IN THE SOFTWARE.
 """
 
-from __future__ import annotations
+from typing import Any
 
-from typing import TYPE_CHECKING, TypedDict
+__all__ = ("MISSING",)
 
-if TYPE_CHECKING:
-    from datetime import datetime
 
-    from typing_extensions import NotRequired
+class _MissingSentinel:
+    __slots__ = ()
 
+    def __eq__(self, other: object) -> bool:
+        return False
 
-__all__ = (
-    "FileResponse",
-    "PasteResponse",
-)
+    def __bool__(self) -> bool:
+        return False
 
+    def __hash__(self) -> int:
+        return 0
 
-class FileResponse(TypedDict):
-    filename: str
-    content: str
-    loc: int
-    charcount: int
-    attachment: str | None
+    def __repr__(self) -> str:
+        return "..."
 
 
-class PasteResponse(TypedDict):
-    id: str
-    author_id: int | None
-    created_at: str
-    expires: str | None
-    last_edited: NotRequired[str]
-    files: list[FileResponse]
-    notice: NotRequired[str]
-
-
-class EditPasteResponse(TypedDict):
-    id: str
-    expires: datetime | None
+MISSING: Any = _MissingSentinel()
```

### Comparing `mystbin_py-6.1.0/pyproject.toml` & `mystbin_py-7.0.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mystbin-py"
-version = "6.1.0"
+version = "7.0.0"
 description = "A small simple wrapper around the mystb.in API."
 authors = ["AbstractUmbra <umbra@abstractumbra.dev>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/PythonistaGuild/mystbin.py"
 repository = "https://github.com/PythonistaGuild/mystbin.py"
 keywords = ["mystbin", "paste"]
@@ -13,14 +13,15 @@
     "Intended Audience :: Developers",
     "Natural Language :: English",
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
     "Topic :: Internet",
     "Typing :: Typed",
 ]
 include = ["LICENSE"]
 packages = [
     { include = "mystbin" },
     { include = "mystbin/**/*.py" },
@@ -54,21 +55,24 @@
 [tool.poetry.group.docs.dependencies]
 sphinx = "*"
 sphinxcontrib-trio = "*"
 furo = "*"
 
 [tool.poetry.group.dev.dependencies]
 ruff = "*"
+"typing-extensions" = "*"
 
 [tool.poetry.scripts]
 version = 'mystbin.__main__:show_version'
 
 [tool.ruff]
 line-length = 125
 target-version = "py38"
+
+[tool.ruff.lint]
 exclude = ["docs/**/*.py"]
 select = [
     "C4",
     "F",
     "G",
     "I",
     "PTH",
@@ -92,42 +96,40 @@
     "UP034",
     "UP038",
     "ANN101",
     "ANN102",
     "ANN401",
 ]
 
-[tool.ruff.format]
-# Like Black, use double quotes for strings.
-quote-style = "double"
-
-# Like Black, indent with spaces, rather than tabs.
-indent-style = "space"
-
-# Like Black, respect magic trailing commas.
-skip-magic-trailing-comma = false
 
-# Like Black, automatically detect the appropriate line ending.
-line-ending = "auto"
-
-[tool.ruff.isort]
+[tool.ruff.lint.isort]
 split-on-trailing-comma = true
 combine-as-imports = true
 
-[tool.ruff.flake8-annotations]
+[tool.ruff.lint.flake8-annotations]
 allow-star-arg-any = true
 
-[tool.ruff.flake8-pytest-style]
+[tool.ruff.lint.flake8-pytest-style]
 fixture-parentheses = false
 mark-parentheses = false
 parametrize-names-type = "csv"
 
-[tool.ruff.flake8-quotes]
+[tool.ruff.lint.flake8-quotes]
 inline-quotes = "single"
 
+[tool.ruff.format]
+# Like Black, use double quotes for strings.
+quote-style = "double"
+# Like Black, indent with spaces, rather than tabs.
+indent-style = "space"
+# Like Black, respect magic trailing commas.
+skip-magic-trailing-comma = false
+# Like Black, automatically detect the appropriate line ending.
+line-ending = "auto"
+
 [tool.pyright]
 ignore = ["docs/conf.py"]
 include = ["mystbin/**/*.py"]
 useLibraryCodeForTypes = true
 typeCheckingMode = "strict"
 pythonVersion = "3.8"
```

### Comparing `mystbin_py-6.1.0/PKG-INFO` & `mystbin_py-7.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mystbin-py
-Version: 6.1.0
+Version: 7.0.0
 Summary: A small simple wrapper around the mystb.in API.
 Home-page: https://github.com/PythonistaGuild/mystbin.py
 License: MIT
 Keywords: mystbin,paste
 Author: AbstractUmbra
 Author-email: umbra@abstractumbra.dev
 Requires-Python: >=3.8,<4.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: mystbin-py Version: 6.1.0 Summary: A small simple
+Metadata-Version: 2.1 Name: mystbin-py Version: 7.0.0 Summary: A small simple
 wrapper around the mystb.in API. Home-page: https://github.com/PythonistaGuild/
 mystbin.py License: MIT Keywords: mystbin,paste Author: AbstractUmbra Author-
 email: umbra@abstractumbra.dev Requires-Python: >=3.8,<4.0 Classifier: Intended
 Audience :: Developers Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English Classifier: Operating System :: OS
 Independent Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
```

