# Comparing `tmp/google_sheets_sdk-0.1.1.tar.gz` & `tmp/google_sheets_sdk-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google_sheets_sdk-0.1.1.tar", max compression
+gzip compressed data, was "google_sheets_sdk-0.1.2.tar", max compression
```

## Comparing `google_sheets_sdk-0.1.1.tar` & `google_sheets_sdk-0.1.2.tar`

### file list

```diff
@@ -1,8 +1,16 @@
--rw-r--r--   0        0        0        0 2024-04-01 19:10:29.127500 google_sheets_sdk-0.1.1/README.md
--rw-r--r--   0        0        0       74 2024-04-03 17:18:45.705883 google_sheets_sdk-0.1.1/google_sheets_sdk/__init__.py
--rw-r--r--   0        0        0     2745 2024-04-03 17:18:12.204401 google_sheets_sdk-0.1.1/google_sheets_sdk/client.py
--rw-r--r--   0        0        0      617 2024-04-01 19:18:07.778334 google_sheets_sdk-0.1.1/google_sheets_sdk/helpers.py
--rw-r--r--   0        0        0      195 2024-04-03 17:19:12.947132 google_sheets_sdk-0.1.1/google_sheets_sdk/schemas.py
--rw-r--r--   0        0        0      317 2024-04-03 17:17:23.401547 google_sheets_sdk-0.1.1/google_sheets_sdk/settings.py
--rw-r--r--   0        0        0      407 2024-04-03 17:20:05.888516 google_sheets_sdk-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      588 1970-01-01 00:00:00.000000 google_sheets_sdk-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-05-08 20:40:25.393452 google_sheets_sdk-0.1.2/README.md
+-rw-r--r--   0        0        0       30 2024-05-09 20:16:26.492100 google_sheets_sdk-0.1.2/google_sheets_sdk/__init__.py
+-rw-r--r--   0        0        0       81 2024-05-09 21:26:16.192570 google_sheets_sdk-0.1.2/google_sheets_sdk/entities/__init__.py
+-rw-r--r--   0        0        0      317 2024-05-09 19:37:37.022530 google_sheets_sdk-0.1.2/google_sheets_sdk/entities/settings.py
+-rw-r--r--   0        0        0      153 2024-05-09 21:45:00.913001 google_sheets_sdk-0.1.2/google_sheets_sdk/entities/sheet.py
+-rw-r--r--   0        0        0       14 2024-05-09 21:45:18.630595 google_sheets_sdk-0.1.2/google_sheets_sdk/entities/spreadsheet.py
+-rw-r--r--   0        0        0     1393 2024-05-09 21:16:10.790753 google_sheets_sdk-0.1.2/google_sheets_sdk/entities/token.py
+-rw-r--r--   0        0        0      347 2024-05-09 21:56:10.068794 google_sheets_sdk-0.1.2/google_sheets_sdk/example.py
+-rw-r--r--   0        0        0       27 2024-05-09 20:14:03.310461 google_sheets_sdk-0.1.2/google_sheets_sdk/frameworks/__init__.py
+-rw-r--r--   0        0        0     2935 2024-05-09 21:54:57.533433 google_sheets_sdk-0.1.2/google_sheets_sdk/frameworks/client/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-09 19:32:08.899991 google_sheets_sdk-0.1.2/google_sheets_sdk/interfaces/controllers/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-09 19:32:06.270051 google_sheets_sdk-0.1.2/google_sheets_sdk/interfaces/repositories/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-09 19:32:11.271937 google_sheets_sdk-0.1.2/google_sheets_sdk/interfaces/services/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-09 21:30:12.963346 google_sheets_sdk-0.1.2/google_sheets_sdk/use_cases/__init__.py
+-rw-r--r--   0        0        0      407 2024-05-09 21:56:32.289292 google_sheets_sdk-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      588 1970-01-01 00:00:00.000000 google_sheets_sdk-0.1.2/PKG-INFO
```

### Comparing `google_sheets_sdk-0.1.1/google_sheets_sdk/client.py` & `google_sheets_sdk-0.1.2/google_sheets_sdk/frameworks/client/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,91 +1,102 @@
-import time as t
-from dataclasses import dataclass
-from typing import Any, ClassVar
-
-from httpx import AsyncClient, HTTPStatusError
-from jose import jwt
-
-from google_sheets_sdk import Settings
-from google_sheets_sdk.helpers import check_token_expiration
-from google_sheets_sdk.schemas import TokenData
+from dataclasses import InitVar, dataclass, field
+from typing import TYPE_CHECKING, ClassVar
+
+from entities import Settings, Sheet, Token
+from entities import spreadsheet as spreadsheet_entity
+from pydantic import BaseModel
+from pydantic.fields import Field
+
+if TYPE_CHECKING:
+    from httpx import AsyncClient, HTTPStatusError
+
+
+class BatchUpdateValuesResponse(BaseModel):
+    spreadsheet_id: str = Field(
+        ...,
+        alias="spreadsheetId",
+    )
+    total_updated_rows: int = Field(
+        ...,
+        alias="totalUpdatedRows",
+    )
+    total_updated_columns: int = Field(
+        ...,
+        alias="totalUpdatedColumns",
+    )
+    total_updated_cells: int = Field(
+        ...,
+        alias="totalUpdatedCells",
+    )
+    total_updated_sheets: int = Field(
+        ...,
+        alias="totalUpdatedSheets",
+    )
 
 
 @dataclass
 class Client:
-    settings: ClassVar["Settings"] = Settings()  # type: ignore
-    base_url: ClassVar[str] = "https://sheets.googleapis.com/"
-    token_data: ClassVar[TokenData] = TokenData(
-        iss=settings.CLIENT_EMAIL,
-        sub=settings.CLIENT_EMAIL,
-        aud=f"{base_url}",
-        scope=settings.SCOPE,
-    )
-
-    http_client: "AsyncClient"
-
-    def get_token(self) -> str:
-        return jwt.encode(
-            self.token_data.model_dump(
-                mode="json",
-            ),
-            self.settings.PRIVATE_KEY.replace(r"\n", "\n"),
-            headers={
-                "kid": self.settings.PRIVATE_KEY_ID,
-            },
-            algorithm="RS256",
-        )
+    _base_url: ClassVar[str] = "https://sheets.googleapis.com/"
 
-    def update_token_data(self) -> None:
-        iat = t.time()
-        self.token_data.iat = iat
-        self.token_data.exp = iat + 3600
+    _http_client: "AsyncClient"
+    _token: Token = field(
+        init=False,
+    )
+    settings: InitVar[Settings]
 
-    def is_token_expired(self) -> bool:
-        return bool(self.token_data.exp) and (self.token_data.exp - t.time()) > 60
+    def __post_init__(
+        self,
+        settings: Settings,
+    ):
+        self._token = Token(
+            email=settings.CLIENT_EMAIL,
+            base_url=self._base_url,
+            scope=settings.SCOPE.unicode_string(),
+            private_key=settings.PRIVATE_KEY.replace(r"\n", "\n"),
+            private_key_id=settings.PRIVATE_KEY_ID,
+        )
 
-    @check_token_expiration
     async def batch_clear_values(
         self,
-        spreadsheet_id: str,
+        spreadsheet_id: spreadsheet_entity.Id,
         ranges: list[str],
-    ) -> dict[str, Any]:
+    ) -> None:
         try:
-            response = await self.http_client.post(
-                url=f"{self.base_url}v4/spreadsheets/{spreadsheet_id}/values:batchClear",
+            response = await self._http_client.post(
+                url=f"{self._base_url}v4/spreadsheets/{spreadsheet_id}/values:batchClear",
                 json={
                     "ranges": ranges,
                 },
                 headers={
-                    "Authorization": f"Bearer {self.get_token()}",
+                    "Authorization": f"Bearer {self._token.encoded}",
                 },
             )
             response.raise_for_status()
         except HTTPStatusError as exc:
-            print(exc.response.text)
             raise exc
-        else:
-            return response.json()
 
-    @check_token_expiration
     async def batch_update_values(
         self,
-        spreadsheet_id: str,
-        data: list[dict[str, list]],
-    ) -> dict[str, Any]:
+        spreadsheet_id: spreadsheet_entity.Id,
+        sheets: list[Sheet],
+    ) -> BatchUpdateValuesResponse:
         try:
-            response = await self.http_client.post(
-                url=f"{self.base_url}v4/spreadsheets/{spreadsheet_id}/values:batchUpdate",
+            response = await self._http_client.post(
+                url=f"{self._base_url}v4/spreadsheets/{spreadsheet_id}/values:batchUpdate",
                 json={
                     "valueInputOption": "USER_ENTERED",
-                    "data": data,
+                    "data": [
+                        sheet.model_dump(
+                            mode="json",
+                        )
+                        for sheet in sheets
+                    ],
                 },
                 headers={
-                    "Authorization": f"Bearer {self.get_token()}",
+                    "Authorization": f"Bearer {self._token.encoded}",
                 },
             )
             response.raise_for_status()
         except HTTPStatusError as exc:
-            print(exc.response.text)
             raise exc
         else:
-            return response.json()
+            return BatchUpdateValuesResponse(**response.json())
```

### Comparing `google_sheets_sdk-0.1.1/PKG-INFO` & `google_sheets_sdk-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-sheets-sdk
-Version: 0.1.1
+Version: 0.1.2
 Summary: 
 Author: Marco Carmona
 Author-email: marcocarmonapy@outlook.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

