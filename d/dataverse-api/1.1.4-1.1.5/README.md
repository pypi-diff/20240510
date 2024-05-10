# Comparing `tmp/dataverse_api-1.1.4.tar.gz` & `tmp/dataverse_api-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dataverse_api-1.1.4.tar", max compression
+gzip compressed data, was "dataverse_api-1.1.5.tar", max compression
```

## Comparing `dataverse_api-1.1.4.tar` & `dataverse_api-1.1.5.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0      213 2024-03-12 13:18:24.297150 dataverse_api-1.1.4/dataverse_api/__init__.py
--rw-r--r--   0        0        0     7066 2024-03-12 13:18:24.297150 dataverse_api-1.1.4/dataverse_api/_api.py
--rw-r--r--   0        0        0    11505 2024-03-12 13:18:24.298152 dataverse_api-1.1.4/dataverse_api/dataverse.py
--rw-r--r--   0        0        0    28222 2024-03-18 21:04:55.984984 dataverse_api-1.1.4/dataverse_api/entity.py
--rw-r--r--   0        0        0      899 2024-03-12 13:18:24.299152 dataverse_api-1.1.4/dataverse_api/errors.py
--rw-r--r--   0        0        0        0 2024-03-12 13:18:24.300151 dataverse_api-1.1.4/dataverse_api/metadata/__init__.py
--rw-r--r--   0        0        0     7375 2024-03-12 13:18:24.300151 dataverse_api-1.1.4/dataverse_api/metadata/attributes.py
--rw-r--r--   0        0        0     1719 2024-03-12 13:18:24.301152 dataverse_api-1.1.4/dataverse_api/metadata/base.py
--rw-r--r--   0        0        0     5269 2024-03-12 13:18:24.301152 dataverse_api-1.1.4/dataverse_api/metadata/complex_properties.py
--rw-r--r--   0        0        0     3563 2024-03-12 13:18:24.302152 dataverse_api-1.1.4/dataverse_api/metadata/entity.py
--rw-r--r--   0        0        0     3113 2024-03-12 13:18:24.302152 dataverse_api-1.1.4/dataverse_api/metadata/enums.py
--rw-r--r--   0        0        0     2006 2024-03-12 13:18:24.303657 dataverse_api-1.1.4/dataverse_api/metadata/helpers.py
--rw-r--r--   0        0        0     3590 2024-03-12 13:18:24.303657 dataverse_api-1.1.4/dataverse_api/metadata/relationships.py
--rw-r--r--   0        0        0     1751 2024-03-12 13:18:24.304664 dataverse_api-1.1.4/dataverse_api/schema.py
--rw-r--r--   0        0        0        0 2024-03-12 13:18:24.305663 dataverse_api-1.1.4/dataverse_api/utils/__init__.py
--rw-r--r--   0        0        0     6699 2024-03-12 13:18:24.306664 dataverse_api-1.1.4/dataverse_api/utils/batching.py
--rw-r--r--   0        0        0      832 2024-03-12 13:18:24.308664 dataverse_api-1.1.4/dataverse_api/utils/data.py
--rw-r--r--   0        0        0     1351 2024-03-12 13:18:24.309664 dataverse_api-1.1.4/dataverse_api/utils/labels.py
--rw-r--r--   0        0        0     2735 2024-03-12 13:18:24.310664 dataverse_api-1.1.4/dataverse_api/utils/text.py
--rw-r--r--   0        0        0     1093 2024-03-12 13:18:24.293773 dataverse_api-1.1.4/LICENSE
--rw-r--r--   0        0        0      934 2024-03-18 21:06:42.981367 dataverse_api-1.1.4/pyproject.toml
--rw-r--r--   0        0        0    10312 2024-03-12 13:18:24.295152 dataverse_api-1.1.4/README.md
--rw-r--r--   0        0        0    10758 1970-01-01 00:00:00.000000 dataverse_api-1.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-05-13 11:36:09.341892 dataverse_api-1.1.5/LICENSE
+-rw-r--r--   0        0        0    10039 2024-05-10 18:52:35.770563 dataverse_api-1.1.5/README.md
+-rw-r--r--   0        0        0      210 2024-01-25 20:34:23.277067 dataverse_api-1.1.5/dataverse_api/__init__.py
+-rw-r--r--   0        0        0     6835 2024-05-10 18:47:53.928202 dataverse_api-1.1.5/dataverse_api/_api.py
+-rw-r--r--   0        0        0    11136 2024-01-25 20:34:23.277847 dataverse_api-1.1.5/dataverse_api/dataverse.py
+-rw-r--r--   0        0        0    29110 2024-05-10 18:50:03.240534 dataverse_api-1.1.5/dataverse_api/entity.py
+-rw-r--r--   0        0        0      863 2024-01-25 20:34:23.278340 dataverse_api-1.1.5/dataverse_api/errors.py
+-rw-r--r--   0        0        0        0 2024-01-25 20:34:23.278433 dataverse_api-1.1.5/dataverse_api/metadata/__init__.py
+-rw-r--r--   0        0        0     7126 2024-01-25 20:34:23.278650 dataverse_api-1.1.5/dataverse_api/metadata/attributes.py
+-rw-r--r--   0        0        0     1658 2024-01-25 20:34:23.278796 dataverse_api-1.1.5/dataverse_api/metadata/base.py
+-rw-r--r--   0        0        0     5089 2024-01-26 21:31:45.311000 dataverse_api-1.1.5/dataverse_api/metadata/complex_properties.py
+-rw-r--r--   0        0        0     3449 2024-01-26 21:58:12.714536 dataverse_api-1.1.5/dataverse_api/metadata/entity.py
+-rw-r--r--   0        0        0     2975 2024-01-25 20:34:23.279380 dataverse_api-1.1.5/dataverse_api/metadata/enums.py
+-rw-r--r--   0        0        0     1933 2024-01-25 20:34:23.279726 dataverse_api-1.1.5/dataverse_api/metadata/helpers.py
+-rw-r--r--   0        0        0     3489 2024-01-25 20:34:23.279922 dataverse_api-1.1.5/dataverse_api/metadata/relationships.py
+-rw-r--r--   0        0        0      201 2024-05-10 18:48:54.519145 dataverse_api-1.1.5/dataverse_api/schema.py
+-rw-r--r--   0        0        0        0 2024-01-25 20:34:23.280166 dataverse_api-1.1.5/dataverse_api/utils/__init__.py
+-rw-r--r--   0        0        0     6460 2024-05-10 18:47:53.928863 dataverse_api-1.1.5/dataverse_api/utils/batching.py
+-rw-r--r--   0        0        0     1725 2024-05-10 18:49:09.081914 dataverse_api-1.1.5/dataverse_api/utils/data.py
+-rw-r--r--   0        0        0     1316 2024-01-25 20:34:23.280651 dataverse_api-1.1.5/dataverse_api/utils/labels.py
+-rw-r--r--   0        0        0     2635 2024-01-25 20:34:23.280787 dataverse_api-1.1.5/dataverse_api/utils/text.py
+-rw-r--r--   0        0        0      915 2024-05-10 18:53:48.339904 dataverse_api-1.1.5/pyproject.toml
+-rw-r--r--   0        0        0    10746 1970-01-01 00:00:00.000000 dataverse_api-1.1.5/PKG-INFO
```

### Comparing `dataverse_api-1.1.4/dataverse_api/entity.py` & `dataverse_api-1.1.5/dataverse_api/entity.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,820 +1,868 @@
-import logging
-from collections.abc import Collection, Iterable, Mapping, MutableMapping, Sequence
-from copy import copy
-from typing import Any, Literal, overload
-
-import pandas as pd
-import requests
-
-from dataverse_api._api import Dataverse
-from dataverse_api.errors import DataverseError, DataverseModeError
-from dataverse_api.metadata.base import BASE_TYPE, MetadataDumper
-from dataverse_api.metadata.complex_properties import Label
-from dataverse_api.metadata.entity import get_altkey_metadata
-from dataverse_api.utils.batching import (
-    APICommand,
-    RequestMethod,
-    chunk_data,
-    transform_to_batch_for_create,
-    transform_to_batch_for_delete,
-    transform_to_batch_for_upsert,
-    transform_upsert_data,
-)
-from dataverse_api.utils.data import convert_dataframe_to_dict
-
-
-class DataverseEntity(Dataverse):
-    def __init__(
-        self,
-        session: requests.Session,
-        environment_url: str,
-        logical_name: str,
-    ):
-        super().__init__(session=session, environment_url=environment_url)
-
-        self.__logical_name = logical_name
-        self.__supports_create_multiple = False
-        self.__supports_update_multiple = False
-
-        # Populate entity properties
-        self.update_schema()
-
-    @property
-    def logical_name(self) -> str:
-        return self.__logical_name
-
-    @property
-    def entity_set_name(self) -> str:
-        return self.__entity_set_name
-
-    @property
-    def primary_id_attr(self) -> str:
-        return self.__primary_id_attr
-
-    @property
-    def primary_img_attr(self) -> str | None:
-        return self.__primary_img_attr
-
-    @property
-    def alternate_keys(self) -> dict[str, list[str]]:
-        return self.__alternate_keys
-
-    @property
-    def supports_create_multiple(self) -> bool:
-        return self.__supports_create_multiple
-
-    @property
-    def supports_update_multiple(self) -> bool:
-        return self.__supports_update_multiple
-
-    def __get_entity_set_properties(self) -> None:
-        """
-        Fetch key attributes of the Entity.
-
-          - `EntitySetName`, used as the API endpoint
-          - `PrimaryIdAttribute`, the primary ID column
-          - `PrimaryImageAttribute`, the primary image column (if any)
-
-        Returns
-        -------
-        EntityData
-            A dataclass with the three relevant attributes.
-        """
-        columns = ["EntitySetName", "PrimaryIdAttribute", "PrimaryImageAttribute"]
-        logging.debug("Retrieving EntityDefinitions for %s", self.logical_name)
-        resp = self._api_call(
-            method=RequestMethod.GET,
-            url=f"EntityDefinitions(LogicalName='{self.logical_name}')",
-            params={"$select": ",".join(columns)},
-        ).json()
-
-        self.__entity_set_name = resp["EntitySetName"]
-        self.__primary_id_attr = resp["PrimaryIdAttribute"]
-        self.__primary_img_attr = resp.get("PrimaryImageAttribute")
-
-    def __get_entity_alternate_keys(self) -> None:
-        """
-        Fetch the alternate keys (if any) for the Entity.
-        """
-        columns = ["SchemaName", "KeyAttributes"]
-        logging.debug("Retrieving alternate keys for %s", self.logical_name)
-        resp = self._api_call(
-            method=RequestMethod.GET,
-            url=f"EntityDefinitions(LogicalName='{self.logical_name}')/Keys",
-            params={"$select": ",".join(columns)},
-        ).json()["value"]
-
-        self.__alternate_keys = {r["SchemaName"]: r["KeyAttributes"] for r in resp}
-
-    def __get_entity_sdk_messages(self) -> None:
-        """
-        Fetch sdk messages to determine whether entity supports certain actions.
-        """
-        create, update = "CreateMultiple", "UpdateMultiple"
-        actions = [create, update]
-        col = "primaryobjecttypecode"
-        msg_col = "sdkmessageid/name"
-
-        params: dict[str, str] = dict()
-        params["$select"] = "sdkmessagefilterid"
-        params["$expand"] = "sdkmessageid($select=name)"
-        params[
-            "$filter"
-        ] = f"""({' or '.join(f"{msg_col} eq '{x}'" for x in actions)}) and {col} eq '{self.logical_name}'"""
-
-        logging.debug("Retrieving SDK messages for %s", self.logical_name)
-        resp = self._api_call(
-            method=RequestMethod.GET,
-            url="sdkmessagefilters",
-            params=params,
-        ).json()["value"]
-        returned_actions = {row["sdkmessageid"]["name"] for row in resp}
-
-        if create in returned_actions:
-            self.__supports_create_multiple = True
-        if update in returned_actions:
-            self.__supports_update_multiple = True
-
-    def update_schema(self, arg: Literal["altkeys", "properties", "messages"] | None = None) -> None:
-        """
-        Update schema.
-        """
-        if arg == "altkeys":
-            self.__get_entity_alternate_keys()
-            return
-
-        self.__get_entity_alternate_keys()
-        self.__get_entity_sdk_messages()
-        self.__get_entity_set_properties()
-
-    @overload
-    def read(
-        self,
-        *,
-        select: Collection[str] | None = None,
-        top: int | None = None,
-        filter: str | None = None,
-        page_size: int | None = None,
-        expand: str | None = None,
-        order_by: str | None = None,
-    ) -> list[dict[str, Any]]:
-        ...
-
-    @overload
-    def read(
-        self,
-        *,
-        select: Collection[str] | None = None,
-        top: int | None = None,
-        filter: str | None = None,
-        page_size: int | None = None,
-        expand: str | None = None,
-        order_by: str | None = None,
-        return_responses: Literal[True],
-    ) -> list[requests.Response]:
-        ...
-
-    def read(
-        self,
-        *,
-        select: Collection[str] | None = None,
-        top: int | None = None,
-        filter: str | None = None,
-        page_size: int | None = None,
-        expand: str | None = None,
-        order_by: str | None = None,
-        return_responses: bool = False,
-    ) -> list[dict[str, Any]] | list[requests.Response]:
-        """
-        Read data from Entity.
-
-        Parameters
-        ----------
-        select : Collection[str]
-            Columns to return in the query.
-        top : int
-            Optional limit on returned records.
-        filter : str
-            A fully qualified filtering string.
-        expand : str
-            A fully qualified expand string.
-        orderby : str
-            A fully qualified order_by string.
-        apply : str
-            A fully qualified string describing aggregation and grouping of returned records.
-        page_size : int
-            Limits the total number of records retrieved per API call.
-        return_responses : bool
-            Returns complete responses instead of data records.
-
-        Returns
-        -------
-        list[dict[str, Any]]
-            The extended "value" element for all response-JSONs from server.
-        """
-
-        additional_headers: dict[str, str] = dict()
-        if page_size is not None:
-            additional_headers["Prefer"] = f"odata.maxpagesize={page_size}"
-
-        params: dict[str, Any] = dict()
-        if select:
-            params["$select"] = ",".join(select)
-        if filter:
-            params["$filter"] = filter
-        if top:
-            params["$top"] = top
-        if order_by:
-            params["$orderby"] = order_by
-        if expand:
-            params["$expand"] = expand
-
-        output: list[requests.Response] = list()
-        url = self.entity_set_name
-
-        # Looping through pages
-        logging.debug("Fetching data for read operation on %s.", self.logical_name)
-        response = self._api_call(
-            method=RequestMethod.GET,
-            url=url,
-            headers=additional_headers,
-            params=params,
-        )
-        output.append(response)
-        while response.json().get("@odata.nextLink"):
-            response = self._api_call(method=RequestMethod.GET, url=response.json()["@odata.nextLink"])
-            output.append(response)
-
-        if return_responses:
-            logging.debug("Fetched all data for read operation, %d responses.", len(output))
-            return output
-        else:
-            data_output: list[dict[str, Any]] = []
-            for resp in output:
-                data_output.extend(resp.json()["value"])
-            logging.debug("Fetched all data for read operation, %d elements.", len(data_output))
-            return data_output
-
-    @overload
-    def create(
-        self,
-        data: Sequence[MutableMapping[str, Any]] | pd.DataFrame,
-        *,
-        mode: Literal["individual", "multiple"] = "individual",
-        detect_duplicates: bool = False,
-        return_created: bool = False,
-        threading: bool = False,
-    ) -> list[requests.Response]:
-        ...
-
-    @overload
-    def create(
-        self,
-        data: Sequence[MutableMapping[str, Any]] | pd.DataFrame,
-        *,
-        mode: Literal["batch"],
-        detect_duplicates: bool = False,
-        return_created: bool = False,
-        batch_size: int | None = None,
-        threading: bool = False,
-    ) -> list[requests.Response]:
-        ...
-
-    def create(
-        self,
-        data: Sequence[MutableMapping[str, Any]] | pd.DataFrame,
-        *,
-        mode: Literal["individual", "multiple", "batch"] = "individual",
-        detect_duplicates: bool = False,
-        return_created: bool = False,
-        batch_size: int | None = None,
-        threading: bool = False,
-    ) -> list[requests.Response]:
-        """
-        Create rows in Dataverse Entity. Failures will occur if trying to insert
-        a record where alternate key already exists, partial success is possible.
-
-        data : Sequence[MutableMapping[str, Any] | pd.DataFrame
-            The data to create in Dataverse, JSON serializable.
-        mode : Literal["individual", "multiple", "batch"]
-            Whether to create rows using individual requests, `CreateMultiple` web API action
-            or as batch requests using the `$batch` endpoint.
-        detect_duplicates : bool
-            Whether Dataverse will run duplicate detection rules upon insertion.
-        return_created : bool
-            Whether the returned list of Responses will contain information on
-            created rows.
-        batch_size : int
-            Optional override if batch mode is specified, useful for tuning workload
-            per batch if 429s occur.
-        """
-        if isinstance(data, pd.DataFrame):
-            data = convert_dataframe_to_dict(data)
-
-        headers: dict[str, str] = dict()
-        if detect_duplicates:
-            headers["MSCRM.SuppressDuplicateDetection"] = "false"
-
-        if return_created:
-            headers["Prefer"] = "return=representation"
-
-        length = len(data)
-        if mode == "individual":
-            logging.debug("%d rows to insert using individual inserts.", length)
-            return self.__create_singles(headers=headers, data=data, threading=threading)
-
-        if mode == "multiple":
-            if not self.supports_create_multiple:
-                raise DataverseError(f"CreateMultiple is not supported by {self.logical_name}. Use a different mode.")
-            logging.debug("%d rows to insert using CreateMultiple.", length)
-            return self.__create_multiple(headers=headers, data=data, threading=threading)
-
-        if mode == "batch":
-            logging.debug(
-                "%d rows to insert using batch insertion.",
-                length,
-            )
-            return self.__create_batch(data=data, batch_size=batch_size, threading=threading)
-
-        raise DataverseModeError(mode, "individual", "multiple", "batch")
-
-    def __create_singles(
-        self,
-        data: Collection[MutableMapping[str, Any]],
-        headers: Mapping[str, str],
-        threading: bool,
-    ) -> list[requests.Response]:
-        """
-        Insert rows one by one using threaded API call.
-        """
-        calls = [
-            APICommand(
-                method=RequestMethod.POST,
-                url=self.entity_set_name,
-                headers=headers,
-                json=row,
-            )
-            for row in data
-        ]
-
-        if threading:
-            return self._threaded_call(calls=calls)
-        return self._individual_call(calls=calls)
-
-    def __create_multiple(
-        self, headers: Mapping[str, str], data: Sequence[MutableMapping[str, Any]], threading: bool
-    ) -> list[requests.Response]:
-        """
-        Insert rows by using the `CreateMultiple` Web API Action.
-        """
-        # Preserving input data
-        data = copy(data)
-
-        # Adding odata type to each record
-        for row in data:
-            row["@odata.type"] = BASE_TYPE + self.logical_name
-
-        # Chunking the payload to suggested size
-        calls = [
-            APICommand(
-                method=RequestMethod.POST,
-                url=f"{self.entity_set_name}/{BASE_TYPE}CreateMultiple",
-                headers=headers,
-                json={"Targets": rows},
-            )
-            for rows in chunk_data(data=data, size=500)
-        ]
-
-        if threading:
-            return self._threaded_call(calls)
-        return self._individual_call(calls)
-
-    def __create_batch(
-        self, data: Collection[MutableMapping[str, Any]], batch_size: int | None, threading: bool
-    ) -> list[requests.Response]:
-        """
-        Run a batch insert operation on the given data.
-        """
-        batch_data = transform_to_batch_for_create(url=self.entity_set_name, data=data)
-        return self._batch_api_call(batch_data, batch_size=batch_size, threading=threading)
-
-    def __delete_singles(self, data: Iterable[str], threading: bool) -> list[requests.Response]:
-        calls = [
-            APICommand(
-                method=RequestMethod.DELETE,
-                url=f"{self.entity_set_name}({id})",
-            )
-            for id in data
-        ]
-
-        if threading:
-            return self._threaded_call(calls=calls)
-        return self._individual_call(calls=calls)
-
-    @overload
-    def delete(
-        self,
-        *,
-        mode: Literal["individual"] = "individual",
-        ids: Collection[str],
-    ) -> list[requests.Response]:
-        ...
-
-    @overload
-    def delete(
-        self,
-        *,
-        mode: Literal["individual"] = "individual",
-        filter: str,
-        threading: bool = False,
-    ) -> list[requests.Response]:
-        ...
-
-    @overload
-    def delete(
-        self, *, mode: Literal["batch"], filter: str, batch_size: int | None = None, threading: bool = False
-    ) -> list[requests.Response]:
-        ...
-
-    @overload
-    def delete(
-        self, *, mode: Literal["batch"], ids: Collection[str], batch_size: int | None = None, threading: bool = False
-    ) -> list[requests.Response]:
-        ...
-
-    def delete(
-        self,
-        *,
-        mode: Literal["individual", "batch"] = "individual",
-        ids: Collection[str] | None = None,
-        filter: str | None = None,
-        batch_size: int | None = None,
-        threading: bool = False,
-    ) -> list[requests.Response]:
-        """
-        Delete rows in Entity.
-
-        Specify either a list of ID's for deletion or a filter
-        string for determining which records to delete.
-
-        Parameters
-        ----------
-        mode : Literal["individual","batch"]
-            Whether to delete rows using individual requests or batch requests.
-        ids : Collection[str]
-            List of primary IDs to delete. Takes precedence if passed.
-        filter : str
-            Filter statement for targeting specific records in Entity
-            for deletion. Use `filter="all"` to delete all records.
-        batch_size : int
-            Optional override if batch mode is specified, useful for tuning workload
-            per batch if 429s occur.
-        """
-        if ids is None and filter is None:
-            raise DataverseError("Function requires either ids to delete or a string passed as filter.")
-
-        if filter == "all":
-            filter = None
-
-        if ids is None:
-            records = self.read(select=[self.primary_id_attr], filter=filter)
-            ids = {row[self.primary_id_attr] for row in records}
-
-        length = len(ids)
-        logging.info("%d rows to delete.", length)
-        if mode == "individual":
-            logging.debug("%d rows to delete using individual deletes.", length)
-            return self.__delete_singles(data=ids, threading=threading)
-
-        if mode == "batch":
-            logging.debug("%d rows to delete using batch deletes.", length)
-            batch_data = transform_to_batch_for_delete(url=self.entity_set_name, data=ids)
-            return self._batch_api_call(batch_data, batch_size=batch_size or 100, timeout=120, threading=threading)
-
-        raise DataverseModeError(mode, "individual", "batch")
-
-    def __delete_column_singles(self, data: Iterable[str], column: str, threading: bool) -> list[requests.Response]:
-        """
-        Delete row column value by individual requests.
-        """
-        calls = [
-            APICommand(
-                method=RequestMethod.DELETE,
-                url=f"{self.entity_set_name}({id})/{column}",
-            )
-            for id in data
-        ]
-        if threading:
-            return self._threaded_call(calls=calls)
-        return self._individual_call(calls=calls)
-
-    @overload
-    def delete_columns(
-        self,
-        columns: Collection[str],
-        *,
-        mode: Literal["individual", "batch"] = "individual",
-        ids: Collection[str],
-        threading: bool,
-    ) -> list[requests.Response]:
-        ...
-
-    @overload
-    def delete_columns(
-        self,
-        columns: Collection[str],
-        *,
-        mode: Literal["individual", "batch"] = "individual",
-        filter: str,
-        threading: bool,
-    ) -> list[requests.Response]:
-        ...
-
-    def delete_columns(
-        self,
-        columns: Collection[str],
-        *,
-        ids: Collection[str] | None = None,
-        filter: str | None = None,
-        mode: Literal["individual", "batch"] = "individual",
-        threading: bool = False,
-    ) -> list[requests.Response]:
-        """
-        Delete values in specific column for rows in Entity.
-
-        Specify either a list of ID's for deletion or a filter
-        string for determining which records to delete.
-
-        Parameters
-        ----------
-        column : Collection[str]
-            The columns in Dataverse to target for deletion.
-        mode : Literal["individual", "batch"]
-            Whether to delete columns using individual requests or batch requests.
-        ids : Collection[str]
-            List of primary IDs to delete. Takes precedence if passed.
-        filter : str
-            Filter statement for targeting specific records in Entity for deletion.
-            Use `filter="all"` to delete all records.
-        """
-        if ids is None and filter is None:
-            raise DataverseError("Function requires either ids to delete or a string passed as filter.")
-
-        if filter == "all":
-            filter = None
-
-        if ids is None:
-            records = self.read(select=[self.primary_id_attr], filter=filter)
-            ids = {row[self.primary_id_attr] for row in records}
-
-        length = len(ids) * len(columns)  # Total number of deletion requests
-        output: list[requests.Response] = []
-        if mode == "individual":
-            logging.debug("%d properties to delete. Using individual deletes.", length)
-            for col in columns:
-                output.extend(self.__delete_column_singles(data=ids, column=col, threading=threading))
-            return output
-
-        if mode == "batch":
-            logging.debug("%d properties to delete. Using batch deletes.", length)
-            for col in columns:
-                batch_data = transform_to_batch_for_delete(url=self.entity_set_name, data=ids, column=col)
-                output.extend(self._batch_api_call(batch_data, threading=threading))
-            return output
-
-        raise DataverseModeError(mode, "individual", "batch")
-
-    def __upsert_singles(
-        self, data: Collection[Mapping[str, Any]], keys: Iterable[str], is_primary_id: bool, threading: bool
-    ) -> list[requests.Response]:
-        """
-        Upsert row by individual requests.
-        """
-        calls = [
-            APICommand(
-                method=RequestMethod.PATCH,
-                url=f"{self.entity_set_name}({key})",
-                json=payload,
-            )
-            for key, payload in transform_upsert_data(data, keys, is_primary_id)
-        ]
-        if threading:
-            return self._threaded_call(calls=calls)
-        return self._individual_call(calls=calls)
-
-    def upsert(
-        self,
-        data: Collection[MutableMapping[str, Any]] | pd.DataFrame,
-        *,
-        mode: Literal["individual", "batch"] = "individual",
-        altkey_name: str | None = None,
-        threading: bool = False,
-    ) -> list[requests.Response]:
-        """
-        Upsert data into Entity.
-
-        Parameters
-        ----------
-        data : Collection[MutableMapping[str, Any]] | pd.DataFrame
-            The data to upsert.
-        mode : Literal["individual", "batch"]
-            Whether to upsert data using individual requests or batch requests.
-        altkey_name : str
-            The alternate key to use as ID (if any).
-            Will assume entity primary ID attribute if not given.
-        """
-
-        if altkey_name is not None:
-            try:
-                key_columns = self.alternate_keys[altkey_name]
-            except KeyError:
-                raise DataverseError(f"Altkey '{altkey_name}' is not valid for Entity '{self.logical_name}'.")
-            is_primary_id = False
-        else:
-            key_columns = [self.primary_id_attr]
-            is_primary_id = True
-
-        if isinstance(data, pd.DataFrame):
-            data = convert_dataframe_to_dict(data)
-
-        if mode == "individual":
-            logging.debug("%d rows to upsert. Using individual upserts.", len(data))
-            return self.__upsert_singles(data=data, keys=key_columns, is_primary_id=is_primary_id, threading=threading)
-
-        if mode == "batch":
-            logging.debug("%d rows to upsert. Using batch upserts.", len(data))
-            batch_data = transform_to_batch_for_upsert(
-                url=self.entity_set_name,
-                data=data,
-                keys=key_columns,
-                is_primary_id=is_primary_id,
-            )
-            return self._batch_api_call(batch_data, threading=threading)
-
-        raise DataverseModeError(mode, "individual", "batch")
-
-    def add_attribute(
-        self,
-        attribute: MetadataDumper,
-        solution_name: str | None = None,
-        return_representation: bool = False,
-    ) -> requests.Response:
-        """
-        Add attribute to Entity.
-
-        Parameters
-        ----------
-        attribute : MetadataDumper
-            Dumpable metadata for new Attribute.
-        solution_name : str
-            Unique name for solution attribute is part of.
-        return_representation : bool
-            Whether to include the metadata representation after
-            creation in the response from server.
-
-        Returns
-        -------
-        requests.Response
-            The response from the server.
-        """
-
-        headers: dict[str, str] = dict()
-
-        if solution_name is not None:
-            headers["MSCRM.SolutionUniqueName"] = solution_name
-
-        if return_representation:
-            headers["Prefer"] = "return=representation"
-
-        return self._api_call(
-            method=RequestMethod.POST,
-            url=f"EntityDefinitions(LogicalName='{self.logical_name}')/Attributes",
-            headers=headers,
-            json=attribute.dump_to_dataverse(),
-        )
-
-    @overload
-    def remove_attribute(self, *, attribute_id: str) -> requests.Response:
-        ...
-
-    @overload
-    def remove_attribute(self, *, logical_name: str) -> requests.Response:
-        ...
-
-    def remove_attribute(
-        self,
-        *,
-        attribute_id: str | None = None,
-        logical_name: str | None = None,
-    ) -> requests.Response:
-        """
-        Remove Attribute from Entity.
-
-        Parameters
-        ----------
-        attribute_id : str
-            GUID of Attribute.
-        logical_name : str
-            LogicalName of Attribute.
-
-        Returns
-        -------
-        requests.Response
-            The response from the server.
-        """
-        if attribute_id is None and logical_name is None:
-            raise DataverseError("Supply either 'id' or 'logical_name' kwarg.")
-
-        if attribute_id:
-            return self._api_call(
-                method=RequestMethod.DELETE,
-                url=f"EntityDefinitions(LogicalName='{self.logical_name}')/Attributes({attribute_id})",
-            )
-
-        return self._api_call(
-            method=RequestMethod.DELETE,
-            url=f"EntityDefinitions(LogicalName='{self.logical_name}')/Attributes(LogicalName='{logical_name}')",
-        )
-
-    def add_alternate_key(
-        self,
-        schema_name: str,
-        display_name: str | Label,
-        key_attributes: Collection[str],
-        return_representation: bool = False,
-    ) -> requests.Response:
-        """
-        Add an alternate key to Entity.
-
-        Parameters
-        ----------
-        alternate_key : MetadataDumper
-            Dumpable metadata for new Alternate Key.
-        """
-        headers: dict[str, str] = dict()
-        if return_representation:
-            headers["Prefer"] = "return_representation"
-
-        key = get_altkey_metadata(
-            schema_name=schema_name,
-            display_name=display_name,
-            key_attributes=key_attributes,
-        )
-
-        resp = self._api_call(
-            method=RequestMethod.POST,
-            url=f"EntityMetadata(LogicalName='{self.logical_name}')/Keys",
-            headers=headers,
-            json=key.dump_to_dataverse(),
-        )
-
-        self.update_schema("altkeys")
-
-        return resp
-
-    @overload
-    def remove_alternate_key(self, *, altkey_id: str) -> requests.Response:
-        ...
-
-    @overload
-    def remove_alternate_key(self, *, logical_name: str) -> requests.Response:
-        ...
-
-    def remove_alternate_key(
-        self,
-        *,
-        altkey_id: str | None = None,
-        logical_name: str | None = None,
-    ) -> requests.Response:
-        """
-        Remove Alternate Key from Entity.
-
-        Parameters
-        ----------
-        attribute_id : str
-            GUID of Alternate Key.
-        logical_name : str
-            LogicalName of Alternate Key.
-
-        Returns
-        -------
-        requests.Response
-            The response from the server.
-        """
-        if altkey_id is None and logical_name is None:
-            raise DataverseError("Supply either 'id' or 'logical_name' kwarg.")
-
-        if altkey_id:
-            resp = self._api_call(
-                method=RequestMethod.DELETE,
-                url=f"EntityDefinitions(LogicalName='{self.logical_name}')/Attributes({altkey_id})",
-            )
-
-        resp = self._api_call(
-            method=RequestMethod.DELETE,
-            url=f"EntityDefinitions(LogicalName='{self.logical_name}')/Attributes(LogicalName='{logical_name}')",
-        )
-
-        self.update_schema("altkeys")
-
-        return resp
+import logging
+from collections.abc import Collection, Iterable, Mapping, MutableMapping, Sequence
+from copy import copy
+from typing import Any, Literal, overload
+
+import pandas as pd
+import requests
+
+from dataverse_api._api import Dataverse
+from dataverse_api.errors import DataverseError, DataverseModeError
+from dataverse_api.metadata.base import BASE_TYPE, MetadataDumper
+from dataverse_api.metadata.complex_properties import Label
+from dataverse_api.metadata.entity import get_altkey_metadata
+from dataverse_api.schema import DataverseRelationships
+from dataverse_api.utils.batching import (
+    APICommand,
+    RequestMethod,
+    chunk_data,
+    transform_to_batch_for_create,
+    transform_to_batch_for_delete,
+    transform_to_batch_for_upsert,
+    transform_upsert_data,
+)
+from dataverse_api.utils.data import (
+    convert_dataframe_to_dict,
+    extract_collection_valued_relationships,
+    extract_single_valued_relationships,
+)
+
+
+class DataverseEntity(Dataverse):
+    def __init__(
+        self,
+        session: requests.Session,
+        environment_url: str,
+        logical_name: str,
+    ):
+        super().__init__(session=session, environment_url=environment_url)
+
+        self.__logical_name = logical_name
+        self.__supports_create_multiple = False
+        self.__supports_update_multiple = False
+
+        # Populate entity properties
+        self.update_schema("all")
+
+    @property
+    def logical_name(self) -> str:
+        return self.__logical_name
+
+    @property
+    def entity_set_name(self) -> str:
+        return self.__entity_set_name
+
+    @property
+    def primary_id_attr(self) -> str:
+        return self.__primary_id_attr
+
+    @property
+    def primary_img_attr(self) -> str | None:
+        return self.__primary_img_attr
+
+    @property
+    def alternate_keys(self) -> dict[str, list[str]]:
+        return self.__alternate_keys
+
+    @property
+    def supports_create_multiple(self) -> bool:
+        return self.__supports_create_multiple
+
+    @property
+    def supports_update_multiple(self) -> bool:
+        return self.__supports_update_multiple
+
+    @property
+    def relationships(self) -> DataverseRelationships:
+        return self.__relationships
+
+    def __get_entity_set_properties(self) -> None:
+        """
+        Fetch key attributes of the Entity.
+
+          - `EntitySetName`, used as the API endpoint
+          - `PrimaryIdAttribute`, the primary ID column
+          - `PrimaryImageAttribute`, the primary image column (if any)
+
+        Returns
+        -------
+        EntityData
+            A dataclass with the three relevant attributes.
+        """
+        columns = ["EntitySetName", "PrimaryIdAttribute", "PrimaryImageAttribute"]
+        logging.debug("Retrieving EntityDefinitions for %s", self.logical_name)
+        resp = self._api_call(
+            method=RequestMethod.GET,
+            url=f"EntityDefinitions(LogicalName='{self.logical_name}')",
+            params={"$select": ",".join(columns)},
+        ).json()
+
+        self.__entity_set_name = resp["EntitySetName"]
+        self.__primary_id_attr = resp["PrimaryIdAttribute"]
+        self.__primary_img_attr = resp.get("PrimaryImageAttribute")
+
+    def __get_entity_alternate_keys(self) -> None:
+        """
+        Fetch the alternate keys (if any) for the Entity.
+        """
+        columns = ["SchemaName", "KeyAttributes"]
+        logging.debug("Retrieving alternate keys for %s", self.logical_name)
+        resp = self._api_call(
+            method=RequestMethod.GET,
+            url=f"EntityDefinitions(LogicalName='{self.logical_name}')/Keys",
+            params={"$select": ",".join(columns)},
+        ).json()["value"]
+
+        self.__alternate_keys = {r["SchemaName"]: r["KeyAttributes"] for r in resp}
+
+    def __get_entity_sdk_messages(self) -> None:
+        """
+        Fetch sdk messages to determine whether Entity supports certain actions.
+        """
+        create, update = "CreateMultiple", "UpdateMultiple"
+        actions = [create, update]
+        col = "primaryobjecttypecode"
+        msg_col = "sdkmessageid/name"
+
+        params: dict[str, str] = dict()
+        params["$select"] = "sdkmessagefilterid"
+        params["$expand"] = "sdkmessageid($select=name)"
+        params[
+            "$filter"
+        ] = f"""({' or '.join(f"{msg_col} eq '{x}'" for x in actions)}) and {col} eq '{self.logical_name}'"""
+
+        logging.debug("Retrieving SDK messages for %s", self.logical_name)
+        resp = self._api_call(
+            method=RequestMethod.GET,
+            url="sdkmessagefilters",
+            params=params,
+        ).json()["value"]
+        returned_actions = {row["sdkmessageid"]["name"] for row in resp}
+
+        if create in returned_actions:
+            self.__supports_create_multiple = True
+        if update in returned_actions:
+            self.__supports_update_multiple = True
+
+    def __get_entity_relationships(self) -> None:
+        """
+        Fetch the relationships for the Entity.
+
+        Collection-valued: 1:N relationships where this Entity is on the one-side.
+        Single-valued: N:1 relationships where this Entity is on the many-side.
+        """
+        one_to_many = self._api_call(
+            method=RequestMethod.GET,
+            url=f"EntityDefinitions(LogicalName='{self.logical_name}')/OneToManyRelationships",
+        ).json()["value"]
+        many_to_one = self._api_call(
+            method=RequestMethod.GET,
+            url=f"EntityDefinitions(LogicalName='{self.logical_name}')/ManyToOneRelationships",
+        ).json()["value"]
+
+        collection_valued = extract_collection_valued_relationships(
+            data=one_to_many, entity_logical_name=self.logical_name
+        )
+        single_valued = extract_single_valued_relationships(data=many_to_one)
+
+        self.__relationships = DataverseRelationships(single_valued=single_valued, collection_valued=collection_valued)
+
+    def update_schema(
+        self, arg: Literal["all", "altkeys", "properties", "messages", "relationships"] | None = None
+    ) -> None:
+        """
+        Update schema.
+        """
+        if arg == "altkeys":
+            self.__get_entity_alternate_keys()
+            return
+
+        if arg == "properties":
+            self.__get_entity_set_properties()
+            return
+
+        if arg == "messages":
+            self.__get_entity_sdk_messages()
+            return
+
+        if arg == "relationships":
+            self.__get_entity_relationships()
+            return
+
+        if arg == "all":
+            self.__get_entity_alternate_keys()
+            self.__get_entity_sdk_messages()
+            self.__get_entity_set_properties()
+            self.__get_entity_relationships()
+
+    @overload
+    def read(
+        self,
+        *,
+        select: Collection[str] | None = None,
+        top: int | None = None,
+        filter: str | None = None,
+        page_size: int | None = None,
+        expand: str | None = None,
+        order_by: str | None = None,
+    ) -> list[dict[str, Any]]:
+        ...
+
+    @overload
+    def read(
+        self,
+        *,
+        select: Collection[str] | None = None,
+        top: int | None = None,
+        filter: str | None = None,
+        page_size: int | None = None,
+        expand: str | None = None,
+        order_by: str | None = None,
+        return_responses: Literal[True],
+    ) -> list[requests.Response]:
+        ...
+
+    def read(
+        self,
+        *,
+        select: Collection[str] | None = None,
+        top: int | None = None,
+        filter: str | None = None,
+        page_size: int | None = None,
+        expand: str | None = None,
+        order_by: str | None = None,
+        return_responses: bool = False,
+    ) -> list[dict[str, Any]] | list[requests.Response]:
+        """
+        Read data from Entity.
+
+        Parameters
+        ----------
+        select : Collection[str]
+            Columns to return in the query.
+        top : int
+            Optional limit on returned records.
+        filter : str
+            A fully qualified filtering string.
+        expand : str
+            A fully qualified expand string.
+        orderby : str
+            A fully qualified order_by string.
+        apply : str
+            A fully qualified string describing aggregation and grouping of returned records.
+        page_size : int
+            Limits the total number of records retrieved per API call.
+        return_responses : bool
+            Returns complete responses instead of data records.
+
+        Returns
+        -------
+        list[dict[str, Any]]
+            The extended "value" element for all response-JSONs from server.
+        """
+
+        additional_headers: dict[str, str] = dict()
+        if page_size is not None:
+            additional_headers["Prefer"] = f"odata.maxpagesize={page_size}"
+
+        params: dict[str, Any] = dict()
+        if select:
+            params["$select"] = ",".join(select)
+        if filter:
+            params["$filter"] = filter
+        if top:
+            params["$top"] = top
+        if order_by:
+            params["$orderby"] = order_by
+        if expand:
+            params["$expand"] = expand
+
+        output: list[requests.Response] = list()
+        url = self.entity_set_name
+
+        # Looping through pages
+        logging.debug("Fetching data for read operation on %s.", self.logical_name)
+        response = self._api_call(
+            method=RequestMethod.GET,
+            url=url,
+            headers=additional_headers,
+            params=params,
+        )
+        output.append(response)
+        while response.json().get("@odata.nextLink"):
+            response = self._api_call(method=RequestMethod.GET, url=response.json()["@odata.nextLink"])
+            output.append(response)
+
+        if return_responses:
+            logging.debug("Fetched all data for read operation, %d responses.", len(output))
+            return output
+        else:
+            data_output: list[dict[str, Any]] = []
+            for resp in output:
+                data_output.extend(resp.json()["value"])
+            logging.debug("Fetched all data for read operation, %d elements.", len(data_output))
+            return data_output
+
+    @overload
+    def create(
+        self,
+        data: Sequence[MutableMapping[str, Any]] | pd.DataFrame,
+        *,
+        mode: Literal["individual", "multiple"] = "individual",
+        detect_duplicates: bool = False,
+        return_created: bool = False,
+        threading: bool = False,
+    ) -> list[requests.Response]:
+        ...
+
+    @overload
+    def create(
+        self,
+        data: Sequence[MutableMapping[str, Any]] | pd.DataFrame,
+        *,
+        mode: Literal["batch"],
+        detect_duplicates: bool = False,
+        return_created: bool = False,
+        batch_size: int | None = None,
+        threading: bool = False,
+    ) -> list[requests.Response]:
+        ...
+
+    def create(
+        self,
+        data: Sequence[MutableMapping[str, Any]] | pd.DataFrame,
+        *,
+        mode: Literal["individual", "multiple", "batch"] = "individual",
+        detect_duplicates: bool = False,
+        return_created: bool = False,
+        batch_size: int | None = None,
+        threading: bool = False,
+    ) -> list[requests.Response]:
+        """
+        Create rows in Dataverse Entity. Failures will occur if trying to insert
+        a record where alternate key already exists, partial success is possible.
+
+        data : Sequence[MutableMapping[str, Any] | pd.DataFrame
+            The data to create in Dataverse, JSON serializable.
+        mode : Literal["individual", "multiple", "batch"]
+            Whether to create rows using individual requests, `CreateMultiple` web API action
+            or as batch requests using the `$batch` endpoint.
+        detect_duplicates : bool
+            Whether Dataverse will run duplicate detection rules upon insertion.
+        return_created : bool
+            Whether the returned list of Responses will contain information on
+            created rows.
+        batch_size : int
+            Optional override if batch mode is specified, useful for tuning workload
+            per batch if 429s occur.
+        """
+        if isinstance(data, pd.DataFrame):
+            data = convert_dataframe_to_dict(data)
+
+        headers: dict[str, str] = dict()
+        if detect_duplicates:
+            headers["MSCRM.SuppressDuplicateDetection"] = "false"
+
+        if return_created:
+            headers["Prefer"] = "return=representation"
+
+        length = len(data)
+        if mode == "individual":
+            logging.debug("%d rows to insert using individual inserts.", length)
+            return self.__create_singles(headers=headers, data=data, threading=threading)
+
+        if mode == "multiple":
+            if not self.supports_create_multiple:
+                raise DataverseError(f"CreateMultiple is not supported by {self.logical_name}. Use a different mode.")
+            logging.debug("%d rows to insert using CreateMultiple.", length)
+            return self.__create_multiple(headers=headers, data=data, threading=threading)
+
+        if mode == "batch":
+            logging.debug(
+                "%d rows to insert using batch insertion.",
+                length,
+            )
+            return self.__create_batch(data=data, batch_size=batch_size, threading=threading)
+
+        raise DataverseModeError(mode, "individual", "multiple", "batch")
+
+    def __create_singles(
+        self,
+        data: Collection[MutableMapping[str, Any]],
+        headers: Mapping[str, str],
+        threading: bool,
+    ) -> list[requests.Response]:
+        """
+        Insert rows one by one using threaded API call.
+        """
+        calls = [
+            APICommand(
+                method=RequestMethod.POST,
+                url=self.entity_set_name,
+                headers=headers,
+                json=row,
+            )
+            for row in data
+        ]
+
+        if threading:
+            return self._threaded_call(calls=calls)
+        return self._individual_call(calls=calls)
+
+    def __create_multiple(
+        self, headers: Mapping[str, str], data: Sequence[MutableMapping[str, Any]], threading: bool
+    ) -> list[requests.Response]:
+        """
+        Insert rows by using the `CreateMultiple` Web API Action.
+        """
+        # Preserving input data
+        data = copy(data)
+
+        # Adding odata type to each record
+        for row in data:
+            row["@odata.type"] = BASE_TYPE + self.logical_name
+
+        # Chunking the payload to suggested size
+        calls = [
+            APICommand(
+                method=RequestMethod.POST,
+                url=f"{self.entity_set_name}/{BASE_TYPE}CreateMultiple",
+                headers=headers,
+                json={"Targets": rows},
+            )
+            for rows in chunk_data(data=data, size=500)
+        ]
+
+        if threading:
+            return self._threaded_call(calls)
+        return self._individual_call(calls)
+
+    def __create_batch(
+        self, data: Collection[MutableMapping[str, Any]], batch_size: int | None, threading: bool
+    ) -> list[requests.Response]:
+        """
+        Run a batch insert operation on the given data.
+        """
+        batch_data = transform_to_batch_for_create(url=self.entity_set_name, data=data)
+        return self._batch_api_call(batch_data, batch_size=batch_size, threading=threading)
+
+    def __delete_singles(self, data: Iterable[str], threading: bool) -> list[requests.Response]:
+        calls = [
+            APICommand(
+                method=RequestMethod.DELETE,
+                url=f"{self.entity_set_name}({id})",
+            )
+            for id in data
+        ]
+
+        if threading:
+            return self._threaded_call(calls=calls)
+        return self._individual_call(calls=calls)
+
+    @overload
+    def delete(
+        self,
+        *,
+        mode: Literal["individual"] = "individual",
+        ids: Collection[str],
+    ) -> list[requests.Response]:
+        ...
+
+    @overload
+    def delete(
+        self,
+        *,
+        mode: Literal["individual"] = "individual",
+        filter: str,
+        threading: bool = False,
+    ) -> list[requests.Response]:
+        ...
+
+    @overload
+    def delete(
+        self, *, mode: Literal["batch"], filter: str, batch_size: int | None = None, threading: bool = False
+    ) -> list[requests.Response]:
+        ...
+
+    @overload
+    def delete(
+        self, *, mode: Literal["batch"], ids: Collection[str], batch_size: int | None = None, threading: bool = False
+    ) -> list[requests.Response]:
+        ...
+
+    def delete(
+        self,
+        *,
+        mode: Literal["individual", "batch"] = "individual",
+        ids: Collection[str] | None = None,
+        filter: str | None = None,
+        batch_size: int | None = None,
+        threading: bool = False,
+    ) -> list[requests.Response]:
+        """
+        Delete rows in Entity.
+
+        Specify either a list of ID's for deletion or a filter
+        string for determining which records to delete.
+
+        Parameters
+        ----------
+        mode : Literal["individual","batch"]
+            Whether to delete rows using individual requests or batch requests.
+        ids : Collection[str]
+            List of primary IDs to delete. Takes precedence if passed.
+        filter : str
+            Filter statement for targeting specific records in Entity
+            for deletion. Use `filter="all"` to delete all records.
+        batch_size : int
+            Optional override if batch mode is specified, useful for tuning workload
+            per batch if 429s occur.
+        """
+        if ids is None and filter is None:
+            raise DataverseError("Function requires either ids to delete or a string passed as filter.")
+
+        if filter == "all":
+            filter = None
+
+        if ids is None:
+            records = self.read(select=[self.primary_id_attr], filter=filter)
+            ids = {row[self.primary_id_attr] for row in records}
+
+        length = len(ids)
+        logging.info("%d rows to delete.", length)
+        if mode == "individual":
+            logging.debug("%d rows to delete using individual deletes.", length)
+            return self.__delete_singles(data=ids, threading=threading)
+
+        if mode == "batch":
+            logging.debug("%d rows to delete using batch deletes.", length)
+            batch_data = transform_to_batch_for_delete(url=self.entity_set_name, data=ids)
+            return self._batch_api_call(batch_data, batch_size=batch_size or 100, timeout=120, threading=threading)
+
+        raise DataverseModeError(mode, "individual", "batch")
+
+    def __delete_column_singles(self, data: Iterable[str], column: str, threading: bool) -> list[requests.Response]:
+        """
+        Delete row column value by individual requests.
+        """
+        calls = [
+            APICommand(
+                method=RequestMethod.DELETE,
+                url=f"{self.entity_set_name}({id})/{column}",
+            )
+            for id in data
+        ]
+        if threading:
+            return self._threaded_call(calls=calls)
+        return self._individual_call(calls=calls)
+
+    @overload
+    def delete_columns(
+        self,
+        columns: Collection[str],
+        *,
+        mode: Literal["individual", "batch"] = "individual",
+        ids: Collection[str],
+        threading: bool,
+    ) -> list[requests.Response]:
+        ...
+
+    @overload
+    def delete_columns(
+        self,
+        columns: Collection[str],
+        *,
+        mode: Literal["individual", "batch"] = "individual",
+        filter: str,
+        threading: bool,
+    ) -> list[requests.Response]:
+        ...
+
+    def delete_columns(
+        self,
+        columns: Collection[str],
+        *,
+        ids: Collection[str] | None = None,
+        filter: str | None = None,
+        mode: Literal["individual", "batch"] = "individual",
+        threading: bool = False,
+    ) -> list[requests.Response]:
+        """
+        Delete values in specific column for rows in Entity.
+
+        Specify either a list of ID's for deletion or a filter
+        string for determining which records to delete.
+
+        Parameters
+        ----------
+        column : Collection[str]
+            The columns in Dataverse to target for deletion.
+        mode : Literal["individual", "batch"]
+            Whether to delete columns using individual requests or batch requests.
+        ids : Collection[str]
+            List of primary IDs to delete. Takes precedence if passed.
+        filter : str
+            Filter statement for targeting specific records in Entity for deletion.
+            Use `filter="all"` to delete all records.
+        """
+        if ids is None and filter is None:
+            raise DataverseError("Function requires either ids to delete or a string passed as filter.")
+
+        if filter == "all":
+            filter = None
+
+        if ids is None:
+            records = self.read(select=[self.primary_id_attr], filter=filter)
+            ids = {row[self.primary_id_attr] for row in records}
+
+        length = len(ids) * len(columns)  # Total number of deletion requests
+        output: list[requests.Response] = []
+        if mode == "individual":
+            logging.debug("%d properties to delete. Using individual deletes.", length)
+            for col in columns:
+                output.extend(self.__delete_column_singles(data=ids, column=col, threading=threading))
+            return output
+
+        if mode == "batch":
+            logging.debug("%d properties to delete. Using batch deletes.", length)
+            for col in columns:
+                batch_data = transform_to_batch_for_delete(url=self.entity_set_name, data=ids, column=col)
+                output.extend(self._batch_api_call(batch_data, threading=threading))
+            return output
+
+        raise DataverseModeError(mode, "individual", "batch")
+
+    def __upsert_singles(
+        self, data: Collection[Mapping[str, Any]], keys: Iterable[str], is_primary_id: bool, threading: bool
+    ) -> list[requests.Response]:
+        """
+        Upsert row by individual requests.
+        """
+        calls = [
+            APICommand(
+                method=RequestMethod.PATCH,
+                url=f"{self.entity_set_name}({key})",
+                json=payload,
+            )
+            for key, payload in transform_upsert_data(data, keys, is_primary_id)
+        ]
+        if threading:
+            return self._threaded_call(calls=calls)
+        return self._individual_call(calls=calls)
+
+    def upsert(
+        self,
+        data: Collection[MutableMapping[str, Any]] | pd.DataFrame,
+        *,
+        mode: Literal["individual", "batch"] = "individual",
+        altkey_name: str | None = None,
+        threading: bool = False,
+    ) -> list[requests.Response]:
+        """
+        Upsert data into Entity.
+
+        Parameters
+        ----------
+        data : Collection[MutableMapping[str, Any]] | pd.DataFrame
+            The data to upsert.
+        mode : Literal["individual", "batch"]
+            Whether to upsert data using individual requests or batch requests.
+        altkey_name : str
+            The alternate key to use as ID (if any).
+            Will assume entity primary ID attribute if not given.
+        """
+
+        if altkey_name is not None:
+            try:
+                key_columns = self.alternate_keys[altkey_name]
+            except KeyError:
+                raise DataverseError(f"Altkey '{altkey_name}' is not valid for Entity '{self.logical_name}'.")
+            is_primary_id = False
+        else:
+            key_columns = [self.primary_id_attr]
+            is_primary_id = True
+
+        if isinstance(data, pd.DataFrame):
+            data = convert_dataframe_to_dict(data)
+
+        if mode == "individual":
+            logging.debug("%d rows to upsert. Using individual upserts.", len(data))
+            return self.__upsert_singles(data=data, keys=key_columns, is_primary_id=is_primary_id, threading=threading)
+
+        if mode == "batch":
+            logging.debug("%d rows to upsert. Using batch upserts.", len(data))
+            batch_data = transform_to_batch_for_upsert(
+                url=self.entity_set_name,
+                data=data,
+                keys=key_columns,
+                is_primary_id=is_primary_id,
+            )
+            return self._batch_api_call(batch_data, threading=threading)
+
+        raise DataverseModeError(mode, "individual", "batch")
+
+    def add_attribute(
+        self,
+        attribute: MetadataDumper,
+        solution_name: str | None = None,
+        return_representation: bool = False,
+    ) -> requests.Response:
+        """
+        Add attribute to Entity.
+
+        Parameters
+        ----------
+        attribute : MetadataDumper
+            Dumpable metadata for new Attribute.
+        solution_name : str
+            Unique name for solution attribute is part of.
+        return_representation : bool
+            Whether to include the metadata representation after
+            creation in the response from server.
+
+        Returns
+        -------
+        requests.Response
+            The response from the server.
+        """
+
+        headers: dict[str, str] = dict()
+
+        if solution_name is not None:
+            headers["MSCRM.SolutionUniqueName"] = solution_name
+
+        if return_representation:
+            headers["Prefer"] = "return=representation"
+
+        return self._api_call(
+            method=RequestMethod.POST,
+            url=f"EntityDefinitions(LogicalName='{self.logical_name}')/Attributes",
+            headers=headers,
+            json=attribute.dump_to_dataverse(),
+        )
+
+    @overload
+    def remove_attribute(self, *, attribute_id: str) -> requests.Response:
+        ...
+
+    @overload
+    def remove_attribute(self, *, logical_name: str) -> requests.Response:
+        ...
+
+    def remove_attribute(
+        self,
+        *,
+        attribute_id: str | None = None,
+        logical_name: str | None = None,
+    ) -> requests.Response:
+        """
+        Remove Attribute from Entity.
+
+        Parameters
+        ----------
+        attribute_id : str
+            GUID of Attribute.
+        logical_name : str
+            LogicalName of Attribute.
+
+        Returns
+        -------
+        requests.Response
+            The response from the server.
+        """
+        if attribute_id is None and logical_name is None:
+            raise DataverseError("Supply either 'id' or 'logical_name' kwarg.")
+
+        if attribute_id:
+            return self._api_call(
+                method=RequestMethod.DELETE,
+                url=f"EntityDefinitions(LogicalName='{self.logical_name}')/Attributes({attribute_id})",
+            )
+
+        return self._api_call(
+            method=RequestMethod.DELETE,
+            url=f"EntityDefinitions(LogicalName='{self.logical_name}')/Attributes(LogicalName='{logical_name}')",
+        )
+
+    def add_alternate_key(
+        self,
+        schema_name: str,
+        display_name: str | Label,
+        key_attributes: Collection[str],
+        return_representation: bool = False,
+    ) -> requests.Response:
+        """
+        Add an alternate key to Entity.
+
+        Parameters
+        ----------
+        alternate_key : MetadataDumper
+            Dumpable metadata for new Alternate Key.
+        """
+        headers: dict[str, str] = dict()
+        if return_representation:
+            headers["Prefer"] = "return_representation"
+
+        key = get_altkey_metadata(
+            schema_name=schema_name,
+            display_name=display_name,
+            key_attributes=key_attributes,
+        )
+
+        resp = self._api_call(
+            method=RequestMethod.POST,
+            url=f"EntityMetadata(LogicalName='{self.logical_name}')/Keys",
+            headers=headers,
+            json=key.dump_to_dataverse(),
+        )
+
+        self.update_schema("altkeys")
+
+        return resp
+
+    @overload
+    def remove_alternate_key(self, *, altkey_id: str) -> requests.Response:
+        ...
+
+    @overload
+    def remove_alternate_key(self, *, logical_name: str) -> requests.Response:
+        ...
+
+    def remove_alternate_key(
+        self,
+        *,
+        altkey_id: str | None = None,
+        logical_name: str | None = None,
+    ) -> requests.Response:
+        """
+        Remove Alternate Key from Entity.
+
+        Parameters
+        ----------
+        attribute_id : str
+            GUID of Alternate Key.
+        logical_name : str
+            LogicalName of Alternate Key.
+
+        Returns
+        -------
+        requests.Response
+            The response from the server.
+        """
+        if altkey_id is None and logical_name is None:
+            raise DataverseError("Supply either 'id' or 'logical_name' kwarg.")
+
+        if altkey_id:
+            resp = self._api_call(
+                method=RequestMethod.DELETE,
+                url=f"EntityDefinitions(LogicalName='{self.logical_name}')/Attributes({altkey_id})",
+            )
+
+        resp = self._api_call(
+            method=RequestMethod.DELETE,
+            url=f"EntityDefinitions(LogicalName='{self.logical_name}')/Attributes(LogicalName='{logical_name}')",
+        )
+
+        self.update_schema("altkeys")
+
+        return resp
```

### Comparing `dataverse_api-1.1.4/dataverse_api/metadata/attributes.py` & `dataverse_api-1.1.5/dataverse_api/metadata/attributes.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,249 +1,249 @@
-"""
-A collection of Dataverse Attribute metadata classes.
-"""
-
-
-from typing import Any
-
-from pydantic import Field
-
-from dataverse_api.metadata.base import BASE_TYPE, MetadataBase
-from dataverse_api.metadata.complex_properties import Label, RequiredLevel, create_label, required_level_default
-from dataverse_api.metadata.enums import (
-    AttributeType,
-    AttributeTypeName,
-    DateTimeFormat,
-    IntegerFormat,
-    MemoFormat,
-    StringFormat,
-)
-from dataverse_api.utils.labels import define_label
-
-
-class AttributeMetadata(MetadataBase):
-    """
-    Base Metadata class for Attributes.
-    """
-
-    schema_name: str
-    description: Label = Field(default_factory=create_label)
-    display_name: Label = Field(default_factory=create_label)
-    required_level: RequiredLevel = Field(default_factory=required_level_default)
-
-
-class LookupAttributeMetadata(AttributeMetadata):
-    """
-    Attribute Metadata for a Lookup column.
-
-    Parameters
-    ----------
-    schema_name : str
-    description : dataverse.Label
-    display_name : dataverse.Label
-    required_level : dataverse.RequiredLevel
-    """
-
-    def model_post_init(self, __context: Any) -> None:
-        self.attribute_type = AttributeType.LOOKUP
-        self.attribute_type_name = AttributeTypeName.LOOKUP
-        self.odata_type = BASE_TYPE + "LookupAttributeMetadata"
-        return super().model_post_init(__context)
-
-
-class StringAttributeMetadata(AttributeMetadata):
-    """
-    Attribute Metadata for a String column.
-
-    Parameters
-    ----------
-    schema_name : str
-    max_length : int
-    format_name : dataverse.StringFormat
-    description : dataverse.Label
-    display_name : dataverse.Label
-    required_level : dataverse.RequiredLevel
-    is_primary_name : bool
-    """
-
-    is_primary_name: bool = Field(default=False)
-    max_length: int = Field(default=100)
-    format_name: StringFormat = Field(default=StringFormat.TEXT)
-    auto_number_format: str | None = Field(default=None)
-
-    def model_post_init(self, __context: Any) -> None:
-        self.odata_type = BASE_TYPE + "StringAttributeMetadata"
-        self.attribute_type = AttributeType.STRING
-        self.attribute_type_name = AttributeTypeName.STRING_TYPE
-        if self.auto_number_format is not None:
-            self.format_name = StringFormat.TEXT
-        return super().model_post_init(__context)
-
-
-class DecimalAttributeMetadata(AttributeMetadata):
-    """
-    Attribute Metadata for a Decimal column.
-
-    Parameters
-    ----------
-    schema_name : str
-    min_value : float
-    max_value : float
-    precision : int
-    description : dataverse.Label
-    display_name : dataverse.Label
-    required_level : dataverse.RequiredLevel
-    """
-
-    min_value: float
-    max_value: float
-    precision: int = 2
-
-    def model_post_init(self, __context: Any) -> None:
-        self.odata_type = BASE_TYPE + "DecimalAttributeMetadata"
-        self.attribute_type = AttributeType.DECIMAL
-        self.attribute_type_name = AttributeTypeName.DECIMAL
-        return super().model_post_init(__context)
-
-
-class IntegerAttributeMetadata(AttributeMetadata):
-    """
-    Attribute Metadata for a Integer column.
-
-    Parameters
-    ----------
-    schema_name : str
-    min_value : int
-    max_value : int
-    precision : int
-    format : dataverse.IntegerFormat
-    description : dataverse.Label
-    display_name : dataverse.Label
-    required_level : dataverse.RequiredLevel
-    """
-
-    min_value: int
-    max_value: int
-    precision: int = 2
-    format: IntegerFormat = Field(default=IntegerFormat.NONE)
-
-    def model_post_init(self, __context: Any) -> None:
-        self.odata_type = BASE_TYPE + "IntegerAttributeMetadata"
-        self.attribute_type = AttributeType.INTEGER
-        self.attribute_type_name = AttributeTypeName.INTEGER
-        return super().model_post_init(__context)
-
-
-class DateTimeAttributeMetadata(AttributeMetadata):
-    """
-    Attribute Metadata for a DateTime column.
-
-    Parameters
-    ----------
-    schema_name : str
-    min_value : int
-    max_value : int
-    precision : int
-    description : dataverse.Label
-    display_name : dataverse.Label
-    required_level : dataverse.RequiredLevel
-    """
-
-    format: DateTimeFormat = Field(default=DateTimeFormat.DATE_AND_TIME)
-
-    def model_post_init(self, __context: Any) -> None:
-        self.odata_type = BASE_TYPE + "DateTimeAttributeMetadata"
-        self.attribute_type = AttributeType.DATE_TIME
-        self.attribute_type_name = AttributeTypeName.DATE_TIME
-        return super().model_post_init(__context)
-
-
-class MemoAttributeMetadata(AttributeMetadata):
-    """
-    Attribute Metadata for a Memo column.
-
-    Parameters
-    ----------
-    schema_name : str
-    description : dataverse.Label
-    display_name : dataverse.Label
-    required_level : dataverse.RequiredLevel
-    """
-
-    format: MemoFormat = Field(default=MemoFormat.TEXT_AREA)
-
-    def model_post_init(self, __context: Any) -> None:
-        self.odata_type = BASE_TYPE + "MemoAttributeMetadata"
-        self.attribute_type = AttributeType.MEMO
-        self.attribute_type_name = AttributeTypeName.MEMO
-        return super().model_post_init(__context)
-
-
-class BigIntAttributeMetadata(AttributeMetadata):
-    """
-    Attribute Metadata for a Memo column.
-
-    Parameters
-    ----------
-    schema_name : str
-    description : dataverse.Label
-    display_name : dataverse.Label
-    required_level : dataverse.RequiredLevel
-    """
-
-    def model_post_init(self, __context: Any) -> None:
-        self.odata_type = BASE_TYPE + "BigIntAttributeMetadata"
-        self.attribute_type = AttributeType.BIG_INT
-        self.attribute_type_name = AttributeTypeName.BIG_INT
-        return super().model_post_init(__context)
-
-
-class BoolOption(MetadataBase):
-    value: int
-    label: Label
-
-
-def bool_opt(val: bool) -> BoolOption:
-    return BoolOption(value=val, label=define_label(str(val)))
-
-
-class BooleanOptionSet(MetadataBase):
-    true_option: BoolOption = Field(default=bool_opt(True))
-    false_option: BoolOption = Field(default=bool_opt(False))
-
-    def model_post_init(self, __context: Any) -> None:
-        self.option_set_type = "Boolean"
-        return super().model_post_init(__context)
-
-
-class BooleanAttributeMetadata(AttributeMetadata):
-    """
-    Attribute Metadata for a Boolean column.
-
-    Parameters
-    ----------
-    schema_name : str
-    option_set : BooleanOptionSet
-    description : dataverse.Label
-    display_name : dataverse.Label
-    required_level : dataverse.RequiredLevel
-    """
-
-    default_value: bool = False
-    option_set: BooleanOptionSet = Field(default=BooleanOptionSet())
-
-    def model_post_init(self, __context: Any) -> None:
-        self.odata_type = BASE_TYPE + "BooleanAttributeMetadata"
-        self.attribute_type = AttributeType.BOOLEAN
-        self.attribute_type_name = AttributeTypeName.BOOLEAN
-        return super().model_post_init(__context)
-
-
-AttributeTypes = (
-    StringAttributeMetadata
-    | DecimalAttributeMetadata
-    | DateTimeAttributeMetadata
-    | IntegerAttributeMetadata
-    | BigIntAttributeMetadata
-    | BooleanAttributeMetadata
-    | MemoAttributeMetadata
-)
+"""
+A collection of Dataverse Attribute metadata classes.
+"""
+
+
+from typing import Any
+
+from pydantic import Field
+
+from dataverse_api.metadata.base import BASE_TYPE, MetadataBase
+from dataverse_api.metadata.complex_properties import Label, RequiredLevel, create_label, required_level_default
+from dataverse_api.metadata.enums import (
+    AttributeType,
+    AttributeTypeName,
+    DateTimeFormat,
+    IntegerFormat,
+    MemoFormat,
+    StringFormat,
+)
+from dataverse_api.utils.labels import define_label
+
+
+class AttributeMetadata(MetadataBase):
+    """
+    Base Metadata class for Attributes.
+    """
+
+    schema_name: str
+    description: Label = Field(default_factory=create_label)
+    display_name: Label = Field(default_factory=create_label)
+    required_level: RequiredLevel = Field(default_factory=required_level_default)
+
+
+class LookupAttributeMetadata(AttributeMetadata):
+    """
+    Attribute Metadata for a Lookup column.
+
+    Parameters
+    ----------
+    schema_name : str
+    description : dataverse.Label
+    display_name : dataverse.Label
+    required_level : dataverse.RequiredLevel
+    """
+
+    def model_post_init(self, __context: Any) -> None:
+        self.attribute_type = AttributeType.LOOKUP
+        self.attribute_type_name = AttributeTypeName.LOOKUP
+        self.odata_type = BASE_TYPE + "LookupAttributeMetadata"
+        return super().model_post_init(__context)
+
+
+class StringAttributeMetadata(AttributeMetadata):
+    """
+    Attribute Metadata for a String column.
+
+    Parameters
+    ----------
+    schema_name : str
+    max_length : int
+    format_name : dataverse.StringFormat
+    description : dataverse.Label
+    display_name : dataverse.Label
+    required_level : dataverse.RequiredLevel
+    is_primary_name : bool
+    """
+
+    is_primary_name: bool = Field(default=False)
+    max_length: int = Field(default=100)
+    format_name: StringFormat = Field(default=StringFormat.TEXT)
+    auto_number_format: str | None = Field(default=None)
+
+    def model_post_init(self, __context: Any) -> None:
+        self.odata_type = BASE_TYPE + "StringAttributeMetadata"
+        self.attribute_type = AttributeType.STRING
+        self.attribute_type_name = AttributeTypeName.STRING_TYPE
+        if self.auto_number_format is not None:
+            self.format_name = StringFormat.TEXT
+        return super().model_post_init(__context)
+
+
+class DecimalAttributeMetadata(AttributeMetadata):
+    """
+    Attribute Metadata for a Decimal column.
+
+    Parameters
+    ----------
+    schema_name : str
+    min_value : float
+    max_value : float
+    precision : int
+    description : dataverse.Label
+    display_name : dataverse.Label
+    required_level : dataverse.RequiredLevel
+    """
+
+    min_value: float
+    max_value: float
+    precision: int = 2
+
+    def model_post_init(self, __context: Any) -> None:
+        self.odata_type = BASE_TYPE + "DecimalAttributeMetadata"
+        self.attribute_type = AttributeType.DECIMAL
+        self.attribute_type_name = AttributeTypeName.DECIMAL
+        return super().model_post_init(__context)
+
+
+class IntegerAttributeMetadata(AttributeMetadata):
+    """
+    Attribute Metadata for a Integer column.
+
+    Parameters
+    ----------
+    schema_name : str
+    min_value : int
+    max_value : int
+    precision : int
+    format : dataverse.IntegerFormat
+    description : dataverse.Label
+    display_name : dataverse.Label
+    required_level : dataverse.RequiredLevel
+    """
+
+    min_value: int
+    max_value: int
+    precision: int = 2
+    format: IntegerFormat = Field(default=IntegerFormat.NONE)
+
+    def model_post_init(self, __context: Any) -> None:
+        self.odata_type = BASE_TYPE + "IntegerAttributeMetadata"
+        self.attribute_type = AttributeType.INTEGER
+        self.attribute_type_name = AttributeTypeName.INTEGER
+        return super().model_post_init(__context)
+
+
+class DateTimeAttributeMetadata(AttributeMetadata):
+    """
+    Attribute Metadata for a DateTime column.
+
+    Parameters
+    ----------
+    schema_name : str
+    min_value : int
+    max_value : int
+    precision : int
+    description : dataverse.Label
+    display_name : dataverse.Label
+    required_level : dataverse.RequiredLevel
+    """
+
+    format: DateTimeFormat = Field(default=DateTimeFormat.DATE_AND_TIME)
+
+    def model_post_init(self, __context: Any) -> None:
+        self.odata_type = BASE_TYPE + "DateTimeAttributeMetadata"
+        self.attribute_type = AttributeType.DATE_TIME
+        self.attribute_type_name = AttributeTypeName.DATE_TIME
+        return super().model_post_init(__context)
+
+
+class MemoAttributeMetadata(AttributeMetadata):
+    """
+    Attribute Metadata for a Memo column.
+
+    Parameters
+    ----------
+    schema_name : str
+    description : dataverse.Label
+    display_name : dataverse.Label
+    required_level : dataverse.RequiredLevel
+    """
+
+    format: MemoFormat = Field(default=MemoFormat.TEXT_AREA)
+
+    def model_post_init(self, __context: Any) -> None:
+        self.odata_type = BASE_TYPE + "MemoAttributeMetadata"
+        self.attribute_type = AttributeType.MEMO
+        self.attribute_type_name = AttributeTypeName.MEMO
+        return super().model_post_init(__context)
+
+
+class BigIntAttributeMetadata(AttributeMetadata):
+    """
+    Attribute Metadata for a Memo column.
+
+    Parameters
+    ----------
+    schema_name : str
+    description : dataverse.Label
+    display_name : dataverse.Label
+    required_level : dataverse.RequiredLevel
+    """
+
+    def model_post_init(self, __context: Any) -> None:
+        self.odata_type = BASE_TYPE + "BigIntAttributeMetadata"
+        self.attribute_type = AttributeType.BIG_INT
+        self.attribute_type_name = AttributeTypeName.BIG_INT
+        return super().model_post_init(__context)
+
+
+class BoolOption(MetadataBase):
+    value: int
+    label: Label
+
+
+def bool_opt(val: bool) -> BoolOption:
+    return BoolOption(value=val, label=define_label(str(val)))
+
+
+class BooleanOptionSet(MetadataBase):
+    true_option: BoolOption = Field(default=bool_opt(True))
+    false_option: BoolOption = Field(default=bool_opt(False))
+
+    def model_post_init(self, __context: Any) -> None:
+        self.option_set_type = "Boolean"
+        return super().model_post_init(__context)
+
+
+class BooleanAttributeMetadata(AttributeMetadata):
+    """
+    Attribute Metadata for a Boolean column.
+
+    Parameters
+    ----------
+    schema_name : str
+    option_set : BooleanOptionSet
+    description : dataverse.Label
+    display_name : dataverse.Label
+    required_level : dataverse.RequiredLevel
+    """
+
+    default_value: bool = False
+    option_set: BooleanOptionSet = Field(default=BooleanOptionSet())
+
+    def model_post_init(self, __context: Any) -> None:
+        self.odata_type = BASE_TYPE + "BooleanAttributeMetadata"
+        self.attribute_type = AttributeType.BOOLEAN
+        self.attribute_type_name = AttributeTypeName.BOOLEAN
+        return super().model_post_init(__context)
+
+
+AttributeTypes = (
+    StringAttributeMetadata
+    | DecimalAttributeMetadata
+    | DateTimeAttributeMetadata
+    | IntegerAttributeMetadata
+    | BigIntAttributeMetadata
+    | BooleanAttributeMetadata
+    | MemoAttributeMetadata
+)
```

### Comparing `dataverse_api-1.1.4/dataverse_api/metadata/base.py` & `dataverse_api-1.1.5/dataverse_api/metadata/base.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,61 +1,61 @@
-"""
-The base Metadata class for Dataverse.
-"""
-from typing import Any, Protocol, Self
-
-from pydantic import BaseModel, ConfigDict
-
-from dataverse_api.utils.text import convert_dict_keys_to_snake, convert_dict_keys_to_title
-
-BASE_TYPE = "Microsoft.Dynamics.CRM."
-
-
-class MetadataDumper(Protocol):
-    @property
-    def schema_name(self) -> str:
-        ...
-
-    def dump_to_dataverse(self) -> dict[str, Any]:
-        ...
-
-
-class MetadataBase(BaseModel):
-    """
-    Defines the base of all Metadata dataclasses, and a few key
-    methods used to serialize an API response and prepare an API request.
-    """
-
-    model_config = ConfigDict(extra="allow", validate_assignment=True)
-
-    @classmethod
-    def model_validate_dataverse(cls, arg: dict[str, Any]) -> Self:
-        """
-        Converts and validates a received deserialized JSON payload
-        into the appropriate Metadata object.
-
-        Parameters
-        ----------
-        arg : dict
-            To be converted into a validated object.
-        """
-
-        converted = convert_dict_keys_to_snake(arg)
-        return cls.model_validate(converted)
-
-    def dump_to_dataverse(self, dropna: bool = True) -> dict[str, Any]:
-        """
-        When called, dumps the vars dictionary as TitleCase,
-        needed to pass payloads to  Dataverse Web API.
-
-        Returns
-        -------
-        dict
-            A dictionary using Dataverse-friendly Keys,
-            appropriately sorted.
-        """
-        if dropna:
-            dump = self.model_dump(mode="json", exclude_none=True)
-        else:
-            dump = self.model_dump(mode="json")
-
-        return convert_dict_keys_to_title(dump)
+"""
+The base Metadata class for Dataverse.
+"""
+from typing import Any, Protocol, Self
+
+from pydantic import BaseModel, ConfigDict
+
+from dataverse_api.utils.text import convert_dict_keys_to_snake, convert_dict_keys_to_title
+
+BASE_TYPE = "Microsoft.Dynamics.CRM."
+
+
+class MetadataDumper(Protocol):
+    @property
+    def schema_name(self) -> str:
+        ...
+
+    def dump_to_dataverse(self) -> dict[str, Any]:
+        ...
+
+
+class MetadataBase(BaseModel):
+    """
+    Defines the base of all Metadata dataclasses, and a few key
+    methods used to serialize an API response and prepare an API request.
+    """
+
+    model_config = ConfigDict(extra="allow", validate_assignment=True)
+
+    @classmethod
+    def model_validate_dataverse(cls, arg: dict[str, Any]) -> Self:
+        """
+        Converts and validates a received deserialized JSON payload
+        into the appropriate Metadata object.
+
+        Parameters
+        ----------
+        arg : dict
+            To be converted into a validated object.
+        """
+
+        converted = convert_dict_keys_to_snake(arg)
+        return cls.model_validate(converted)
+
+    def dump_to_dataverse(self, dropna: bool = True) -> dict[str, Any]:
+        """
+        When called, dumps the vars dictionary as TitleCase,
+        needed to pass payloads to  Dataverse Web API.
+
+        Returns
+        -------
+        dict
+            A dictionary using Dataverse-friendly Keys,
+            appropriately sorted.
+        """
+        if dropna:
+            dump = self.model_dump(mode="json", exclude_none=True)
+        else:
+            dump = self.model_dump(mode="json")
+
+        return convert_dict_keys_to_title(dump)
```

### Comparing `dataverse_api-1.1.4/dataverse_api/metadata/complex_properties.py` & `dataverse_api-1.1.5/dataverse_api/metadata/complex_properties.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,180 +1,180 @@
-"""
-A collection of Dataverse Complex Property metadata classes.
-"""
-
-from collections.abc import Sequence
-from typing import Any, overload
-
-from pydantic import Field
-
-from dataverse_api.metadata.base import BASE_TYPE, MetadataBase
-from dataverse_api.metadata.enums import (
-    AssociatedMenuBehavior,
-    AssociatedMenuGroup,
-    AttributeRequiredLevel,
-    CascadeType,
-)
-
-
-class RequiredLevel(MetadataBase):
-    """
-    Complex Property describing the Required Level of an Attribute.
-
-    Parameters
-    ----------
-    value : AttributeRequiredLevel
-        Enum designating the actual required level value for the Attribute.
-    can_be_changed: bool
-        Whether the setting can be changed.
-    """
-
-    value: AttributeRequiredLevel = AttributeRequiredLevel.NONE
-    can_be_changed: bool = True
-
-    def model_post_init(self, _: Any) -> None:
-        self.managed_property_logical_name: str = "canmodifyrequirementlevelsettings"
-
-
-def required_level_default() -> RequiredLevel:
-    return RequiredLevel()
-
-
-class LocalizedLabel(MetadataBase):
-    """
-    Complex property describing a Localized Label in Dataverse.
-    Localized labels are associated with a Microsoft Locale ID (LCID)
-
-    Parameters
-    ----------
-    label : str
-        The text to be shown.
-    language_code : int
-        The associated language code for the specific localized label.
-    """
-
-    label: str
-    language_code: int = 1033
-    is_managed: bool = False
-
-    def model_post_init(self, _: Any) -> None:
-        self.odata_type: str = BASE_TYPE + "LocalizedLabel"
-
-
-class Label(MetadataBase):
-    """
-    Complex property describing a Label in Dataverse.
-
-    Parameters
-    ----------
-    localized_labels : list of `LocalizedLabels`
-        The list of localized labels defined for the `Label`. Each
-        `LocalizedLabel` defines the label for an associated language code.
-    """
-
-    localized_labels: Sequence[LocalizedLabel] = Field(default_factory=list)
-
-    def model_post_init(self, _: Any) -> None:
-        self.odata_type: str = BASE_TYPE + "Label"
-
-
-@overload
-def create_label() -> Label:
-    ...
-
-
-@overload
-def create_label(*, label: str) -> Label:
-    ...
-
-
-@overload
-def create_label(*, label: str, language_code: int) -> Label:
-    ...
-
-
-@overload
-def create_label(*, labels: Sequence[tuple[str, int]]) -> Label:
-    ...
-
-
-def create_label(
-    *,
-    label: str | None = None,
-    language_code: int | None = None,
-    labels: Sequence[tuple[str, int]] | None = None,
-) -> Label:
-    """
-    Creates a new `Label` instance.
-
-    Parameters
-    ----------
-    label : string or tuple of string and integer
-        For creating one `LocalizedLabel` within the `Label`.
-    code : int
-        The language code for a given `label`.
-    labels: tuple of string and integer
-        For specifying multiple `LocalizedLabel`s within the `Label`.
-        Each tuple represents one label/language code pair.
-
-    Returns
-    -------
-    `Label`
-        A metadata object according to Dataverse specification.
-
-    Raises
-    ------
-    ValueError: If input types are incorrect.
-    AssertionError: If tuples are incorrectly typed.
-
-    Notes
-    -----
-    The language codes recognized by the Dataverse organization can be retrieved
-    using the `DataverseClient.get_language_codes` method. Language codes specified
-    outside of the values returned by this method will be silently ignored by the API.
-    """
-
-    if language_code is None:
-        language_code = 1033
-
-    if label:
-        localized_labels = [LocalizedLabel(label=label, language_code=language_code)]
-    elif labels:
-        localized_labels = [LocalizedLabel(label=label[0], language_code=label[1]) for label in labels]
-    else:
-        localized_labels = [LocalizedLabel(label="Label")]
-    return Label(localized_labels=localized_labels)
-
-
-class AssociatedMenuConfiguration(MetadataBase):
-    """
-    Complex Property for Associated Menu Config.
-
-    Parameters
-    ----------
-    behavior : AssociatedMenuBehavior
-        Describes the behavior of the associated menu for a one-to-many relationship.
-    group: AssociatedMenuGroup
-        Describes the group in which to display the associated menu for an entity relationship.
-    order : int
-        The order for the associated menu. Value must be higher than 10 000.
-    label : Label
-        The label for the associated menu.
-    """
-
-    behavior: AssociatedMenuBehavior = AssociatedMenuBehavior.USE_COLLECTION_NAME
-    group: AssociatedMenuGroup = AssociatedMenuGroup.DETAILS
-    order: int = 10000
-    label: Label = Field(default_factory=lambda: create_label(label=""))
-
-
-class CascadeConfiguration(MetadataBase):
-    """
-    Complex Property for Cascade Configuration.
-    """
-
-    assign: CascadeType = Field(default=CascadeType.CASCADE)
-    delete: CascadeType = Field(default=CascadeType.CASCADE)
-    merge: CascadeType = Field(default=CascadeType.CASCADE)
-    reparent: CascadeType = Field(default=CascadeType.CASCADE)
-    share: CascadeType = Field(default=CascadeType.CASCADE)
-    unshare: CascadeType = Field(default=CascadeType.CASCADE)
+"""
+A collection of Dataverse Complex Property metadata classes.
+"""
+
+from collections.abc import Sequence
+from typing import Any, overload
+
+from pydantic import Field
+
+from dataverse_api.metadata.base import BASE_TYPE, MetadataBase
+from dataverse_api.metadata.enums import (
+    AssociatedMenuBehavior,
+    AssociatedMenuGroup,
+    AttributeRequiredLevel,
+    CascadeType,
+)
+
+
+class RequiredLevel(MetadataBase):
+    """
+    Complex Property describing the Required Level of an Attribute.
+
+    Parameters
+    ----------
+    value : AttributeRequiredLevel
+        Enum designating the actual required level value for the Attribute.
+    can_be_changed: bool
+        Whether the setting can be changed.
+    """
+
+    value: AttributeRequiredLevel = AttributeRequiredLevel.NONE
+    can_be_changed: bool = True
+
+    def model_post_init(self, _: Any) -> None:
+        self.managed_property_logical_name: str = "canmodifyrequirementlevelsettings"
+
+
+def required_level_default() -> RequiredLevel:
+    return RequiredLevel()
+
+
+class LocalizedLabel(MetadataBase):
+    """
+    Complex property describing a Localized Label in Dataverse.
+    Localized labels are associated with a Microsoft Locale ID (LCID)
+
+    Parameters
+    ----------
+    label : str
+        The text to be shown.
+    language_code : int
+        The associated language code for the specific localized label.
+    """
+
+    label: str
+    language_code: int = 1033
+    is_managed: bool = False
+
+    def model_post_init(self, _: Any) -> None:
+        self.odata_type: str = BASE_TYPE + "LocalizedLabel"
+
+
+class Label(MetadataBase):
+    """
+    Complex property describing a Label in Dataverse.
+
+    Parameters
+    ----------
+    localized_labels : list of `LocalizedLabels`
+        The list of localized labels defined for the `Label`. Each
+        `LocalizedLabel` defines the label for an associated language code.
+    """
+
+    localized_labels: Sequence[LocalizedLabel] = Field(default_factory=list)
+
+    def model_post_init(self, _: Any) -> None:
+        self.odata_type: str = BASE_TYPE + "Label"
+
+
+@overload
+def create_label() -> Label:
+    ...
+
+
+@overload
+def create_label(*, label: str) -> Label:
+    ...
+
+
+@overload
+def create_label(*, label: str, language_code: int) -> Label:
+    ...
+
+
+@overload
+def create_label(*, labels: Sequence[tuple[str, int]]) -> Label:
+    ...
+
+
+def create_label(
+    *,
+    label: str | None = None,
+    language_code: int | None = None,
+    labels: Sequence[tuple[str, int]] | None = None,
+) -> Label:
+    """
+    Creates a new `Label` instance.
+
+    Parameters
+    ----------
+    label : string or tuple of string and integer
+        For creating one `LocalizedLabel` within the `Label`.
+    code : int
+        The language code for a given `label`.
+    labels: tuple of string and integer
+        For specifying multiple `LocalizedLabel`s within the `Label`.
+        Each tuple represents one label/language code pair.
+
+    Returns
+    -------
+    `Label`
+        A metadata object according to Dataverse specification.
+
+    Raises
+    ------
+    ValueError: If input types are incorrect.
+    AssertionError: If tuples are incorrectly typed.
+
+    Notes
+    -----
+    The language codes recognized by the Dataverse organization can be retrieved
+    using the `DataverseClient.get_language_codes` method. Language codes specified
+    outside of the values returned by this method will be silently ignored by the API.
+    """
+
+    if language_code is None:
+        language_code = 1033
+
+    if label:
+        localized_labels = [LocalizedLabel(label=label, language_code=language_code)]
+    elif labels:
+        localized_labels = [LocalizedLabel(label=label[0], language_code=label[1]) for label in labels]
+    else:
+        localized_labels = [LocalizedLabel(label="Label")]
+    return Label(localized_labels=localized_labels)
+
+
+class AssociatedMenuConfiguration(MetadataBase):
+    """
+    Complex Property for Associated Menu Config.
+
+    Parameters
+    ----------
+    behavior : AssociatedMenuBehavior
+        Describes the behavior of the associated menu for a one-to-many relationship.
+    group: AssociatedMenuGroup
+        Describes the group in which to display the associated menu for an entity relationship.
+    order : int
+        The order for the associated menu. Value must be higher than 10 000.
+    label : Label
+        The label for the associated menu.
+    """
+
+    behavior: AssociatedMenuBehavior = AssociatedMenuBehavior.USE_COLLECTION_NAME
+    group: AssociatedMenuGroup = AssociatedMenuGroup.DETAILS
+    order: int = 10000
+    label: Label = Field(default_factory=lambda: create_label(label=""))
+
+
+class CascadeConfiguration(MetadataBase):
+    """
+    Complex Property for Cascade Configuration.
+    """
+
+    assign: CascadeType = Field(default=CascadeType.CASCADE)
+    delete: CascadeType = Field(default=CascadeType.CASCADE)
+    merge: CascadeType = Field(default=CascadeType.CASCADE)
+    reparent: CascadeType = Field(default=CascadeType.CASCADE)
+    share: CascadeType = Field(default=CascadeType.CASCADE)
+    unshare: CascadeType = Field(default=CascadeType.CASCADE)
```

### Comparing `dataverse_api-1.1.4/dataverse_api/metadata/entity.py` & `dataverse_api-1.1.5/dataverse_api/metadata/entity.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,114 +1,114 @@
-"""
-The Dataverse Entity metadata class, and a function to define it using as little
-data as possible for ease of use.
-"""
-
-
-from collections.abc import Collection, Sequence
-from typing import Any
-
-from dataverse_api.metadata.attributes import AttributeTypes
-from dataverse_api.metadata.base import BASE_TYPE, MetadataBase
-from dataverse_api.metadata.complex_properties import Label
-from dataverse_api.metadata.enums import OwnershipType
-from dataverse_api.utils.labels import define_label
-
-
-class EntityMetadata(MetadataBase):
-    """
-    Entity Metadata for Dataverse.
-    """
-
-    schema_name: str
-    description: Label
-    display_name: Label
-    display_collection_name: Label
-    attributes: Sequence[AttributeTypes] | None = None
-    ownership_type: OwnershipType
-    is_activity: bool
-    has_activities: bool
-    has_notes: bool
-
-    def model_post_init(self, __context: Any) -> None:
-        self.odata_type = BASE_TYPE + "EntityMetadata"
-        return super().model_post_init(__context)
-
-
-def define_entity(
-    schema_name: str,
-    attributes: Sequence[AttributeTypes],
-    description: str | Label | None = None,
-    display_name: str | Label | None = None,
-    display_collection_name: str | Label | None = None,
-    ownership_type: OwnershipType = OwnershipType.NONE,
-    is_activity: bool = False,
-    has_activities: bool = False,
-    has_notes: bool = False,
-) -> EntityMetadata:
-    """
-    Defining an EntityMetadata instance.
-
-    Parameters
-    ----------
-    schema_name : str
-        Schema name of the Entity.
-    attributes : list of AttributeMetadata
-        List of `AttributeMetadata` where exactly one element must
-        represent the primary attribute for the Entity.
-    description: Optional string or `Label`
-        A short description of the Entity. Defaults to empty string.
-    display_name: Optional string or `Label`
-        The display name of the Entity.
-    display_collection_name:
-        The display name of the Entity Collection (plural).
-    """
-
-    _name = " ".join(schema_name.split("_")[1:])
-
-    # Handle labels
-    description = define_label(description)
-    display_name = define_label(display_name, _name)
-    display_collection_name = define_label(display_collection_name, _name + "s")
-
-    return EntityMetadata(
-        schema_name=schema_name,
-        attributes=attributes,
-        description=description,
-        display_name=display_name,
-        display_collection_name=display_collection_name,
-        ownership_type=ownership_type,
-        is_activity=is_activity,
-        has_activities=has_activities,
-        has_notes=has_notes,
-    )
-
-
-class AlternateKeyMetadata(MetadataBase):
-    schema_name: str
-    display_name: Label
-    key_attributes: Sequence[str]
-
-
-def get_altkey_metadata(
-    schema_name: str,
-    display_name: str | Label,
-    key_attributes: Collection[str],
-) -> AlternateKeyMetadata:
-    """
-    Get `AlternateKeyMetadata`.
-
-    Parameters
-    ----------
-    schema_name : str
-        Schema name of alternate key.
-    display_name : str | Label
-        Display name or Label for alternate key.
-    key_attributes : Collection[str]
-        Collection of strings that comprise the alternate key.
-    """
-    if isinstance(display_name, str):
-        display_name = define_label(display_name)
-
-    key_attributes = list(set(key_attributes))
-
-    return AlternateKeyMetadata(schema_name=schema_name, display_name=display_name, key_attributes=key_attributes)
+"""
+The Dataverse Entity metadata class, and a function to define it using as little
+data as possible for ease of use.
+"""
+
+
+from collections.abc import Collection, Sequence
+from typing import Any
+
+from dataverse_api.metadata.attributes import AttributeTypes
+from dataverse_api.metadata.base import BASE_TYPE, MetadataBase
+from dataverse_api.metadata.complex_properties import Label
+from dataverse_api.metadata.enums import OwnershipType
+from dataverse_api.utils.labels import define_label
+
+
+class EntityMetadata(MetadataBase):
+    """
+    Entity Metadata for Dataverse.
+    """
+
+    schema_name: str
+    description: Label
+    display_name: Label
+    display_collection_name: Label
+    attributes: Sequence[AttributeTypes] | None = None
+    ownership_type: OwnershipType
+    is_activity: bool
+    has_activities: bool
+    has_notes: bool
+
+    def model_post_init(self, __context: Any) -> None:
+        self.odata_type = BASE_TYPE + "EntityMetadata"
+        return super().model_post_init(__context)
+
+
+def define_entity(
+    schema_name: str,
+    attributes: Sequence[AttributeTypes],
+    description: str | Label | None = None,
+    display_name: str | Label | None = None,
+    display_collection_name: str | Label | None = None,
+    ownership_type: OwnershipType = OwnershipType.NONE,
+    is_activity: bool = False,
+    has_activities: bool = False,
+    has_notes: bool = False,
+) -> EntityMetadata:
+    """
+    Defining an EntityMetadata instance.
+
+    Parameters
+    ----------
+    schema_name : str
+        Schema name of the Entity.
+    attributes : list of AttributeMetadata
+        List of `AttributeMetadata` where exactly one element must
+        represent the primary attribute for the Entity.
+    description: Optional string or `Label`
+        A short description of the Entity. Defaults to empty string.
+    display_name: Optional string or `Label`
+        The display name of the Entity.
+    display_collection_name:
+        The display name of the Entity Collection (plural).
+    """
+
+    _name = " ".join(schema_name.split("_")[1:])
+
+    # Handle labels
+    description = define_label(description)
+    display_name = define_label(display_name, _name)
+    display_collection_name = define_label(display_collection_name, _name + "s")
+
+    return EntityMetadata(
+        schema_name=schema_name,
+        attributes=attributes,
+        description=description,
+        display_name=display_name,
+        display_collection_name=display_collection_name,
+        ownership_type=ownership_type,
+        is_activity=is_activity,
+        has_activities=has_activities,
+        has_notes=has_notes,
+    )
+
+
+class AlternateKeyMetadata(MetadataBase):
+    schema_name: str
+    display_name: Label
+    key_attributes: Sequence[str]
+
+
+def get_altkey_metadata(
+    schema_name: str,
+    display_name: str | Label,
+    key_attributes: Collection[str],
+) -> AlternateKeyMetadata:
+    """
+    Get `AlternateKeyMetadata`.
+
+    Parameters
+    ----------
+    schema_name : str
+        Schema name of alternate key.
+    display_name : str | Label
+        Display name or Label for alternate key.
+    key_attributes : Collection[str]
+        Collection of strings that comprise the alternate key.
+    """
+    if isinstance(display_name, str):
+        display_name = define_label(display_name)
+
+    key_attributes = list(set(key_attributes))
+
+    return AlternateKeyMetadata(schema_name=schema_name, display_name=display_name, key_attributes=key_attributes)
```

### Comparing `dataverse_api-1.1.4/dataverse_api/metadata/enums.py` & `dataverse_api-1.1.5/dataverse_api/metadata/enums.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,138 +1,138 @@
-"""
-A collection of Dataverse Enum metadata classes.
-"""
-from enum import Enum
-
-
-class BaseEnum(Enum):
-    """
-    Base Enum class as callable. Used for standard Enums that return only a string.
-    Note that the API payload requires the TitleCased Enum names and not the
-    integer counterparts listed in Microsofts resource pages.
-    """
-
-    def _get_value(self) -> str | dict[str, str]:
-        return self.value
-
-
-class StringFormat(BaseEnum):
-    """
-    Enum for String Format options.
-    """
-
-    EMAIL = {"value": "Email"}
-    TEXT = {"value": "Text"}
-    TEXT_AREA = {"value": "TextArea"}
-    URL = {"value": "Url"}
-    TICKER_SYMBOL = {"value": "TickerSymbol"}
-    PHONETIC_GUIDE = {"value": "PhoneticGuide"}
-    VERSION_NUMBER = {"value": "VersionNumber"}
-    # PHONE = {"value":"Phone"} Internal use only.
-    JSON = {"value": "Json"}
-    RICH_TEXT = {"value": "RichText"}
-
-
-class AttributeType(BaseEnum):
-    BIG_INT = "BigInt"
-    BOOLEAN = "Boolean"
-    DATE_TIME = "DateTime"
-    DECIMAL = "Decimal"
-    INTEGER = "Integer"
-    LOOKUP = "Lookup"
-    MEMO = "Memo"
-    STRING = "String"
-
-
-class AttributeTypeName(BaseEnum):
-    BIG_INT = {"value": "BigIntType"}
-    BOOLEAN = {"value": "BooleanType"}
-    DATE_TIME = {"value": "DateTimeType"}
-    DECIMAL = {"value": "DecimalType"}
-    INTEGER = {"value": "IntegerType"}
-    LOOKUP = {"value": "LookupType"}
-    MEMO = {"Value": "MemoType"}
-    STRING_TYPE = {"value": "StringType"}
-
-
-class AssociatedMenuBehavior(BaseEnum):
-    """
-    Enum for Associated Menu Behavior for Relationships.
-    """
-
-    USE_COLLECTION_NAME = "UseCollectionName"
-    USE_LABEL = "UseLabel"
-    DO_NOT_DISPLAY = "DoNotDisplay"
-
-
-class AssociatedMenuGroup(BaseEnum):
-    """
-    Enum for Associated Menu Group for Relationships.
-    """
-
-    DETAILS = "Details"
-    SALES = "Sales"
-    SERVICE = "Service"
-    MARKETING = "Marketing"
-
-
-class CascadeType(BaseEnum):
-    """
-    Enum for Cascade Types.
-    """
-
-    NO_CASCADE = "NoCascade"
-    CASCADE = "Cascade"
-    ACTIVE = "Active"
-    USER_OWNED = "UserOwned"
-    REMOVE_LINK = "RemoveLink"
-    RESTRICT = "Restrict"
-
-
-class DateTimeFormat(BaseEnum):
-    """
-    Enum for DateTime Formats.
-    """
-
-    DATE_ONLY = "DateOnly"
-    DATE_AND_TIME = "DateAndTime"
-
-
-class IntegerFormat(BaseEnum):
-    """
-    Enum for Integer Formats.
-    """
-
-    NONE = "None"
-    DURATION = "Duration"
-    TIME_ZONE = "TimeZone"
-    LANGUAGE = "Language"
-    LOCALE = "Locale"
-
-
-class MemoFormat(BaseEnum):
-    """
-    Enum for Memo Formats.
-    """
-
-    TEXT_AREA = "TextArea"
-    RICH_TEXT = "RichText"
-
-
-class OwnershipType(BaseEnum):
-    """
-    Enum for Ownership Types for Entities.
-    """
-
-    NONE = "None"
-    USER_OWNED = "UserOwned"
-    ORGANIZATION_OWNED = "OrganizationOwned"
-
-
-class AttributeRequiredLevel(BaseEnum):
-    """
-    Enum for Required Level of Attribute.
-    """
-
-    NONE = "None"
-    APPLICATION_REQUIRED = "ApplicationRequired"
-    RECOMMENDED = "Recommended"
+"""
+A collection of Dataverse Enum metadata classes.
+"""
+from enum import Enum
+
+
+class BaseEnum(Enum):
+    """
+    Base Enum class as callable. Used for standard Enums that return only a string.
+    Note that the API payload requires the TitleCased Enum names and not the
+    integer counterparts listed in Microsofts resource pages.
+    """
+
+    def _get_value(self) -> str | dict[str, str]:
+        return self.value
+
+
+class StringFormat(BaseEnum):
+    """
+    Enum for String Format options.
+    """
+
+    EMAIL = {"value": "Email"}
+    TEXT = {"value": "Text"}
+    TEXT_AREA = {"value": "TextArea"}
+    URL = {"value": "Url"}
+    TICKER_SYMBOL = {"value": "TickerSymbol"}
+    PHONETIC_GUIDE = {"value": "PhoneticGuide"}
+    VERSION_NUMBER = {"value": "VersionNumber"}
+    # PHONE = {"value":"Phone"} Internal use only.
+    JSON = {"value": "Json"}
+    RICH_TEXT = {"value": "RichText"}
+
+
+class AttributeType(BaseEnum):
+    BIG_INT = "BigInt"
+    BOOLEAN = "Boolean"
+    DATE_TIME = "DateTime"
+    DECIMAL = "Decimal"
+    INTEGER = "Integer"
+    LOOKUP = "Lookup"
+    MEMO = "Memo"
+    STRING = "String"
+
+
+class AttributeTypeName(BaseEnum):
+    BIG_INT = {"value": "BigIntType"}
+    BOOLEAN = {"value": "BooleanType"}
+    DATE_TIME = {"value": "DateTimeType"}
+    DECIMAL = {"value": "DecimalType"}
+    INTEGER = {"value": "IntegerType"}
+    LOOKUP = {"value": "LookupType"}
+    MEMO = {"Value": "MemoType"}
+    STRING_TYPE = {"value": "StringType"}
+
+
+class AssociatedMenuBehavior(BaseEnum):
+    """
+    Enum for Associated Menu Behavior for Relationships.
+    """
+
+    USE_COLLECTION_NAME = "UseCollectionName"
+    USE_LABEL = "UseLabel"
+    DO_NOT_DISPLAY = "DoNotDisplay"
+
+
+class AssociatedMenuGroup(BaseEnum):
+    """
+    Enum for Associated Menu Group for Relationships.
+    """
+
+    DETAILS = "Details"
+    SALES = "Sales"
+    SERVICE = "Service"
+    MARKETING = "Marketing"
+
+
+class CascadeType(BaseEnum):
+    """
+    Enum for Cascade Types.
+    """
+
+    NO_CASCADE = "NoCascade"
+    CASCADE = "Cascade"
+    ACTIVE = "Active"
+    USER_OWNED = "UserOwned"
+    REMOVE_LINK = "RemoveLink"
+    RESTRICT = "Restrict"
+
+
+class DateTimeFormat(BaseEnum):
+    """
+    Enum for DateTime Formats.
+    """
+
+    DATE_ONLY = "DateOnly"
+    DATE_AND_TIME = "DateAndTime"
+
+
+class IntegerFormat(BaseEnum):
+    """
+    Enum for Integer Formats.
+    """
+
+    NONE = "None"
+    DURATION = "Duration"
+    TIME_ZONE = "TimeZone"
+    LANGUAGE = "Language"
+    LOCALE = "Locale"
+
+
+class MemoFormat(BaseEnum):
+    """
+    Enum for Memo Formats.
+    """
+
+    TEXT_AREA = "TextArea"
+    RICH_TEXT = "RichText"
+
+
+class OwnershipType(BaseEnum):
+    """
+    Enum for Ownership Types for Entities.
+    """
+
+    NONE = "None"
+    USER_OWNED = "UserOwned"
+    ORGANIZATION_OWNED = "OrganizationOwned"
+
+
+class AttributeRequiredLevel(BaseEnum):
+    """
+    Enum for Required Level of Attribute.
+    """
+
+    NONE = "None"
+    APPLICATION_REQUIRED = "ApplicationRequired"
+    RECOMMENDED = "Recommended"
```

### Comparing `dataverse_api-1.1.4/dataverse_api/metadata/helpers.py` & `dataverse_api-1.1.5/dataverse_api/metadata/helpers.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,73 +1,73 @@
-"""
-Some helper definitions for key actions in Dataverse.
-These are not defined in Dataverse but are used to abstract some use-cases
-for this framework.
-"""
-from dataclasses import dataclass, field
-
-
-@dataclass(slots=True)
-class Publisher:
-    """
-    A class to define a new Dataverse Publisher.
-
-    Parameters
-    ----------
-    name : str
-        The display name of the Publisher.
-    unique_name : str
-        The unique name of the Publisher.
-    description : str
-    prefix: str
-        The prefix of Entities and Attributes associated with the Publisher.
-    option_prefix: int
-        The prefix of options for Choices associated with the Publisher.
-    """
-
-    name: str
-    unique_name: str
-    description: str
-    prefix: str
-    option_prefix: int
-
-    def __call__(self) -> dict[str, int | str]:
-        return {
-            "friendlyname": self.name,
-            "uniquename": self.unique_name,
-            "description": self.description,
-            "customizationprefix": self.prefix,
-            "customizationoptionvalueprefix": self.option_prefix,
-        }
-
-
-@dataclass(slots=True)
-class Solution:
-    """
-    A class to define a new Dataverse Solution.
-
-    Parameters
-    ----------
-    name : str
-        The display name of the Solution.
-    unique_name : str
-        The unique name of the Solution.
-    description : str
-        A description of the Solution.
-    publisher_guid : str
-        The Dataverse GUID of the associated Publisher.
-    """
-
-    name: str
-    unique_name: str
-    description: str
-    publisher_guid: str
-    version: str = field(init=False, default="1.0.0.0")
-
-    def __call__(self) -> dict[str, int | str]:
-        return {
-            "friendlyname": self.name,
-            "uniquename": self.unique_name,
-            "description": self.description,
-            "version": self.version,
-            "publisher@odata.bind": f"publishers({self.publisher_guid})",
-        }
+"""
+Some helper definitions for key actions in Dataverse.
+These are not defined in Dataverse but are used to abstract some use-cases
+for this framework.
+"""
+from dataclasses import dataclass, field
+
+
+@dataclass(slots=True)
+class Publisher:
+    """
+    A class to define a new Dataverse Publisher.
+
+    Parameters
+    ----------
+    name : str
+        The display name of the Publisher.
+    unique_name : str
+        The unique name of the Publisher.
+    description : str
+    prefix: str
+        The prefix of Entities and Attributes associated with the Publisher.
+    option_prefix: int
+        The prefix of options for Choices associated with the Publisher.
+    """
+
+    name: str
+    unique_name: str
+    description: str
+    prefix: str
+    option_prefix: int
+
+    def __call__(self) -> dict[str, int | str]:
+        return {
+            "friendlyname": self.name,
+            "uniquename": self.unique_name,
+            "description": self.description,
+            "customizationprefix": self.prefix,
+            "customizationoptionvalueprefix": self.option_prefix,
+        }
+
+
+@dataclass(slots=True)
+class Solution:
+    """
+    A class to define a new Dataverse Solution.
+
+    Parameters
+    ----------
+    name : str
+        The display name of the Solution.
+    unique_name : str
+        The unique name of the Solution.
+    description : str
+        A description of the Solution.
+    publisher_guid : str
+        The Dataverse GUID of the associated Publisher.
+    """
+
+    name: str
+    unique_name: str
+    description: str
+    publisher_guid: str
+    version: str = field(init=False, default="1.0.0.0")
+
+    def __call__(self) -> dict[str, int | str]:
+        return {
+            "friendlyname": self.name,
+            "uniquename": self.unique_name,
+            "description": self.description,
+            "version": self.version,
+            "publisher@odata.bind": f"publishers({self.publisher_guid})",
+        }
```

### Comparing `dataverse_api-1.1.4/dataverse_api/metadata/relationships.py` & `dataverse_api-1.1.5/dataverse_api/metadata/relationships.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,101 +1,101 @@
-"""
-A collection of Dataverse Relationship metadata classes.
-"""
-
-
-from typing import Any
-
-from pydantic import Field
-
-from dataverse_api.metadata.attributes import LookupAttributeMetadata
-from dataverse_api.metadata.base import BASE_TYPE, MetadataBase
-from dataverse_api.metadata.complex_properties import AssociatedMenuConfiguration, CascadeConfiguration, Label
-from dataverse_api.utils.labels import define_label
-
-
-class RelationshipMetadata(MetadataBase):
-    """
-    Base Metadata class for Relationships.
-    """
-
-    schema_name: str
-    is_valid_for_advanced_find: bool = True
-    description: Label | None = Field(default=None)
-    display_name: Label | None = Field(default=None)
-
-
-class OneToManyRelationshipMetadata(RelationshipMetadata):
-    """
-    Metadata for a One-to-Many relationship between Entities.
-    """
-
-    referenced_entity: str
-    referencing_entity: str
-    lookup: LookupAttributeMetadata
-    referenced_attribute: str | None = Field(default=None)
-    cascade_configuration: CascadeConfiguration = Field(default_factory=CascadeConfiguration)
-    associated_menu_configuration: AssociatedMenuConfiguration = Field(default_factory=AssociatedMenuConfiguration)
-
-    def model_post_init(self, __context: Any) -> None:
-        self.odata_type = BASE_TYPE + "OneToManyRelationshipMetadata"
-        return super().model_post_init(__context)
-
-
-def define_relationship(
-    schema_name: str,
-    referencing_entity: str,
-    referenced_entity: str,
-    lookup: str | LookupAttributeMetadata,
-    *,
-    referenced_attribute: str | None = None,
-    description: str | Label | None = None,
-    display_name: str | Label | None = None,
-    is_valid_for_advanced_find: bool = True,
-) -> OneToManyRelationshipMetadata:
-    """
-    Defines a RelationshipMetadata between the referencing Entity (on the many-side)
-    and the referenced Entity (on the one-side).
-
-    Parameters
-    ----------
-    schema_name : str
-        The Schema name for the Relationship.
-    referencing_entity: str
-        The Entity on the many-side of the Relationship.
-    referenced_entity: str
-        The Entity on the one-side of the Relationship.
-    referenced_attribute:
-        The attribute referenced by the Relationship.
-    lookup : str or LookupAttributeMetadata
-        Either a fully defined LookupAttributeMetadata or the
-        schema name of the lookup column that will be created
-        in the referencing Entity.
-    description : str or `Label`
-        Defines the description of the Relationship.
-    display_name: str or `Label`
-        The display name of the Relationship.
-    """
-    _name = " ".join(schema_name.split(" ")[1:])
-
-    description = define_label(label=description, override="")
-    display_name = define_label(label=display_name, override=_name)
-
-    if isinstance(lookup, str):
-        lookup_label = define_label(f"Relationship between {referencing_entity} and {referenced_entity}.")
-
-        lookup = LookupAttributeMetadata(
-            schema_name=f"rel_{referenced_entity[:41]}",
-            description=lookup_label,
-            display_name=lookup_label,
-        )
-
-    return OneToManyRelationshipMetadata(
-        schema_name=schema_name,
-        description=description,
-        display_name=display_name,
-        is_valid_for_advanced_find=is_valid_for_advanced_find,
-        referenced_attribute=referenced_attribute,
-        referenced_entity=referenced_entity,
-        referencing_entity=referencing_entity,
-        lookup=lookup,
-    )
+"""
+A collection of Dataverse Relationship metadata classes.
+"""
+
+
+from typing import Any
+
+from pydantic import Field
+
+from dataverse_api.metadata.attributes import LookupAttributeMetadata
+from dataverse_api.metadata.base import BASE_TYPE, MetadataBase
+from dataverse_api.metadata.complex_properties import AssociatedMenuConfiguration, CascadeConfiguration, Label
+from dataverse_api.utils.labels import define_label
+
+
+class RelationshipMetadata(MetadataBase):
+    """
+    Base Metadata class for Relationships.
+    """
+
+    schema_name: str
+    is_valid_for_advanced_find: bool = True
+    description: Label | None = Field(default=None)
+    display_name: Label | None = Field(default=None)
+
+
+class OneToManyRelationshipMetadata(RelationshipMetadata):
+    """
+    Metadata for a One-to-Many relationship between Entities.
+    """
+
+    referenced_entity: str
+    referencing_entity: str
+    lookup: LookupAttributeMetadata
+    referenced_attribute: str | None = Field(default=None)
+    cascade_configuration: CascadeConfiguration = Field(default_factory=CascadeConfiguration)
+    associated_menu_configuration: AssociatedMenuConfiguration = Field(default_factory=AssociatedMenuConfiguration)
+
+    def model_post_init(self, __context: Any) -> None:
+        self.odata_type = BASE_TYPE + "OneToManyRelationshipMetadata"
+        return super().model_post_init(__context)
+
+
+def define_relationship(
+    schema_name: str,
+    referencing_entity: str,
+    referenced_entity: str,
+    lookup: str | LookupAttributeMetadata,
+    *,
+    referenced_attribute: str | None = None,
+    description: str | Label | None = None,
+    display_name: str | Label | None = None,
+    is_valid_for_advanced_find: bool = True,
+) -> OneToManyRelationshipMetadata:
+    """
+    Defines a RelationshipMetadata between the referencing Entity (on the many-side)
+    and the referenced Entity (on the one-side).
+
+    Parameters
+    ----------
+    schema_name : str
+        The Schema name for the Relationship.
+    referencing_entity: str
+        The Entity on the many-side of the Relationship.
+    referenced_entity: str
+        The Entity on the one-side of the Relationship.
+    referenced_attribute:
+        The attribute referenced by the Relationship.
+    lookup : str or LookupAttributeMetadata
+        Either a fully defined LookupAttributeMetadata or the
+        schema name of the lookup column that will be created
+        in the referencing Entity.
+    description : str or `Label`
+        Defines the description of the Relationship.
+    display_name: str or `Label`
+        The display name of the Relationship.
+    """
+    _name = " ".join(schema_name.split(" ")[1:])
+
+    description = define_label(label=description, override="")
+    display_name = define_label(label=display_name, override=_name)
+
+    if isinstance(lookup, str):
+        lookup_label = define_label(f"Relationship between {referencing_entity} and {referenced_entity}.")
+
+        lookup = LookupAttributeMetadata(
+            schema_name=f"rel_{referenced_entity[:41]}",
+            description=lookup_label,
+            display_name=lookup_label,
+        )
+
+    return OneToManyRelationshipMetadata(
+        schema_name=schema_name,
+        description=description,
+        display_name=display_name,
+        is_valid_for_advanced_find=is_valid_for_advanced_find,
+        referenced_attribute=referenced_attribute,
+        referenced_entity=referenced_entity,
+        referencing_entity=referencing_entity,
+        lookup=lookup,
+    )
```

### Comparing `dataverse_api-1.1.4/dataverse_api/utils/batching.py` & `dataverse_api-1.1.5/dataverse_api/utils/batching.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,235 +1,235 @@
-from collections.abc import Iterable, Sequence
-from dataclasses import dataclass, field
-from enum import Enum, auto
-from textwrap import dedent
-from typing import Any, Collection, Generator, Mapping, MutableMapping, TypeVar
-from urllib.parse import urljoin
-
-from dataverse_api.utils.data import serialize_json
-from dataverse_api.utils.text import encode_altkeys
-
-T = TypeVar("T")
-
-
-class RequestMethod(Enum):
-    GET = auto()
-    POST = auto()
-    PATCH = auto()
-    PUT = auto()
-    DELETE = auto()
-
-
-@dataclass
-class APICommand:
-    """
-    For encapsulating a single request.
-
-    Parameters
-    ----------
-    url : str
-    method : str
-    """
-
-    url: str
-    method: RequestMethod
-    headers: Mapping[str, str] | None = None
-    params: Mapping[str, str] | None = None
-    data: str | None = None
-    json: MutableMapping[str, Any] | None = None
-
-
-@dataclass(slots=True)
-class BatchCommand:
-    """
-    For encapsulating a singular Dataverse batch command.
-
-    Parameters
-    ----------
-    url : str
-        The url that will be appended to the endpoint url.
-    method : RequestMethod
-        The request method for the batch command.
-    headers : dict
-        Any additional headers to pass for the specific batch command.
-    data : dict
-        Optional JSON serializable payload depending on request method.
-    """
-
-    url: str
-    method: RequestMethod
-    headers: Mapping[str, str] | None = field(default=None)
-    data: Mapping[str, Any] | None = field(default=None)
-    extra_header: str = field(init=False, default="")
-    single_col: bool = field(init=False, default=False)
-    content_type: str = field(init=False, default="Content-Type: application/json")
-
-    def __post_init__(self) -> None:
-        if self.method == RequestMethod.PUT:
-            self.single_col = True
-            assert self.data is not None
-            assert len(self.data) == 1
-            col, value = list(self.data.items())[0]
-            self.url += f"/{col}"
-            self.data = {"value": value}
-
-        if self.method == RequestMethod.POST:
-            self.content_type += "; type=entry"
-
-        if self.headers:
-            print("Extra!")
-            self.extra_header = "\n".join([f"{k}: {v}" for k, v in self.headers.items()])
-
-        self.url = encode_altkeys(self.url)
-
-    def encode(self, batch_id: str, api_url: str) -> str:
-        """
-        Encodes the batch command into a string.
-
-        Parameters
-        ----------
-        batch_id : str
-            A generated batch ID.
-        api_url : str
-            The base API endpoint.
-
-        Returns
-        -------
-        str
-            The batch command encoded as a string.
-        """
-
-        url = urljoin(api_url, self.url)
-
-        row_command = f"""\
-        --{batch_id}
-        Content-Type: application/http
-        Content-Transfer-Encoding: binary
-
-        {self.method.name} {url} HTTP/1.1
-        {self.content_type}
-        {self.extra_header}\n
-        {serialize_json(self.data)}
-        """
-        return dedent(row_command)
-
-
-def chunk_data(data: Sequence[T], size: int = 500) -> Generator[Sequence[T], None, None]:
-    """
-    Simple function to chunk a list into a maximum number of
-    elements per chunk.
-
-    Parameters
-    ----------
-    data : list of `DataverseBatchCommand`
-        List containing all commands to be chunked.
-    size: int, optional
-        Chunking size.
-
-    Yields
-    ------
-    list of `DataverseBatchCommand`
-    """
-    for i in range(0, len(data), size):
-        yield data[i : i + size]  # noqa E203
-
-
-def transform_to_batch_for_create(
-    url: str,
-    data: Collection[Mapping[str, Any]],
-) -> list[BatchCommand]:
-    """Transform data payload to creation batch data."""
-    return [BatchCommand(url, method=RequestMethod.POST, data=row) for row in data]
-
-
-def transform_to_batch_for_delete(url: str, data: Iterable[str], column: str | None = None) -> list[BatchCommand]:
-    """
-    Transform data payload to deletion batch data.
-
-    Parameters
-    ----------
-    url : str
-        The EntitySetName of targeted Dataverse Entity.
-    data : iterable of str
-        Primary IDs for deletion.
-    column : str
-        Optional column to target for deletion.
-
-    Returns
-    -------
-    list of BatchDataCommand
-        Payload for passing to the API batch call endpoint.
-    """
-    column = "" if column is None else f"/{column}"
-    return [BatchCommand(url=f"{url}({id}){column}", method=RequestMethod.DELETE) for id in data]
-
-
-UpsertDataType = tuple[str, dict[str, Any]]
-
-
-def transform_upsert_data(
-    data: Collection[Mapping[str, Any]],
-    keys: Iterable[str],
-    is_primary_id: bool,
-) -> Generator[UpsertDataType, None, None]:
-    """
-    Transform upsert data to keys and payload.
-
-    Parameters
-    ----------
-    data : Collection[Mapping[str, Any]]
-        The data to upsert to Dataverse.
-    keys : Iterable[str]
-        The keys to extract from the data to form the target row identifier.
-    is_primary_id : bool
-        Whether the given key (singular) is the primary ID attribute for the Entity.
-
-    Yields
-    -------
-    tuple : str, dict
-        [0] : The target row identifier
-        [1] : The data payload
-    """
-    for row in data:
-        if is_primary_id:
-            # No repr on string
-            row_key = [f"{row[part]}" for part in keys]
-        else:
-            # Repr on string
-            row_key = [f"{part}={row[part].__repr__()}" for part in keys]
-        row_data = {k: v for k, v in row.items() if k not in keys}
-
-        yield ",".join(row_key), row_data
-
-
-def transform_to_batch_for_upsert(
-    url: str,
-    data: Collection[MutableMapping[str, Any]],
-    keys: Iterable[str],
-    is_primary_id: bool = False,
-) -> list[BatchCommand]:
-    """
-    Transform data payload to upsert batch data.
-
-    Parameters
-    ----------
-    url : str
-        The Entity endpoint for upsertion.
-    data : collection of data dictionaries
-        The data to be upserted into Dataverse.
-    keys : iterable of str
-        The keys used to identify unique rows in the dataset.
-    is_id : bool
-        Whether the supplied singular key is the Entity primary ID attribute.
-    """
-    commands = []
-
-    for keys, payload in transform_upsert_data(data, keys, is_primary_id):
-        commands.append(
-            BatchCommand(
-                url=f"{url}({keys})",
-                method=RequestMethod.PATCH,
-                data=payload,
-            )
-        )
-
-    return commands
+from collections.abc import Iterable, Sequence
+from dataclasses import dataclass, field
+from enum import StrEnum
+from textwrap import dedent
+from typing import Any, Collection, Generator, Mapping, MutableMapping, TypeVar
+from urllib.parse import urljoin
+
+from dataverse_api.utils.data import serialize_json
+from dataverse_api.utils.text import encode_altkeys
+
+T = TypeVar("T")
+
+
+class RequestMethod(StrEnum):
+    GET = "GET"
+    POST = "POST"
+    PATCH = "PATCH"
+    PUT = "PUT"
+    DELETE = "DELETE"
+
+
+@dataclass
+class APICommand:
+    """
+    For encapsulating a single request.
+
+    Parameters
+    ----------
+    url : str
+    method : str
+    """
+
+    url: str
+    method: RequestMethod
+    headers: Mapping[str, str] | None = None
+    params: Mapping[str, str] | None = None
+    data: str | None = None
+    json: MutableMapping[str, Any] | None = None
+
+
+@dataclass(slots=True)
+class BatchCommand:
+    """
+    For encapsulating a singular Dataverse batch command.
+
+    Parameters
+    ----------
+    url : str
+        The url that will be appended to the endpoint url.
+    method : RequestMethod
+        The request method for the batch command.
+    headers : dict
+        Any additional headers to pass for the specific batch command.
+    data : dict
+        Optional JSON serializable payload depending on request method.
+    """
+
+    url: str
+    method: RequestMethod
+    headers: Mapping[str, str] | None = field(default=None)
+    data: Mapping[str, Any] | None = field(default=None)
+    extra_header: str = field(init=False, default="")
+    single_col: bool = field(init=False, default=False)
+    content_type: str = field(init=False, default="Content-Type: application/json")
+
+    def __post_init__(self) -> None:
+        if self.method == RequestMethod.PUT:
+            self.single_col = True
+            assert self.data is not None
+            assert len(self.data) == 1
+            col, value = list(self.data.items())[0]
+            self.url += f"/{col}"
+            self.data = {"value": value}
+
+        if self.method == RequestMethod.POST:
+            self.content_type += "; type=entry"
+
+        if self.headers:
+            print("Extra!")
+            self.extra_header = "\n".join([f"{k}: {v}" for k, v in self.headers.items()])
+
+        self.url = encode_altkeys(self.url)
+
+    def encode(self, batch_id: str, api_url: str) -> str:
+        """
+        Encodes the batch command into a string.
+
+        Parameters
+        ----------
+        batch_id : str
+            A generated batch ID.
+        api_url : str
+            The base API endpoint.
+
+        Returns
+        -------
+        str
+            The batch command encoded as a string.
+        """
+
+        url = urljoin(api_url, self.url)
+
+        row_command = f"""\
+        --{batch_id}
+        Content-Type: application/http
+        Content-Transfer-Encoding: binary
+
+        {self.method} {url} HTTP/1.1
+        {self.content_type}
+        {self.extra_header}\n
+        {serialize_json(self.data)}
+        """
+        return dedent(row_command)
+
+
+def chunk_data(data: Sequence[T], size: int = 500) -> Generator[Sequence[T], None, None]:
+    """
+    Simple function to chunk a list into a maximum number of
+    elements per chunk.
+
+    Parameters
+    ----------
+    data : list of `DataverseBatchCommand`
+        List containing all commands to be chunked.
+    size: int, optional
+        Chunking size.
+
+    Yields
+    ------
+    list of `DataverseBatchCommand`
+    """
+    for i in range(0, len(data), size):
+        yield data[i : i + size]  # noqa E203
+
+
+def transform_to_batch_for_create(
+    url: str,
+    data: Collection[Mapping[str, Any]],
+) -> list[BatchCommand]:
+    """Transform data payload to creation batch data."""
+    return [BatchCommand(url, method=RequestMethod.POST, data=row) for row in data]
+
+
+def transform_to_batch_for_delete(url: str, data: Iterable[str], column: str | None = None) -> list[BatchCommand]:
+    """
+    Transform data payload to deletion batch data.
+
+    Parameters
+    ----------
+    url : str
+        The EntitySetName of targeted Dataverse Entity.
+    data : iterable of str
+        Primary IDs for deletion.
+    column : str
+        Optional column to target for deletion.
+
+    Returns
+    -------
+    list of BatchDataCommand
+        Payload for passing to the API batch call endpoint.
+    """
+    column = "" if column is None else f"/{column}"
+    return [BatchCommand(url=f"{url}({id}){column}", method=RequestMethod.DELETE) for id in data]
+
+
+UpsertDataType = tuple[str, dict[str, Any]]
+
+
+def transform_upsert_data(
+    data: Collection[Mapping[str, Any]],
+    keys: Iterable[str],
+    is_primary_id: bool,
+) -> Generator[UpsertDataType, None, None]:
+    """
+    Transform upsert data to keys and payload.
+
+    Parameters
+    ----------
+    data : Collection[Mapping[str, Any]]
+        The data to upsert to Dataverse.
+    keys : Iterable[str]
+        The keys to extract from the data to form the target row identifier.
+    is_primary_id : bool
+        Whether the given key (singular) is the primary ID attribute for the Entity.
+
+    Yields
+    -------
+    tuple : str, dict
+        [0] : The target row identifier
+        [1] : The data payload
+    """
+    for row in data:
+        if is_primary_id:
+            # No repr on string
+            row_key = [f"{row[part]}" for part in keys]
+        else:
+            # Repr on string
+            row_key = [f"{part}={row[part].__repr__()}" for part in keys]
+        row_data = {k: v for k, v in row.items() if k not in keys}
+
+        yield ",".join(row_key), row_data
+
+
+def transform_to_batch_for_upsert(
+    url: str,
+    data: Collection[MutableMapping[str, Any]],
+    keys: Iterable[str],
+    is_primary_id: bool = False,
+) -> list[BatchCommand]:
+    """
+    Transform data payload to upsert batch data.
+
+    Parameters
+    ----------
+    url : str
+        The Entity endpoint for upsertion.
+    data : collection of data dictionaries
+        The data to be upserted into Dataverse.
+    keys : iterable of str
+        The keys used to identify unique rows in the dataset.
+    is_id : bool
+        Whether the supplied singular key is the Entity primary ID attribute.
+    """
+    commands = []
+
+    for keys, payload in transform_upsert_data(data, keys, is_primary_id):
+        commands.append(
+            BatchCommand(
+                url=f"{url}({keys})",
+                method=RequestMethod.PATCH,
+                data=payload,
+            )
+        )
+
+    return commands
```

### Comparing `dataverse_api-1.1.4/LICENSE` & `dataverse_api-1.1.5/LICENSE`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2023 Marcus Risanger
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2023 Marcus Risanger
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `dataverse_api-1.1.4/pyproject.toml` & `dataverse_api-1.1.5/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,39 +1,40 @@
-[tool.poetry]
-name = "dataverse-api"
-version = "1.1.4"
-description = "Abstraction layer for interacting with Microsoft Dataverse Web API using Python."
-authors = ["Marcus Risanger <69350948+MarcusRisanger@users.noreply.github.com>"]
-readme = "README.md"
-
-[tool.poetry.dependencies]
-python = "^3.11"
-msal = "^1.26.0"
-msal-requests-auth = "^0.7.0"
-pandas = "^2.0.1"
-sqlalchemy = "^2.0.23"
-pyodbc = "^5.0.1"
-pydantic = "^2.5.3"
-
-
-[tool.poetry.group.dev.dependencies]
-ipykernel = "^6.26.0"
-python-dotenv = "^1.0.0"
-pre-commit = "^3.5.0"
-coverage = "^7.4.0"
-pytest = "^7.4.3"
-pytest-mock = "^3.12.0"
-requests-mock = "^1.11.0"
-responses = "^0.24.1"
-types-requests = "^2.31.0.10"
-pytest-xdist = "^3.5.0"
-pandas-stubs = "^2.1.4.231218"
-ruff = "^0.1.9"
-
-[build-system]
-requires = ["poetry-core"]
-build-backend = "poetry.core.masonry.api"
-
-
-[tool.ruff]
-line-length = 120
-ignore-init-module-imports = true
+[tool.poetry]
+name = "dataverse-api"
+version = "1.1.5"
+description = "Abstraction layer for interacting with Microsoft Dataverse Web API using Python."
+authors = ["Marcus Risanger <69350948+MarcusRisanger@users.noreply.github.com>"]
+readme = "README.md"
+
+[tool.poetry.dependencies]
+python = "^3.11"
+msal = "^1.26.0"
+msal-requests-auth = "^0.7.0"
+pandas = "^2.0.1"
+sqlalchemy = "^2.0.23"
+pyodbc = "^5.0.1"
+pydantic = "^2.5.3"
+
+
+[tool.poetry.group.dev.dependencies]
+ipykernel = "^6.26.0"
+python-dotenv = "^1.0.0"
+pre-commit = "^3.5.0"
+coverage = "^7.4.0"
+pytest = "^7.4.3"
+pytest-mock = "^3.12.0"
+requests-mock = "^1.11.0"
+responses = "^0.24.1"
+types-requests = "^2.31.0.10"
+pytest-xdist = "^3.5.0"
+pandas-stubs = "^2.1.4.231218"
+ruff = "^0.4.4"
+tabulate = "^0.9.0"
+
+[build-system]
+requires = ["poetry-core"]
+build-backend = "poetry.core.masonry.api"
+
+
+[tool.ruff]
+line-length = 120
+ignore-init-module-imports = true
```

### Comparing `dataverse_api-1.1.4/README.md` & `dataverse_api-1.1.5/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,261 +1,261 @@
-# `dataverse-api`
-
-[![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
-[![Build Status](https://github.com/MarcusRisanger/dataverse-api/workflows/release/badge.svg)](https://github.com/MarcusRisanger/dataverse-api/actions)
-[![codecov](https://codecov.io/gh/MarcusRisanger/Dataverse-API/branch/main/graph/badge.svg)](https://codecov.io/gh/MarcusRisanger/Dataverse-API)
-
-The `dataverse-api` package is an abstraction layer developed for allowing simple interaction with Microsoft Dataverse Web API.
-
-# Table of Contents
-* [Description](#Description)
-* [Getting Started](#getting-started)
-* [Development environment](#development-environment)
-    * [Code requirements](#code-requirements)
-    * [Testing](#testing)
-* [To do](#to-do)
-* [Usage](#usage)
-    * [DataverseClient](#dataverseclient)
-        * [Initialize DataverseClient](#initialize-dataverseclient)
-        * [Create new Entity](#create-new-entity)
-        * [Update existing Entity](#update-existing-entity)
-    * [DataverseEntity](#dataverseentity)
-        * [Initialize Entity interface](#initialize-interface-with-entity)
-        * [Read](#read)
-        * [Create](#create)
-        * [Upsert](#upsert)
-        * [Delete](#delete)
-        * [Add and remove Attributes](#add-and-remove-attributes)
-        * [Add and remove Alternate Keys](#add-and-remove-alternate-keys)
-
-
-
-# Description
-
-The main goal of this project was to enable some use-cases against Dataverse that I wanted to explore for a work assignment, while getting some experience in programming and testing out different ways of setting up the codebase.
-
-The functionality I have built into this Dataverse wrapper constitutes the functionality I have wanted to explore myself.
-
-Most important is to enable creating, upserting, updating and deleting rows of data into Dataverse tables using common data structures, and implementing choices on how these requests are to be formed. For example, when creating new rows, the user can choose between individual `POST` requests per row, combining data into batch requests against the `$batch` endpoint, or even to use the `CreateMultiple` Dataverse action.
-
-The framework is written in Python 3.11, seeing as this runtime is available in the current release of Azure Functions.
-
-## Getting started
-
-Usage is fairly simple - authentication must be handled by the user. The `DataverseClient` simply accepts an already authorized `requests.Session` with which to handle API requests.
-
-I suggest using `msal` and `msal-requests-auth` for authenticating the `Session`. The examples below include this way of implementing auth:
-
-```python
-import os
-
-from msal import ConfidentialClientApplication
-from msal_requests_auth.auth import ClientCredentialAuth
-from requests import Session
-
-from dataverse_api import DataverseClient
-
-# Prepare Auth
-app_reg = ConfidentialClientApplication(
-    client_id=os.getenv("app_id"),
-    client_credential=os.getenv("client_secret"),
-    authority=os.getenv("authority_url"),
-)
-environment_url = os.getenv("environment_url")
-auth = ClientCredentialAuth(
-    client=app_reg,
-    scopes=[environment_url + "/.default"]
-)
-
-# Prepare Session
-session = Session()
-session.auth = auth
-
-# Instantiate DataverseClient
-client = DataverseClient(session=session, environment_url=environment_url)
-
-# Instantiate interface to Entity
-entity = client.entity(logical_name="organization")
-
-# Read data!
-entity.read(select=["name"])
-```
-
-
-## Development environment
-
-[poetry](https://python-poetry.org) is used for managing dependencies. To develop
-`dataverse-api`, follow the below steps to set up your local environment:
-
-1.  [Install poetry](https://python-poetry.org/docs/#installation) if you haven't already.
-
-2.  Clone repository:
-    ```
-    $ git clone git@github.com:MarcusRisanger/dataverse-api.git
-    ```
-3.  Move into the newly created local repository:
-    ```
-    $ cd dataverse-api
-    ```
-4.  Create virtual environment and install dependencies:
-    ```
-    $ poetry install
-    ```
-
-### Code requirements
-
-All code must pass [ruff](https://github.com/astral-sh/ruff) style checks to be merged. It is recommended to install pre-commit hooks to ensure this locally before commiting code:
-
-```
-$ poetry run pre-commit install
-```
-
-Each public method, class and module should have docstrings. Docstrings are written in the Numpy style.
-
-### Testing
-
-To produce Coverage reports, run the following commands:
-
-```
-$ poetry run coverage run -m pytest
-$ poetry run coverage xml
-```
-
-## To Do:
-* Documentation ..
-* Metadata
-    - Choice
-    - Multichoice
-    - Money
-* Entity implementation
-    - Illegal file extensions
-    - Upload file
-    - Upload image
-    - Upload large file
-    - Add / remove relationships
-    - Add relationships (single/collection valued) as attr on entity
-    - Add columns as attr on entity
-* Add Tests:
-    - Add column
-    - Remove column
-    - Add alternate key
-    - Remove alternate key
-* Implement `CreateMultiple` request if creating more than 100 elements?
-    - https://learn.microsoft.com/en-us/power-apps/developer/data-platform/bulk-operations?tabs=webapi#createmultiple
-* Implement BulkDelete Action?
-    - https://learn.microsoft.com/en-us/power-apps/developer/data-platform/delete-data-bulk?tabs=sdk
-
-# Usage
-
-## DataverseClient
-
-### Initialize DataverseClient
-
-For now, I've coded the framework around the `requests` library, for good and bad! In the future, I will consider generalizing further, letting the user pass an authenticated requests handler of choice to the framework by specifying a `Protocol` to follow instead.
-
-To instantiate, pass a `requests.Session` together with a Dataverse environment URL to the `DataverseClient` constructor:
-
-```python
-session = Session()
-session.auth = auth
-environment_url = os.getenv("dataverse_url")
-
-client = DataverseClient(session=session, environment_url=environment_url)
-```
-
-### Create new Entity
-
-It is possible to create a new Entity using the `DataverseClient`. This requires a full `EntityMetadata` definition according to Dataverse standards. You can make this yourself and follow the `MetadataDumper` protocol, or use the provided `define_entity` function.
-
-The `define_label` function makes it simple to generate `Label` metadata with correct `LocalizedLabels` in its payload.
-
-In the example below, the optional `return_representation` argument has been set to `True` to receive the full Entity metadata definition as created by Dataverse as part of the server response. The response can be parsed by `EntityMetadata` classmethod to get a full fledged object for editing.
-
-```python
-from dataverse_api.metadata.attributes import StringAttributeMetadata
-from dataverse_api.metadata.entity import EntityMetadata, define_entity
-from dataverse_api.utils.labels import define_label
-
-new_entity = define_entity(
-    schema_name="new_name",
-    attributes=[StringAttributeMetadata(
-        schema_name="new_primary_col",
-        is_primary_name = True,
-        description=define_label("Primary column for Entity."),
-        display_name=define_label("Autonumber Column"),
-        auto_number_format="{SEQNUM:6}-#-{RANDSTRING:3}")],
-    description=define_label("Entity Created by Client"),
-    display_name=define_label("Programmatically Created Table")
-)
-
-resp = client.create_entity(new_entity, return_representation=True)
-entity_meta = EntityMetadata.model_validate_dataverse(resp.json())
-```
-
-### Update existing Entity
-
-You can update an existing Entity definition easily by retrieving the Entity metadata definition, and reupload an adjusted version.
-
-Below is a simple example. Note that this method also supports `return_representation` in the same manner as the `DataverseClient.create_entity()` method, if you want to return the edited Entity metadata as persisted in Dataverse.
-
-```python
-metadata = client.get_entity_definition("new_name")
-metadata.display_name.localized_labels[0].label = "Overridden Display Name"
-
-client.update_entity(metadata)
-```
-
-## DataverseEntity
-
-### Initialize interface with Entity
-
-To initializes an interface with a specific Dataverse Entity, use the `DataverseClient.entity()` method. It returns a `DataverseEntity` object that allows interaction with this specific entity.
-
-```python
-entity = client.entity(logical_name="foo")
-```
-As of now, only `LogicalName` is supported for instantiating a new `DataverseEntity` object.
-
-
-### Read
-
-The `DataverseEntity.read()` method has been furnished with the necessary arguments to do querying as specified in the [Microsoft Dataverse documentation](https://learn.microsoft.com/en-us/power-apps/developer/data-platform/webapi/query-data-web-api?view=dataverse-latest).
-
-A simple example:
-
-```python
-data = entity.read(select=["name","address"], filter="salary gt 10000", top=5, order_by="salary desc")
-```
-
-### Create
-
-To create rows, you can use a `pandas.DataFrame` or a simple construct like a list of dicts, where each dict contains the data for a single row.
-
-Below is an example of creating rows in the Entity by passing a dataframe and specifying that the creation method should be the `CreateMultiple` web API Action. The `return_created` argument can be set to `True` if you need the IDs as reference.
-
-```python
-entity.create(data=df, mode="multiple", return_created=True)
-```
-
-Note that the different modes provide different content when `return_created` is set to `True` - the script simply sets a `Prefer` header to include created data in the server response.
-
-For now the user may choose how to handle this based on the list of `requests.Response` objects that will be returned by the method.
-
-### Upsert
-
-Upserting data into Dataverse is simple. If you are just updating existing data you may have the URI (Primary Attribute ID) in your data. You can then omit the `alternate_key` argument.
-
-```python
-entity.upsert(data=df, alternate_key="my_key", mode="batch")
-```
-
-### Delete
-
-TBD
-
-### Add and remove Attributes
-
-TBD
-
-## Add and remove Alternate Keys
-
-TBD
+# `dataverse-api`
+
+[![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
+[![Build Status](https://github.com/MarcusRisanger/dataverse-api/workflows/release/badge.svg)](https://github.com/MarcusRisanger/dataverse-api/actions)
+[![codecov](https://codecov.io/gh/MarcusRisanger/Dataverse-API/branch/main/graph/badge.svg)](https://codecov.io/gh/MarcusRisanger/Dataverse-API)
+
+The `dataverse-api` package is an abstraction layer developed for allowing simple interaction with Microsoft Dataverse Web API.
+
+# Table of Contents
+* [Description](#Description)
+* [Getting Started](#getting-started)
+* [Development environment](#development-environment)
+    * [Code requirements](#code-requirements)
+    * [Testing](#testing)
+* [To do](#to-do)
+* [Usage](#usage)
+    * [DataverseClient](#dataverseclient)
+        * [Initialize DataverseClient](#initialize-dataverseclient)
+        * [Create new Entity](#create-new-entity)
+        * [Update existing Entity](#update-existing-entity)
+    * [DataverseEntity](#dataverseentity)
+        * [Initialize Entity interface](#initialize-interface-with-entity)
+        * [Read](#read)
+        * [Create](#create)
+        * [Upsert](#upsert)
+        * [Delete](#delete)
+        * [Add and remove Attributes](#add-and-remove-attributes)
+        * [Add and remove Alternate Keys](#add-and-remove-alternate-keys)
+
+
+
+# Description
+
+The main goal of this project was to enable some use-cases against Dataverse that I wanted to explore for a work assignment, while getting some experience in programming and testing out different ways of setting up the codebase.
+
+The functionality I have built into this Dataverse wrapper constitutes the functionality I have wanted to explore myself.
+
+Most important is to enable creating, upserting, updating and deleting rows of data into Dataverse tables using common data structures, and implementing choices on how these requests are to be formed. For example, when creating new rows, the user can choose between individual `POST` requests per row, combining data into batch requests against the `$batch` endpoint, or even to use the `CreateMultiple` Dataverse action.
+
+The framework is written in Python 3.11, seeing as this runtime is available in the current release of Azure Functions.
+
+## Getting started
+
+Usage is fairly simple - authentication must be handled by the user. The `DataverseClient` simply accepts an already authorized `requests.Session` with which to handle API requests.
+
+I suggest using `msal` and `msal-requests-auth` for authenticating the `Session`. The examples below include this way of implementing auth:
+
+```python
+import os
+
+from msal import ConfidentialClientApplication
+from msal_requests_auth.auth import ClientCredentialAuth
+from requests import Session
+
+from dataverse_api import DataverseClient
+
+# Prepare Auth
+app_reg = ConfidentialClientApplication(
+    client_id=os.getenv("app_id"),
+    client_credential=os.getenv("client_secret"),
+    authority=os.getenv("authority_url"),
+)
+environment_url = os.getenv("environment_url")
+auth = ClientCredentialAuth(
+    client=app_reg,
+    scopes=[environment_url + "/.default"]
+)
+
+# Prepare Session
+session = Session()
+session.auth = auth
+
+# Instantiate DataverseClient
+client = DataverseClient(session=session, environment_url=environment_url)
+
+# Instantiate interface to Entity
+entity = client.entity(logical_name="organization")
+
+# Read data!
+entity.read(select=["name"])
+```
+
+
+## Development environment
+
+[poetry](https://python-poetry.org) is used for managing dependencies. To develop
+`dataverse-api`, follow the below steps to set up your local environment:
+
+1.  [Install poetry](https://python-poetry.org/docs/#installation) if you haven't already.
+
+2.  Clone repository:
+    ```
+    $ git clone git@github.com:MarcusRisanger/dataverse-api.git
+    ```
+3.  Move into the newly created local repository:
+    ```
+    $ cd dataverse-api
+    ```
+4.  Create virtual environment and install dependencies:
+    ```
+    $ poetry install
+    ```
+
+### Code requirements
+
+All code must pass [ruff](https://github.com/astral-sh/ruff) style checks to be merged. It is recommended to install pre-commit hooks to ensure this locally before commiting code:
+
+```
+$ poetry run pre-commit install
+```
+
+Each public method, class and module should have docstrings. Docstrings are written in the Numpy style.
+
+### Testing
+
+To produce Coverage reports, run the following commands:
+
+```
+$ poetry run coverage run -m pytest
+$ poetry run coverage xml
+```
+
+## To Do:
+* Documentation ..
+* Metadata
+    - Choice
+    - Multichoice
+    - Money
+* Entity implementation
+    - Illegal file extensions
+    - Upload file
+    - Upload image
+    - Upload large file
+    - Add / remove relationships
+    - Add relationships (single/collection valued) as attr on entity
+    - Add columns as attr on entity
+* Add Tests:
+    - Add column
+    - Remove column
+    - Add alternate key
+    - Remove alternate key
+* Implement `CreateMultiple` request if creating more than 100 elements?
+    - https://learn.microsoft.com/en-us/power-apps/developer/data-platform/bulk-operations?tabs=webapi#createmultiple
+* Implement BulkDelete Action?
+    - https://learn.microsoft.com/en-us/power-apps/developer/data-platform/delete-data-bulk?tabs=sdk
+
+# Usage
+
+## DataverseClient
+
+### Initialize DataverseClient
+
+For now, I've coded the framework around the `requests` library, for good and bad! In the future, I will consider generalizing further, letting the user pass an authenticated requests handler of choice to the framework by specifying a `Protocol` to follow instead.
+
+To instantiate, pass a `requests.Session` together with a Dataverse environment URL to the `DataverseClient` constructor:
+
+```python
+session = Session()
+session.auth = auth
+environment_url = os.getenv("dataverse_url")
+
+client = DataverseClient(session=session, environment_url=environment_url)
+```
+
+### Create new Entity
+
+It is possible to create a new Entity using the `DataverseClient`. This requires a full `EntityMetadata` definition according to Dataverse standards. You can make this yourself and follow the `MetadataDumper` protocol, or use the provided `define_entity` function.
+
+The `define_label` function makes it simple to generate `Label` metadata with correct `LocalizedLabels` in its payload.
+
+In the example below, the optional `return_representation` argument has been set to `True` to receive the full Entity metadata definition as created by Dataverse as part of the server response. The response can be parsed by `EntityMetadata` classmethod to get a full fledged object for editing.
+
+```python
+from dataverse_api.metadata.attributes import StringAttributeMetadata
+from dataverse_api.metadata.entity import EntityMetadata, define_entity
+from dataverse_api.utils.labels import define_label
+
+new_entity = define_entity(
+    schema_name="new_name",
+    attributes=[StringAttributeMetadata(
+        schema_name="new_primary_col",
+        is_primary_name = True,
+        description=define_label("Primary column for Entity."),
+        display_name=define_label("Autonumber Column"),
+        auto_number_format="{SEQNUM:6}-#-{RANDSTRING:3}")],
+    description=define_label("Entity Created by Client"),
+    display_name=define_label("Programmatically Created Table")
+)
+
+resp = client.create_entity(new_entity, return_representation=True)
+entity_meta = EntityMetadata.model_validate_dataverse(resp.json())
+```
+
+### Update existing Entity
+
+You can update an existing Entity definition easily by retrieving the Entity metadata definition, and reupload an adjusted version.
+
+Below is a simple example. Note that this method also supports `return_representation` in the same manner as the `DataverseClient.create_entity()` method, if you want to return the edited Entity metadata as persisted in Dataverse.
+
+```python
+metadata = client.get_entity_definition("new_name")
+metadata.display_name.localized_labels[0].label = "Overridden Display Name"
+
+client.update_entity(metadata)
+```
+
+## DataverseEntity
+
+### Initialize interface with Entity
+
+To initializes an interface with a specific Dataverse Entity, use the `DataverseClient.entity()` method. It returns a `DataverseEntity` object that allows interaction with this specific entity.
+
+```python
+foo = client.entity(logical_name="foo")
+```
+As of now, only `LogicalName` is supported for instantiating a new `DataverseEntity` object.
+
+
+### Read
+
+The `DataverseEntity.read()` method has been furnished with the necessary arguments to do querying as specified in the [Microsoft Dataverse documentation](https://learn.microsoft.com/en-us/power-apps/developer/data-platform/webapi/query-data-web-api?view=dataverse-latest).
+
+A simple example:
+
+```python
+data = foo.read(select=["name","address"], filter="salary gt 10000", top=5, order_by="salary desc")
+```
+
+### Create
+
+To create rows, you can use a `pandas.DataFrame` or a simple construct like a list of dicts, where each dict contains the data for a single row.
+
+Below is an example of creating rows in the Entity by passing a dataframe and specifying that the creation method should be the `CreateMultiple` web API Action. The `return_created` argument can be set to `True` if you need the IDs as reference.
+
+```python
+foo.create(data=df, mode="multiple", return_created=True)
+```
+
+Note that the different modes provide different content when `return_created` is set to `True` - the script simply sets a `Prefer` header to include created data in the server response.
+
+For now the user may choose how to handle this based on the list of `requests.Response` objects that will be returned by the method.
+
+### Upsert
+
+Upserting data into Dataverse is simple. If you are just updating existing data you may have the URI (Primary Attribute ID) in your data. You can then omit the `alternate_key` argument.
+
+```python
+foo.upsert(data=df, alternate_key="my_key", mode="batch")
+```
+
+### Delete
+
+TBD
+
+### Add and remove Attributes
+
+TBD
+
+## Add and remove Alternate Keys
+
+TBD
```

### Comparing `dataverse_api-1.1.4/PKG-INFO` & `dataverse_api-1.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dataverse-api
-Version: 1.1.4
+Version: 1.1.5
 Summary: Abstraction layer for interacting with Microsoft Dataverse Web API using Python.
 Author: Marcus Risanger
 Author-email: 69350948+MarcusRisanger@users.noreply.github.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
@@ -225,49 +225,49 @@
 ## DataverseEntity
 
 ### Initialize interface with Entity
 
 To initializes an interface with a specific Dataverse Entity, use the `DataverseClient.entity()` method. It returns a `DataverseEntity` object that allows interaction with this specific entity.
 
 ```python
-entity = client.entity(logical_name="foo")
+foo = client.entity(logical_name="foo")
 ```
 As of now, only `LogicalName` is supported for instantiating a new `DataverseEntity` object.
 
 
 ### Read
 
 The `DataverseEntity.read()` method has been furnished with the necessary arguments to do querying as specified in the [Microsoft Dataverse documentation](https://learn.microsoft.com/en-us/power-apps/developer/data-platform/webapi/query-data-web-api?view=dataverse-latest).
 
 A simple example:
 
 ```python
-data = entity.read(select=["name","address"], filter="salary gt 10000", top=5, order_by="salary desc")
+data = foo.read(select=["name","address"], filter="salary gt 10000", top=5, order_by="salary desc")
 ```
 
 ### Create
 
 To create rows, you can use a `pandas.DataFrame` or a simple construct like a list of dicts, where each dict contains the data for a single row.
 
 Below is an example of creating rows in the Entity by passing a dataframe and specifying that the creation method should be the `CreateMultiple` web API Action. The `return_created` argument can be set to `True` if you need the IDs as reference.
 
 ```python
-entity.create(data=df, mode="multiple", return_created=True)
+foo.create(data=df, mode="multiple", return_created=True)
 ```
 
 Note that the different modes provide different content when `return_created` is set to `True` - the script simply sets a `Prefer` header to include created data in the server response.
 
 For now the user may choose how to handle this based on the list of `requests.Response` objects that will be returned by the method.
 
 ### Upsert
 
 Upserting data into Dataverse is simple. If you are just updating existing data you may have the URI (Primary Attribute ID) in your data. You can then omit the `alternate_key` argument.
 
 ```python
-entity.upsert(data=df, alternate_key="my_key", mode="batch")
+foo.upsert(data=df, alternate_key="my_key", mode="batch")
 ```
 
 ### Delete
 
 TBD
 
 ### Add and remove Attributes
```

