# Comparing `tmp/usercloudssdk-1.6.0.tar.gz` & `tmp/usercloudssdk-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "usercloudssdk-1.6.0.tar", last modified: Mon Mar 25 20:55:54 2024, max compression
+gzip compressed data, was "usercloudssdk-1.7.0.tar", last modified: Thu May  9 22:40:50 2024, max compression
```

## Comparing `usercloudssdk-1.6.0.tar` & `usercloudssdk-1.7.0.tar`

### file list

```diff
@@ -1,24 +1,26 @@
-drwxr-xr-x   0 jwang      (501) staff       (20)        0 2024-03-25 20:55:54.624063 usercloudssdk-1.6.0/
--rw-r--r--   0 jwang      (501) staff       (20)      954 2024-03-25 20:55:54.623856 usercloudssdk-1.6.0/PKG-INFO
--rw-r--r--   0 jwang      (501) staff       (20)      984 2024-03-04 16:46:15.000000 usercloudssdk-1.6.0/README.md
--rw-r--r--   0 jwang      (501) staff       (20)     1041 2024-03-25 20:55:11.000000 usercloudssdk-1.6.0/pyproject.toml
--rw-r--r--   0 jwang      (501) staff       (20)       38 2024-03-25 20:55:54.624104 usercloudssdk-1.6.0/setup.cfg
-drwxr-xr-x   0 jwang      (501) staff       (20)        0 2024-03-25 20:55:54.620597 usercloudssdk-1.6.0/src/
-drwxr-xr-x   0 jwang      (501) staff       (20)        0 2024-03-25 20:55:54.622746 usercloudssdk-1.6.0/src/usercloudssdk/
--rw-r--r--   0 jwang      (501) staff       (20)        0 2024-03-04 16:46:15.000000 usercloudssdk-1.6.0/src/usercloudssdk/__init__.py
--rw-r--r--   0 jwang      (501) staff       (20)    40669 2024-03-25 19:34:08.000000 usercloudssdk-1.6.0/src/usercloudssdk/asyncclient.py
--rw-r--r--   0 jwang      (501) staff       (20)    37368 2024-03-25 19:34:08.000000 usercloudssdk-1.6.0/src/usercloudssdk/client.py
--rw-r--r--   0 jwang      (501) staff       (20)      965 2024-03-04 16:46:15.000000 usercloudssdk-1.6.0/src/usercloudssdk/client_helpers.py
--rw-r--r--   0 jwang      (501) staff       (20)     1335 2024-03-04 16:46:15.000000 usercloudssdk-1.6.0/src/usercloudssdk/client_test.py
--rw-r--r--   0 jwang      (501) staff       (20)     1310 2024-03-04 16:46:15.000000 usercloudssdk-1.6.0/src/usercloudssdk/constants.py
--rw-r--r--   0 jwang      (501) staff       (20)     1452 2024-03-04 16:46:15.000000 usercloudssdk-1.6.0/src/usercloudssdk/errors.py
--rw-r--r--   0 jwang      (501) staff       (20)    39629 2024-03-04 16:46:15.000000 usercloudssdk-1.6.0/src/usercloudssdk/models.py
--rw-r--r--   0 jwang      (501) staff       (20)      791 2024-03-04 16:46:15.000000 usercloudssdk-1.6.0/src/usercloudssdk/policies.py
--rw-r--r--   0 jwang      (501) staff       (20)     6260 2024-03-04 16:46:15.000000 usercloudssdk-1.6.0/src/usercloudssdk/uchttpclient.py
--rw-r--r--   0 jwang      (501) staff       (20)      558 2024-03-25 19:34:08.000000 usercloudssdk-1.6.0/src/usercloudssdk/ucjson.py
-drwxr-xr-x   0 jwang      (501) staff       (20)        0 2024-03-25 20:55:54.623628 usercloudssdk-1.6.0/src/usercloudssdk.egg-info/
--rw-r--r--   0 jwang      (501) staff       (20)      954 2024-03-25 20:55:54.000000 usercloudssdk-1.6.0/src/usercloudssdk.egg-info/PKG-INFO
--rw-r--r--   0 jwang      (501) staff       (20)      567 2024-03-25 20:55:54.000000 usercloudssdk-1.6.0/src/usercloudssdk.egg-info/SOURCES.txt
--rw-r--r--   0 jwang      (501) staff       (20)        1 2024-03-25 20:55:54.000000 usercloudssdk-1.6.0/src/usercloudssdk.egg-info/dependency_links.txt
--rw-r--r--   0 jwang      (501) staff       (20)      129 2024-03-25 20:55:54.000000 usercloudssdk-1.6.0/src/usercloudssdk.egg-info/requires.txt
--rw-r--r--   0 jwang      (501) staff       (20)       14 2024-03-25 20:55:54.000000 usercloudssdk-1.6.0/src/usercloudssdk.egg-info/top_level.txt
+drwxr-xr-x   0 gintwoss   (501) staff       (20)        0 2024-05-09 22:40:50.078087 usercloudssdk-1.7.0/
+-rw-r--r--   0 gintwoss   (501) staff       (20)     1103 2023-10-03 22:02:15.000000 usercloudssdk-1.7.0/LICENSE
+-rw-r--r--   0 gintwoss   (501) staff       (20)     2257 2024-05-09 22:40:50.077925 usercloudssdk-1.7.0/PKG-INFO
+-rw-r--r--   0 gintwoss   (501) staff       (20)      984 2024-05-09 20:42:43.000000 usercloudssdk-1.7.0/README.md
+-rw-r--r--   0 gintwoss   (501) staff       (20)     1041 2024-05-09 22:33:50.000000 usercloudssdk-1.7.0/pyproject.toml
+-rw-r--r--   0 gintwoss   (501) staff       (20)       38 2024-05-09 22:40:50.078121 usercloudssdk-1.7.0/setup.cfg
+drwxr-xr-x   0 gintwoss   (501) staff       (20)        0 2024-05-09 22:40:50.074456 usercloudssdk-1.7.0/src/
+drwxr-xr-x   0 gintwoss   (501) staff       (20)        0 2024-05-09 22:40:50.077076 usercloudssdk-1.7.0/src/usercloudssdk/
+-rw-r--r--   0 gintwoss   (501) staff       (20)        0 2023-10-03 22:02:15.000000 usercloudssdk-1.7.0/src/usercloudssdk/__init__.py
+-rw-r--r--   0 gintwoss   (501) staff       (20)    43439 2024-05-09 20:42:43.000000 usercloudssdk-1.7.0/src/usercloudssdk/asyncclient.py
+-rw-r--r--   0 gintwoss   (501) staff       (20)    39929 2024-05-09 20:42:43.000000 usercloudssdk-1.7.0/src/usercloudssdk/client.py
+-rw-r--r--   0 gintwoss   (501) staff       (20)      965 2024-05-09 20:42:43.000000 usercloudssdk-1.7.0/src/usercloudssdk/client_helpers.py
+-rw-r--r--   0 gintwoss   (501) staff       (20)     1335 2024-05-09 20:42:43.000000 usercloudssdk-1.7.0/src/usercloudssdk/client_test.py
+-rw-r--r--   0 gintwoss   (501) staff       (20)     1310 2024-05-09 20:42:43.000000 usercloudssdk-1.7.0/src/usercloudssdk/constants.py
+-rw-r--r--   0 gintwoss   (501) staff       (20)      676 2024-05-09 20:42:43.000000 usercloudssdk-1.7.0/src/usercloudssdk/data_types.py
+-rw-r--r--   0 gintwoss   (501) staff       (20)     1452 2024-05-09 20:42:43.000000 usercloudssdk-1.7.0/src/usercloudssdk/errors.py
+-rw-r--r--   0 gintwoss   (501) staff       (20)    45721 2024-05-09 20:42:43.000000 usercloudssdk-1.7.0/src/usercloudssdk/models.py
+-rw-r--r--   0 gintwoss   (501) staff       (20)      791 2024-05-09 20:42:43.000000 usercloudssdk-1.7.0/src/usercloudssdk/policies.py
+-rw-r--r--   0 gintwoss   (501) staff       (20)     6260 2024-05-09 20:42:43.000000 usercloudssdk-1.7.0/src/usercloudssdk/uchttpclient.py
+-rw-r--r--   0 gintwoss   (501) staff       (20)      574 2024-05-09 20:42:43.000000 usercloudssdk-1.7.0/src/usercloudssdk/ucjson.py
+drwxr-xr-x   0 gintwoss   (501) staff       (20)        0 2024-05-09 22:40:50.077738 usercloudssdk-1.7.0/src/usercloudssdk.egg-info/
+-rw-r--r--   0 gintwoss   (501) staff       (20)     2257 2024-05-09 22:40:50.000000 usercloudssdk-1.7.0/src/usercloudssdk.egg-info/PKG-INFO
+-rw-r--r--   0 gintwoss   (501) staff       (20)      607 2024-05-09 22:40:50.000000 usercloudssdk-1.7.0/src/usercloudssdk.egg-info/SOURCES.txt
+-rw-r--r--   0 gintwoss   (501) staff       (20)        1 2024-05-09 22:40:50.000000 usercloudssdk-1.7.0/src/usercloudssdk.egg-info/dependency_links.txt
+-rw-r--r--   0 gintwoss   (501) staff       (20)      129 2024-05-09 22:40:50.000000 usercloudssdk-1.7.0/src/usercloudssdk.egg-info/requires.txt
+-rw-r--r--   0 gintwoss   (501) staff       (20)       14 2024-05-09 22:40:50.000000 usercloudssdk-1.7.0/src/usercloudssdk.egg-info/top_level.txt
```

### Comparing `usercloudssdk-1.6.0/README.md` & `usercloudssdk-1.7.0/README.md`

 * *Files identical despite different names*

### Comparing `usercloudssdk-1.6.0/pyproject.toml` & `usercloudssdk-1.7.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "usercloudssdk"
-version = "1.6.0"
+version = "1.7.0"
 description = "Python SDK for UserClouds"
 authors = [{ name = "UserClouds", email = "info@userclouds.com" }]
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: 3.9",
```

### Comparing `usercloudssdk-1.6.0/src/usercloudssdk/asyncclient.py` & `usercloudssdk-1.7.0/src/usercloudssdk/asyncclient.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 from .errors import UserCloudsSDKError
 from .models import (
     Accessor,
     AccessPolicy,
     AccessPolicyTemplate,
     Column,
     ColumnConsentedPurposes,
+    ColumnDataType,
     ColumnRetentionDurationResponse,
     ColumnRetentionDurationsResponse,
     Edge,
     EdgeType,
     InspectTokenResponse,
     Mutator,
     Object,
@@ -181,17 +182,67 @@
             "row_data": row_data,
             "id": id,
             "organization_id": organization_id,
             "region": region,
         }
         return await self._post_async("/userstore/api/users", json_data=body)
 
+    # ColumnDataType Operations
+
+    async def CreateColumnDataTypeAsync(
+        self, dataType: ColumnDataType, if_not_exists: bool = False
+    ) -> ColumnDataType:
+        try:
+            resp_json = await self._post_async(
+                "/userstore/config/datatypes",
+                json_data={"data_type": dataType.__dict__},
+            )
+            return ColumnDataType.from_json(resp_json)
+        except UserCloudsSDKError as err:
+            if if_not_exists:
+                dataType.id = _id_from_identical_conflict(err)
+                return dataType
+            raise err
+
+    async def DeleteColumnDataTypeAsync(self, id: uuid.UUID) -> bool:
+        return await self._delete_async(f"/userstore/config/datatypes/{id}")
+
+    async def GetColumnDataTypeAsync(self, id: uuid.UUID) -> ColumnDataType:
+        resp_json = await self._get_async(f"/userstore/config/datatypes/{id}")
+        return ColumnDataType.from_json(resp_json)
+
+    async def ListColumnDataTypesAsync(
+        self, limit: int = 0, starting_after: uuid.UUID | None = None
+    ) -> list[ColumnDataType]:
+        params: dict[str, int | str] = {}
+        if limit > 0:
+            params["limit"] = limit
+        if starting_after is not None:
+            params["starting_after"] = f"id:{starting_after}"
+        params["version"] = "3"
+        resp_json = await self._get_async("/userstore/config/datatypes", params=params)
+        dataTypes = [
+            ColumnDataType.from_json(dataType) for dataType in resp_json["data"]
+        ]
+        return dataTypes
+
+    async def UpdateColumnDataTypeAsync(
+        self, dataType: ColumnDataType
+    ) -> ColumnDataType:
+        resp_json = await self._put_async(
+            f"/userstore/config/datatypes/{dataType.id}",
+            json_data={"data_type": dataType.__dict__},
+        )
+        return ColumnDataType.from_json(resp_json)
+
     # Column Operations
 
-    async def CreateColumnAsync(self, column: Column, if_not_exists=False) -> Column:
+    async def CreateColumnAsync(
+        self, column: Column, if_not_exists: bool = False
+    ) -> Column:
         try:
             resp_json = await self._post_async(
                 "/userstore/config/columns", json_data={"column": column.__dict__}
             )
             return Column.from_json(resp_json)
         except UserCloudsSDKError as err:
             if if_not_exists:
@@ -225,15 +276,15 @@
             json_data={"column": column.__dict__},
         )
         return Column.from_json(resp_json)
 
     # Purpose Operations
 
     async def CreatePurposeAsync(
-        self, purpose: Purpose, if_not_exists=False
+        self, purpose: Purpose, if_not_exists: bool = False
     ) -> Purpose:
         try:
             resp_json = await self._post_async(
                 "/userstore/config/purposes", json_data={"purpose": purpose.__dict__}
             )
             return Purpose.from_json(resp_json)
         except UserCloudsSDKError as err:
@@ -434,15 +485,15 @@
             json_data=req.to_json(),
         )
         return ColumnRetentionDurationsResponse.from_json(resp)
 
     # Access Policy Templates
 
     async def CreateAccessPolicyTemplateAsync(
-        self, access_policy_template: AccessPolicyTemplate, if_not_exists=False
+        self, access_policy_template: AccessPolicyTemplate, if_not_exists: bool = False
     ) -> AccessPolicyTemplate | UserCloudsSDKError:
         try:
             resp_json = await self._post_async(
                 "/tokenizer/policies/accesstemplate",
                 json_data={"access_policy_template": access_policy_template.__dict__},
             )
             return AccessPolicyTemplate.from_json(resp_json)
@@ -494,15 +545,15 @@
             f"/tokenizer/policies/accesstemplate/{id}",
             params={"template_version": str(version)},
         )
 
     # Access Policies
 
     async def CreateAccessPolicyAsync(
-        self, access_policy: AccessPolicy, if_not_exists=False
+        self, access_policy: AccessPolicy, if_not_exists: bool = False
     ) -> AccessPolicy | UserCloudsSDKError:
         try:
             resp_json = await self._post_async(
                 "/tokenizer/policies/access",
                 json_data={"access_policy": access_policy.__dict__},
             )
             return AccessPolicy.from_json(resp_json)
@@ -548,15 +599,15 @@
             f"/tokenizer/policies/access/{id}",
             params={"policy_version": str(version)},
         )
 
     # Transformers
 
     async def CreateTransformerAsync(
-        self, transformer: Transformer, if_not_exists=False
+        self, transformer: Transformer, if_not_exists: bool = False
     ):
         try:
             resp_json = await self._post_async(
                 "/tokenizer/policies/transformation",
                 json_data={"transformer": transformer.__dict__},
             )
             return Transformer.from_json(resp_json)
@@ -585,15 +636,15 @@
 
     async def DeleteTransformerAsync(self, id: uuid.UUID):
         return await self._delete_async(f"/tokenizer/policies/transformation/{id}")
 
     # Accessor Operations
 
     async def CreateAccessorAsync(
-        self, accessor: Accessor, if_not_exists=False
+        self, accessor: Accessor, if_not_exists: bool = False
     ) -> Accessor:
         try:
             resp_json = await self._post_async(
                 "/userstore/config/accessors", json_data={"accessor": accessor.__dict__}
             )
             return Accessor.from_json(resp_json)
         except UserCloudsSDKError as err:
@@ -639,15 +690,15 @@
             "selector_values": selector_values,
         }
         return await self._post_async("/userstore/api/accessors", json_data=body)
 
     # Mutator Operations
 
     async def CreateMutatorAsync(
-        self, mutator: Mutator, if_not_exists=False
+        self, mutator: Mutator, if_not_exists: bool = False
     ) -> Mutator:
         try:
             resp_json = await self._post_async(
                 "/userstore/config/mutators", json_data={"mutator": mutator.__dict__}
             )
             return Mutator.from_json(resp_json)
         except UserCloudsSDKError as e:
@@ -779,15 +830,17 @@
             params["starting_after"] = f"id:{starting_after}"
         params["version"] = "3"
         j = await self._get_async("/authz/objects", params=params)
 
         objects = [Object.from_json(o) for o in j["data"]]
         return objects
 
-    async def CreateObjectAsync(self, object: Object, if_not_exists=False) -> Object:
+    async def CreateObjectAsync(
+        self, object: Object, if_not_exists: bool = False
+    ) -> Object:
         try:
             j = await self._post_async(
                 "/authz/objects", json_data={"object": object.__dict__}
             )
             return Object.from_json(j)
         except UserCloudsSDKError as e:
             if if_not_exists:
@@ -812,15 +865,15 @@
             params["starting_after"] = f"id:{starting_after}"
         params["version"] = "3"
         j = await self._get_async("/authz/edges", params=params)
 
         edges = [Edge.from_json(e) for e in j["data"]]
         return edges
 
-    async def CreateEdgeAsync(self, edge: Edge, if_not_exists=False) -> Edge:
+    async def CreateEdgeAsync(self, edge: Edge, if_not_exists: bool = False) -> Edge:
         try:
             j = await self._post_async(
                 "/authz/edges", json_data={"edge": edge.__dict__}
             )
             return Edge.from_json(j)
         except UserCloudsSDKError as e:
             if if_not_exists:
@@ -846,15 +899,15 @@
         params["version"] = "3"
         j = await self._get_async("/authz/objecttypes", params=params)
 
         object_types = [ObjectType.from_json(ot) for ot in j["data"]]
         return object_types
 
     async def CreateObjectTypeAsync(
-        self, object_type: ObjectType, if_not_exists=False
+        self, object_type: ObjectType, if_not_exists: bool = False
     ) -> ObjectType:
         try:
             j = await self._post_async(
                 "/authz/objecttypes", json_data={"object_type": object_type.__dict__}
             )
             return ObjectType.from_json(j)
         except UserCloudsSDKError as e:
@@ -881,15 +934,15 @@
         params["version"] = "3"
         j = await self._get_async("/authz/edgetypes", params=params)
 
         edge_types = [EdgeType.from_json(et) for et in j["data"]]
         return edge_types
 
     async def CreateEdgeTypeAsync(
-        self, edge_type: EdgeType, if_not_exists=False
+        self, edge_type: EdgeType, if_not_exists: bool = False
     ) -> EdgeType:
         try:
             j = await self._post_async(
                 "/authz/edgetypes", json_data={"edge_type": edge_type.__dict__}
             )
             return EdgeType.from_json(j)
         except UserCloudsSDKError as e:
@@ -916,15 +969,15 @@
         params["version"] = "3"
         j = await self._get_async("/authz/organizations", params=params)
 
         organizations = [Organization.from_json(o) for o in j["data"]]
         return organizations
 
     async def CreateOrganizationAsync(
-        self, organization: Organization, if_not_exists=False
+        self, organization: Organization, if_not_exists: bool = False
     ) -> Organization:
         try:
             json_data = await self._post_async(
                 "/authz/organizations",
                 json_data={"organization": organization.__dict__},
             )
             return Organization.from_json(json_data)
@@ -965,14 +1018,31 @@
 
     async def GetExternalOIDCIssuersAsync(self) -> list[str]:
         return await self._get_async("/userstore/oidcissuers")
 
     async def UpdateExternalOIDCIssuersAsync(self, issuers: list[str]) -> list[str]:
         return await self._put_async("/userstore/oidcissuers", json_data=issuers)
 
+    async def UploadDataImportFileAsync(
+        self, file_path: Path, import_type: str = "executemutator"
+    ) -> uuid.UUID:
+        json_data = await self._get_async(
+            f"/userstore/upload/dataimport?import_type={import_type}"
+        )
+        import_id = uuid.UUID(json_data["import_id"])
+        with open(file_path, "rb") as f:
+            resp = await self._client.put_async(json_data["presigned_url"], content=f)
+            if resp.status_code >= 400:
+                raise UserCloudsSDKError.from_response(resp)
+        return import_id
+
+    async def CheckDataImportStatusAsync(self, import_id: uuid.UUID) -> dict:
+        json_data = await self._get_async(f"/userstore/upload/dataimport/{import_id}")
+        return json_data
+
     # Access Token Helpers
 
     async def _get_access_token_async(self) -> str:
         # Encode the client ID and client secret
         headers = {
             "Authorization": f"Basic {self._authorization}",
             "Content-Type": "application/x-www-form-urlencoded",
```

### Comparing `usercloudssdk-1.6.0/src/usercloudssdk/client.py` & `usercloudssdk-1.7.0/src/usercloudssdk/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 from .errors import UserCloudsSDKError
 from .models import (
     Accessor,
     AccessPolicy,
     AccessPolicyTemplate,
     Column,
     ColumnConsentedPurposes,
+    ColumnDataType,
     ColumnRetentionDurationResponse,
     ColumnRetentionDurationsResponse,
     Edge,
     EdgeType,
     InspectTokenResponse,
     Mutator,
     Object,
@@ -175,17 +176,63 @@
             "row_data": row_data,
             "id": id,
             "organization_id": organization_id,
             "region": region,
         }
         return self._post("/userstore/api/users", json_data=body)
 
+    # ColumnDataType Operations
+
+    def CreateColumnDataType(
+        self, dataType: ColumnDataType, if_not_exists: bool = False
+    ) -> ColumnDataType:
+        try:
+            resp_json = self._post(
+                "/userstore/config/datatypes",
+                json_data={"data_type": dataType.__dict__},
+            )
+            return ColumnDataType.from_json(resp_json)
+        except UserCloudsSDKError as err:
+            if if_not_exists:
+                dataType.id = _id_from_identical_conflict(err)
+                return dataType
+            raise err
+
+    def DeleteColumnDataType(self, id: uuid.UUID) -> bool:
+        return self._delete(f"/userstore/config/datatypes/{id}")
+
+    def GetColumnDataType(self, id: uuid.UUID) -> ColumnDataType:
+        resp_json = self._get(f"/userstore/config/datatypes/{id}")
+        return ColumnDataType.from_json(resp_json)
+
+    def ListColumnDataTypes(
+        self, limit: int = 0, starting_after: uuid.UUID | None = None
+    ) -> list[ColumnDataType]:
+        params: dict[str, int | str] = {}
+        if limit > 0:
+            params["limit"] = limit
+        if starting_after is not None:
+            params["starting_after"] = f"id:{starting_after}"
+        params["version"] = "3"
+        resp_json = self._get("/userstore/config/datatypes", params=params)
+        dataTypes = [
+            ColumnDataType.from_json(dataType) for dataType in resp_json["data"]
+        ]
+        return dataTypes
+
+    def UpdateColumnDataType(self, dataType: ColumnDataType) -> ColumnDataType:
+        resp_json = self._put(
+            f"/userstore/config/datatypes/{dataType.id}",
+            json_data={"data_type": dataType.__dict__},
+        )
+        return ColumnDataType.from_json(resp_json)
+
     # Column Operations
 
-    def CreateColumn(self, column: Column, if_not_exists=False) -> Column:
+    def CreateColumn(self, column: Column, if_not_exists: bool = False) -> Column:
         try:
             resp_json = self._post(
                 "/userstore/config/columns", json_data={"column": column.__dict__}
             )
             return Column.from_json(resp_json)
         except UserCloudsSDKError as err:
             if if_not_exists:
@@ -218,15 +265,15 @@
             f"/userstore/config/columns/{column.id}",
             json_data={"column": column.__dict__},
         )
         return Column.from_json(resp_json)
 
     # Purpose Operations
 
-    def CreatePurpose(self, purpose: Purpose, if_not_exists=False) -> Purpose:
+    def CreatePurpose(self, purpose: Purpose, if_not_exists: bool = False) -> Purpose:
         try:
             resp_json = self._post(
                 "/userstore/config/purposes", json_data={"purpose": purpose.__dict__}
             )
             return Purpose.from_json(resp_json)
         except UserCloudsSDKError as err:
             if if_not_exists:
@@ -424,15 +471,15 @@
             json_data=req.to_json(),
         )
         return ColumnRetentionDurationsResponse.from_json(resp)
 
     # Access Policy Templates
 
     def CreateAccessPolicyTemplate(
-        self, access_policy_template: AccessPolicyTemplate, if_not_exists=False
+        self, access_policy_template: AccessPolicyTemplate, if_not_exists: bool = False
     ) -> AccessPolicyTemplate | UserCloudsSDKError:
         try:
             resp_json = self._post(
                 "/tokenizer/policies/accesstemplate",
                 json_data={"access_policy_template": access_policy_template.__dict__},
             )
             return AccessPolicyTemplate.from_json(resp_json)
@@ -476,15 +523,15 @@
             f"/tokenizer/policies/accesstemplate/{id}",
             params={"template_version": str(version)},
         )
 
     # Access Policies
 
     def CreateAccessPolicy(
-        self, access_policy: AccessPolicy, if_not_exists=False
+        self, access_policy: AccessPolicy, if_not_exists: bool = False
     ) -> AccessPolicy | UserCloudsSDKError:
         try:
             resp_json = self._post(
                 "/tokenizer/policies/access",
                 json_data={"access_policy": access_policy.__dict__},
             )
             return AccessPolicy.from_json(resp_json)
@@ -527,15 +574,15 @@
         return self._delete(
             f"/tokenizer/policies/access/{id}",
             params={"policy_version": str(version)},
         )
 
     # Transformers
 
-    def CreateTransformer(self, transformer: Transformer, if_not_exists=False):
+    def CreateTransformer(self, transformer: Transformer, if_not_exists: bool = False):
         try:
             resp_json = self._post(
                 "/tokenizer/policies/transformation",
                 json_data={"transformer": transformer.__dict__},
             )
             return Transformer.from_json(resp_json)
         except UserCloudsSDKError as err:
@@ -558,15 +605,17 @@
     # Note: Transformers are immutable, so no Update method is provided.
 
     def DeleteTransformer(self, id: uuid.UUID):
         return self._delete(f"/tokenizer/policies/transformation/{id}")
 
     # Accessor Operations
 
-    def CreateAccessor(self, accessor: Accessor, if_not_exists=False) -> Accessor:
+    def CreateAccessor(
+        self, accessor: Accessor, if_not_exists: bool = False
+    ) -> Accessor:
         try:
             resp_json = self._post(
                 "/userstore/config/accessors", json_data={"accessor": accessor.__dict__}
             )
             return Accessor.from_json(resp_json)
         except UserCloudsSDKError as err:
             if if_not_exists:
@@ -610,15 +659,15 @@
             "context": context,
             "selector_values": selector_values,
         }
         return self._post("/userstore/api/accessors", json_data=body)
 
     # Mutator Operations
 
-    def CreateMutator(self, mutator: Mutator, if_not_exists=False) -> Mutator:
+    def CreateMutator(self, mutator: Mutator, if_not_exists: bool = False) -> Mutator:
         try:
             resp_json = self._post(
                 "/userstore/config/mutators", json_data={"mutator": mutator.__dict__}
             )
             return Mutator.from_json(resp_json)
         except UserCloudsSDKError as e:
             if if_not_exists:
@@ -747,15 +796,15 @@
             params["starting_after"] = f"id:{starting_after}"
         params["version"] = "3"
         j = self._get("/authz/objects", params=params)
 
         objects = [Object.from_json(o) for o in j["data"]]
         return objects
 
-    def CreateObject(self, object: Object, if_not_exists=False) -> Object:
+    def CreateObject(self, object: Object, if_not_exists: bool = False) -> Object:
         try:
             j = self._post("/authz/objects", json_data={"object": object.__dict__})
             return Object.from_json(j)
         except UserCloudsSDKError as e:
             if if_not_exists:
                 object.id = _id_from_identical_conflict(e)
                 return object
@@ -778,15 +827,15 @@
             params["starting_after"] = f"id:{starting_after}"
         params["version"] = "3"
         j = self._get("/authz/edges", params=params)
 
         edges = [Edge.from_json(e) for e in j["data"]]
         return edges
 
-    def CreateEdge(self, edge: Edge, if_not_exists=False) -> Edge:
+    def CreateEdge(self, edge: Edge, if_not_exists: bool = False) -> Edge:
         try:
             j = self._post("/authz/edges", json_data={"edge": edge.__dict__})
             return Edge.from_json(j)
         except UserCloudsSDKError as e:
             if if_not_exists:
                 edge.id = _id_from_identical_conflict(e)
                 return edge
@@ -810,15 +859,15 @@
         params["version"] = "3"
         j = self._get("/authz/objecttypes", params=params)
 
         object_types = [ObjectType.from_json(ot) for ot in j["data"]]
         return object_types
 
     def CreateObjectType(
-        self, object_type: ObjectType, if_not_exists=False
+        self, object_type: ObjectType, if_not_exists: bool = False
     ) -> ObjectType:
         try:
             j = self._post(
                 "/authz/objecttypes", json_data={"object_type": object_type.__dict__}
             )
             return ObjectType.from_json(j)
         except UserCloudsSDKError as e:
@@ -844,15 +893,17 @@
             params["starting_after"] = f"id:{starting_after}"
         params["version"] = "3"
         j = self._get("/authz/edgetypes", params=params)
 
         edge_types = [EdgeType.from_json(et) for et in j["data"]]
         return edge_types
 
-    def CreateEdgeType(self, edge_type: EdgeType, if_not_exists=False) -> EdgeType:
+    def CreateEdgeType(
+        self, edge_type: EdgeType, if_not_exists: bool = False
+    ) -> EdgeType:
         try:
             j = self._post(
                 "/authz/edgetypes", json_data={"edge_type": edge_type.__dict__}
             )
             return EdgeType.from_json(j)
         except UserCloudsSDKError as e:
             if if_not_exists:
@@ -878,15 +929,15 @@
         params["version"] = "3"
         j = self._get("/authz/organizations", params=params)
 
         organizations = [Organization.from_json(o) for o in j["data"]]
         return organizations
 
     def CreateOrganization(
-        self, organization: Organization, if_not_exists=False
+        self, organization: Organization, if_not_exists: bool = False
     ) -> Organization:
         try:
             json_data = self._post(
                 "/authz/organizations",
                 json_data={"organization": organization.__dict__},
             )
             return Organization.from_json(json_data)
@@ -925,14 +976,29 @@
 
     def GetExternalOIDCIssuers(self) -> list[str]:
         return self._get("/userstore/oidcissuers")
 
     def UpdateExternalOIDCIssuers(self, issuers: list[str]) -> list[str]:
         return self._put("/userstore/oidcissuers", json_data=issuers)
 
+    def UploadDataImportFile(
+        self, file_path: Path, import_type: str = "executemutator"
+    ) -> uuid.UUID:
+        json_data = self._get(f"/userstore/upload/dataimport?import_type={import_type}")
+        import_id = uuid.UUID(json_data["import_id"])
+        with open(file_path, "rb") as f:
+            resp = self._client.put(json_data["presigned_url"], content=f)
+            if resp.status_code >= 400:
+                raise UserCloudsSDKError.from_response(resp)
+        return import_id
+
+    def CheckDataImportStatus(self, import_id: uuid.UUID) -> dict:
+        json_data = self._get(f"/userstore/upload/dataimport/{import_id}")
+        return json_data
+
     # Access Token Helpers
 
     def _get_access_token(self) -> str:
         # Encode the client ID and client secret
         headers = {
             "Authorization": f"Basic {self._authorization}",
             "Content-Type": "application/x-www-form-urlencoded",
```

### Comparing `usercloudssdk-1.6.0/src/usercloudssdk/client_helpers.py` & `usercloudssdk-1.7.0/src/usercloudssdk/client_helpers.py`

 * *Files identical despite different names*

### Comparing `usercloudssdk-1.6.0/src/usercloudssdk/client_test.py` & `usercloudssdk-1.7.0/src/usercloudssdk/client_test.py`

 * *Files identical despite different names*

### Comparing `usercloudssdk-1.6.0/src/usercloudssdk/constants.py` & `usercloudssdk-1.7.0/src/usercloudssdk/constants.py`

 * *Files identical despite different names*

### Comparing `usercloudssdk-1.6.0/src/usercloudssdk/errors.py` & `usercloudssdk-1.7.0/src/usercloudssdk/errors.py`

 * *Files identical despite different names*

### Comparing `usercloudssdk-1.6.0/src/usercloudssdk/models.py` & `usercloudssdk-1.7.0/src/usercloudssdk/models.py`

 * *Files 10% similar despite different names*

```diff
@@ -134,14 +134,164 @@
         if hasattr(self, "name"):
             rsc_id["name"] = self.name
         if not rsc_id:
             raise ValueError("ResourceID is empty")
         return rsc_id
 
 
+class CompositeField:
+    data_type: ResourceID
+    name: str
+    camel_case_name: str
+    struct_name: str
+    required: bool
+    ignore_for_uniqueness: bool
+
+    def __init__(
+        self,
+        data_type: ResourceID,
+        name: str,
+        camel_case_name: str = "",
+        struct_name: str = "",
+        required: bool = False,
+        ignore_for_uniqueness: bool = False,
+    ) -> None:
+        self.data_type = data_type
+        self.name = name
+        self.camel_case_name = camel_case_name
+        self.struct_name = struct_name
+        self.required = required
+        self.ignore_for_uniqueness = ignore_for_uniqueness
+
+    def __str__(self) -> str:
+        return f"CompositeField: {self.name} [{self.data_type}]"
+
+    def __repr__(self) -> str:
+        return f"CompositeField(data_type={self.data_type}, name={self.name}, camel_case_name={self.camel_case_name}, struct_name={self.struct_name}, required={self.required}, ignore_for_uniqueness={self.ignore_for_uniqueness})"
+
+    def to_json(self) -> str:
+        return ucjson.dumps(
+            {
+                "data_type": self.data_type,
+                "name": self.name,
+                "camel_case_name": self.camel_case_name,
+                "struct_name": self.struct_name,
+                "required": self.required,
+                "ignore_for_uniqueness": self.ignore_for_uniqueness,
+            }
+        )
+
+    @classmethod
+    def from_json(cls, json_data: dict) -> ColumnField:
+        return cls(
+            data_type=ResourceID.from_json(json_data["data_type"]),
+            name=json_data["name"],
+            camel_case_name=json_data["camel_case_name"],
+            struct_name=json_data["struct_name"],
+            required=json_data["required"],
+            ignore_for_uniqueness=json_data["ignore_for_uniqueness"],
+        )
+
+
+class CompositeAttributes:
+    include_id: bool
+    fields: list[CompositeField]
+
+    def __init__(
+        self,
+        include_id: bool,
+        fields: list[CompositeField],
+    ) -> None:
+        self.include_id = include_id
+        self.fields = fields
+
+    def __str__(self) -> str:
+        return (
+            f"CompositeAttributes: include_id={self.include_id}, fields={self.fields}"
+        )
+
+    def __repr__(self) -> str:
+        return f"CompsositeAttributes(include_id={self.include_id}, fields={self.fields!r})"
+
+    def to_json(self) -> str:
+        return ucjson.dumps(
+            {
+                "include_id": self.include_id,
+                "fields": [field.to_json() for field in self.fields],
+            }
+        )
+
+    @classmethod
+    def from_json(cls, json_data: dict) -> CompositeAttributes:
+        return cls(
+            include_id=json_data["include_id"],
+            fields=json_data["fields"],
+        )
+
+
+class ColumnDataType:
+    id: uuid.UUID
+    name: str
+    description: str
+    is_composite_field_type: bool
+    is_native: bool
+    composite_attributes: CompositeAttributes
+
+    def __init__(
+        self,
+        id: uuid.UUID,
+        name: str,
+        description: str,
+        is_composite_field_type: bool = False,
+        is_native: bool = False,
+        composite_attributes: CompositeAttributes | None = None,
+    ) -> None:
+        self.id = id
+        self.name = name
+        self.description = description
+        self.is_composite_field_type = is_composite_field_type
+        self.is_native = is_native
+        if composite_attributes is None:
+            self.composite_attributes = CompositeAttributes(
+                include_id=False,
+                fields=[],
+            )
+        else:
+            self.composite_attributes = composite_attributes
+
+    def to_json(self) -> str:
+        return ucjson.dumps(
+            {
+                "id": str(self.id),
+                "name": self.name,
+                "description": self.description,
+                "is_composite_field_type": self.is_composite_field_type,
+                "is_native": self.is_native,
+                "composite_attributes": self.composite_attributes,
+            }
+        )
+
+    @classmethod
+    def from_json(cls, json_data: dict) -> ColumnDataType:
+        return cls(
+            id=uuid.UUID(json_data["id"]),
+            name=json_data["name"],
+            description=json_data["description"],
+            is_composite_field_type=json_data["is_composite_field_type"],
+            is_native=json_data["is_native"],
+            composite_attributes=json_data["composite_attributes"],
+        )
+
+    def __str__(self) -> str:
+        return f"ColumnDataType {self.name} [{self.description}] - {self.id}"
+
+    def __repr__(self) -> str:
+        return f"ColumnDataType(id={self.id}, name={self.name}, description={self.description})"
+
+
 class ColumnField:
     type: DataType
     name: str
     camel_case_name: str
     struct_name: str
     required: bool
     ignore_for_uniqueness: bool
@@ -190,121 +340,136 @@
             required=json_data["required"],
             ignore_for_uniqueness=json_data["ignore_for_uniqueness"],
         )
 
 
 class ColumnConstraints:
     immutable_required: bool
+    partial_updates: bool
     unique_id_required: bool
     unique_required: bool
     fields: list[ColumnField]
 
     def __init__(
         self,
         immutable_required: bool,
+        partial_updates: bool,
         unique_id_required: bool,
         unique_required: bool,
         fields: list[ColumnField],
     ) -> None:
         self.immutable_required = immutable_required
+        self.partial_updates = partial_updates
         self.unique_id_required = unique_id_required
         self.unique_required = unique_required
         self.fields = fields
 
     def __str__(self) -> str:
-        return f"ColumnConstraints: immutable_required={self.immutable_required}, unique_id_required={self.unique_id_required}, unique_required={self.unique_required}, fields={self.fields}"
+        return f"ColumnConstraints: immutable_required={self.immutable_required}, partial_updates={self.partial_updates}, unique_id_required={self.unique_id_required}, unique_required={self.unique_required}, fields={self.fields}"
 
     def __repr__(self) -> str:
-        return f"ColumnConstraints(immutable_required={self.immutable_required}, unique_id_required={self.unique_id_required}, unique_required={self.unique_required}, fields={self.fields!r})"
+        return f"ColumnConstraints(immutable_required={self.immutable_required}, partial_updates={self.partial_updates}, unique_id_required={self.unique_id_required}, unique_required={self.unique_required}, fields={self.fields!r})"
 
     def to_json(self) -> str:
         return ucjson.dumps(
             {
                 "immutable_required": self.immutable_required,
+                "partial_updates": self.partial_updates,
                 "unique_id_required": self.unique_id_required,
                 "unique_required": self.unique_required,
-                "fields": self.fields,
+                "fields": [field.to_json() for field in self.fields],
             }
         )
 
     @classmethod
     def from_json(cls, json_data: dict) -> ColumnConstraints:
         return cls(
             immutable_required=json_data["immutable_required"],
+            partial_updates=(
+                json_data["partial_updates"]
+                if "partial_updates" in json_data
+                else False
+            ),
             unique_id_required=json_data["unique_id_required"],
             unique_required=json_data["unique_required"],
             fields=json_data["fields"],
         )
 
 
 class Column:
     id: uuid.UUID
     name: str
+    data_type: ResourceID | None
     type: DataType
     is_array: bool
     default_value: str
     index_type: ColumnIndexType
     constraints: ColumnConstraints
 
     def __init__(
         self,
         id: uuid.UUID,
         name: str,
         type: str | DataType,
         is_array: bool,
         default_value: str,
         index_type: str | ColumnIndexType,
+        data_type: ResourceID | None = None,
         constraints: ColumnConstraints | None = None,
     ) -> None:
         self.id = id
         self.name = name
+        self.data_type = data_type
         self.type = DataType(type)
         self.is_array = is_array
         self.default_value = default_value
         self.index_type = ColumnIndexType(index_type)
         if constraints is None:
             self.constraints = ColumnConstraints(
                 immutable_required=False,
+                partial_updates=False,
                 unique_id_required=False,
                 unique_required=False,
                 fields=[],
             )
         else:
             self.constraints = constraints
 
     def to_json(self) -> str:
         return ucjson.dumps(
             {
                 "id": str(self.id),
                 "name": self.name,
+                "data_type": self.data_type,
                 "type": self.type.value,
                 "is_array": self.is_array,
                 "default_value": self.default_value,
                 "index_type": self.index_type.value,
                 "constraints": self.constraints,
             }
         )
 
     @classmethod
     def from_json(cls, json_data: dict) -> Column:
         return cls(
             id=uuid.UUID(json_data["id"]),
             name=json_data["name"],
+            data_type=ResourceID.from_json(json_data["data_type"]),
             type=DataType(json_data["type"]),
             is_array=json_data["is_array"],
             default_value=json_data["default_value"],
             index_type=ColumnIndexType(json_data["index_type"]),
             constraints=json_data["constraints"],
         )
 
     def __str__(self) -> str:
-        return f"Column {self.name} [{self.type}] - {self.id}"
+        return f"Column {self.name} [{self.type}] [{self.data_type}] - {self.id}"
 
     def __repr__(self) -> str:
-        return f"Column(id={self.id}, name={self.name}, type={self.type})"
+        return f"Column(id={self.id}, name={self.name}, data_type={self.data_type}, type={self.type})"
 
 
 class Purpose:
     id: uuid.UUID
     name: str
     description: str
 
@@ -662,56 +827,64 @@
             ],
         )
 
 
 class Transformer:
     id: uuid.UUID
     name: str
+    input_data_type: ResourceID | None
     input_type: DataType
     input_type_constraints: ColumnConstraints
+    output_data_type: ResourceID | None
     output_type: DataType
     output_type_constraints: ColumnConstraints
     reuse_existing_token: bool
     transform_type: TransformType
     function: str
     parameters: str
 
     def __init__(
         self,
         id: uuid.UUID = uuid.UUID(int=0),
         name: str = "",
+        input_data_type: ResourceID | None = None,
         input_type: str | DataType = DataType.STRING,
+        output_data_type: ResourceID | None = None,
         output_type: str | DataType = DataType.STRING,
         reuse_existing_token: bool = False,
         transform_type: str | TransformType = TransformType.PASSTHROUGH,
         function: str = "",
         parameters: str = "",
         input_type_constraints: ColumnConstraints | None = None,
         output_type_constraints: ColumnConstraints | None = None,
     ) -> None:
         self.id = id
         self.name = name
+        self.input_data_type = input_data_type
         self.input_type = DataType(input_type)
+        self.output_data_type = output_data_type
         self.output_type = DataType(output_type)
         self.reuse_existing_token = reuse_existing_token
         self.transform_type = TransformType(transform_type)
         self.function = function
         self.parameters = parameters
         if input_type_constraints is None:
             self.input_type_constraints = ColumnConstraints(
                 immutable_required=False,
+                partial_updates=False,
                 unique_id_required=False,
                 unique_required=False,
                 fields=[],
             )
         else:
             self.input_type_constraints = input_type_constraints
         if output_type_constraints is None:
             self.output_type_constraints = ColumnConstraints(
                 immutable_required=False,
+                partial_updates=False,
                 unique_id_required=False,
                 unique_required=False,
                 fields=[],
             )
         else:
             self.output_type_constraints = output_type_constraints
 
@@ -722,36 +895,40 @@
         return f"Transformer {self.name} - {self.id}"
 
     def to_json(self) -> str:
         return ucjson.dumps(
             {
                 "id": str(self.id),
                 "name": self.name,
+                "input_data_type": self.input_data_type,
                 "input_type": self.input_type.value,
                 "input_type_constraints": self.input_type_constraints,
+                "output_data_type": self.output_data_type,
                 "output_type": self.output_type.value,
                 "output_type_constraints": self.output_type_constraints,
                 "reuse_existing_token": self.reuse_existing_token,
                 "transform_type": self.transform_type.value,
                 "function": self.function,
                 "parameters": self.parameters,
             },
         )
 
     @classmethod
     def from_json(cls, json_data: dict) -> Transformer:
         return cls(
             id=uuid.UUID(json_data["id"]),
             name=json_data["name"],
+            input_data_type=ResourceID.from_json(json_data["input_data_type"]),
             input_type=DataType(json_data["input_type"]),
             input_type_constraints=(
                 json_data["input_type_constraints"]
                 if "input_type_constraints" in json_data
                 else None
             ),
+            output_data_type=ResourceID.from_json(json_data["output_data_type"]),
             output_type=DataType(json_data["output_type"]),
             output_type_constraints=(
                 json_data["output_type_constraints"]
                 if "output_type_constraints" in json_data
                 else None
             ),
             reuse_existing_token=json_data["reuse_existing_token"],
```

### Comparing `usercloudssdk-1.6.0/src/usercloudssdk/policies.py` & `usercloudssdk-1.7.0/src/usercloudssdk/policies.py`

 * *Files identical despite different names*

### Comparing `usercloudssdk-1.6.0/src/usercloudssdk/uchttpclient.py` & `usercloudssdk-1.7.0/src/usercloudssdk/uchttpclient.py`

 * *Files identical despite different names*

### Comparing `usercloudssdk-1.6.0/src/usercloudssdk/ucjson.py` & `usercloudssdk-1.7.0/src/usercloudssdk/ucjson.py`

 * *Files 16% similar despite different names*

```diff
@@ -13,12 +13,12 @@
         return str(obj)
     elif isinstance(obj, Enum):
         return obj.value
     return obj.__dict__
 
 
 def loads(data: str) -> dict:
-    return json.loads(data)
+    return json.loads(data) if data else {}
 
 
 def dumps(data: dict) -> str:
     return json.dumps(data, default=serializer, ensure_ascii=False)
```

### Comparing `usercloudssdk-1.6.0/src/usercloudssdk.egg-info/SOURCES.txt` & `usercloudssdk-1.7.0/src/usercloudssdk.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,17 @@
+LICENSE
 README.md
 pyproject.toml
 src/usercloudssdk/__init__.py
 src/usercloudssdk/asyncclient.py
 src/usercloudssdk/client.py
 src/usercloudssdk/client_helpers.py
 src/usercloudssdk/client_test.py
 src/usercloudssdk/constants.py
+src/usercloudssdk/data_types.py
 src/usercloudssdk/errors.py
 src/usercloudssdk/models.py
 src/usercloudssdk/policies.py
 src/usercloudssdk/uchttpclient.py
 src/usercloudssdk/ucjson.py
 src/usercloudssdk.egg-info/PKG-INFO
 src/usercloudssdk.egg-info/SOURCES.txt
```

