# Comparing `tmp/airbyte-0.8.4.tar.gz` & `tmp/airbyte-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airbyte-0.8.4.tar", max compression
+gzip compressed data, was "airbyte-0.9.0.tar", max compression
```

## Comparing `airbyte-0.8.4.tar` & `airbyte-0.9.0.tar`

### file list

```diff
@@ -1,56 +1,58 @@
--rw-r--r--   0        0        0     3804 2024-04-02 06:23:28.499375 airbyte-0.8.4/LICENSE.md
--rw-r--r--   0        0        0     6176 2024-04-02 06:23:28.499375 airbyte-0.8.4/README.md
--rw-r--r--   0        0        0     1154 2024-04-02 06:23:28.499375 airbyte-0.8.4/airbyte/__init__.py
--rw-r--r--   0        0        0     2262 2024-04-02 06:23:28.499375 airbyte-0.8.4/airbyte/_batch_handles.py
--rw-r--r--   0        0        0    16354 2024-04-02 06:23:28.499375 airbyte-0.8.4/airbyte/_executor.py
--rw-r--r--   0        0        0        0 2024-04-02 06:23:28.503375 airbyte-0.8.4/airbyte/_processors/__init__.py
--rw-r--r--   0        0        0     9095 2024-04-02 06:23:28.503375 airbyte-0.8.4/airbyte/_processors/base.py
--rw-r--r--   0        0        0      352 2024-04-02 06:23:28.503375 airbyte-0.8.4/airbyte/_processors/file/__init__.py
--rw-r--r--   0        0        0     7496 2024-04-02 06:23:28.503375 airbyte-0.8.4/airbyte/_processors/file/base.py
--rw-r--r--   0        0        0      928 2024-04-02 06:23:28.503375 airbyte-0.8.4/airbyte/_processors/file/jsonl.py
--rw-r--r--   0        0        0       79 2024-04-02 06:23:28.503375 airbyte-0.8.4/airbyte/_processors/sql/__init__.py
--rw-r--r--   0        0        0    32880 2024-04-02 06:23:28.503375 airbyte-0.8.4/airbyte/_processors/sql/base.py
--rw-r--r--   0        0        0     8568 2024-04-02 06:23:28.503375 airbyte-0.8.4/airbyte/_processors/sql/bigquery.py
--rw-r--r--   0        0        0     3949 2024-04-02 06:23:28.503375 airbyte-0.8.4/airbyte/_processors/sql/duckdb.py
--rw-r--r--   0        0        0     1235 2024-04-02 06:23:28.503375 airbyte-0.8.4/airbyte/_processors/sql/motherduck.py
--rw-r--r--   0        0        0      837 2024-04-02 06:23:28.503375 airbyte-0.8.4/airbyte/_processors/sql/postgres.py
--rw-r--r--   0        0        0     3762 2024-04-02 06:23:28.503375 airbyte-0.8.4/airbyte/_processors/sql/snowflake.py
--rw-r--r--   0        0        0      420 2024-04-02 06:23:28.503375 airbyte-0.8.4/airbyte/_util/__init__.py
--rw-r--r--   0        0        0     3855 2024-04-02 06:23:28.503375 airbyte-0.8.4/airbyte/_util/document_rendering.py
--rw-r--r--   0        0        0     1854 2024-04-02 06:23:28.503375 airbyte-0.8.4/airbyte/_util/google_secrets.py
--rw-r--r--   0        0        0     3355 2024-04-02 06:23:28.503375 airbyte-0.8.4/airbyte/_util/meta.py
--rw-r--r--   0        0        0     6988 2024-04-02 06:23:28.503375 airbyte-0.8.4/airbyte/_util/name_normalizers.py
--rw-r--r--   0        0        0     1683 2024-04-02 06:23:28.503375 airbyte-0.8.4/airbyte/_util/pip_util.py
--rw-r--r--   0        0        0    10605 2024-04-02 06:23:28.503375 airbyte-0.8.4/airbyte/_util/telemetry.py
--rw-r--r--   0        0        0      903 2024-04-02 06:23:28.503375 airbyte-0.8.4/airbyte/caches/__init__.py
--rw-r--r--   0        0        0    10139 2024-04-02 06:23:28.503375 airbyte-0.8.4/airbyte/caches/_catalog_manager.py
--rw-r--r--   0        0        0     3775 2024-04-02 06:23:28.503375 airbyte-0.8.4/airbyte/caches/base.py
--rw-r--r--   0        0        0     2124 2024-04-02 06:23:28.503375 airbyte-0.8.4/airbyte/caches/bigquery.py
--rw-r--r--   0        0        0     1947 2024-04-02 06:23:28.503375 airbyte-0.8.4/airbyte/caches/duckdb.py
--rw-r--r--   0        0        0      471 2024-04-02 06:23:28.503375 airbyte-0.8.4/airbyte/caches/generic.py
--rw-r--r--   0        0        0     1169 2024-04-02 06:23:28.503375 airbyte-0.8.4/airbyte/caches/motherduck.py
--rw-r--r--   0        0        0     1213 2024-04-02 06:23:28.503375 airbyte-0.8.4/airbyte/caches/postgres.py
--rw-r--r--   0        0        0     1627 2024-04-02 06:23:28.503375 airbyte-0.8.4/airbyte/caches/snowflake.py
--rw-r--r--   0        0        0     1998 2024-04-02 06:23:28.503375 airbyte-0.8.4/airbyte/caches/util.py
--rw-r--r--   0        0        0      346 2024-04-02 06:23:28.503375 airbyte-0.8.4/airbyte/datasets/__init__.py
--rw-r--r--   0        0        0     2212 2024-04-02 06:23:28.503375 airbyte-0.8.4/airbyte/datasets/_base.py
--rw-r--r--   0        0        0      917 2024-04-02 06:23:28.503375 airbyte-0.8.4/airbyte/datasets/_lazy.py
--rw-r--r--   0        0        0      819 2024-04-02 06:23:28.503375 airbyte-0.8.4/airbyte/datasets/_map.py
--rw-r--r--   0        0        0     5481 2024-04-02 06:23:28.503375 airbyte-0.8.4/airbyte/datasets/_sql.py
--rw-r--r--   0        0        0     1861 2024-04-02 06:23:28.503375 airbyte-0.8.4/airbyte/documents.py
--rw-r--r--   0        0        0     9245 2024-04-02 06:23:28.503375 airbyte-0.8.4/airbyte/exceptions.py
--rw-r--r--   0        0        0    13834 2024-04-02 06:23:28.503375 airbyte-0.8.4/airbyte/progress.py
--rw-r--r--   0        0        0        0 2024-04-02 06:23:28.503375 airbyte-0.8.4/airbyte/py.typed
--rw-r--r--   0        0        0     1580 2024-04-02 06:23:28.503375 airbyte-0.8.4/airbyte/results.py
--rw-r--r--   0        0        0     3519 2024-04-02 06:23:28.503375 airbyte-0.8.4/airbyte/secrets.py
--rw-r--r--   0        0        0      517 2024-04-02 06:23:28.503375 airbyte-0.8.4/airbyte/sources/__init__.py
--rw-r--r--   0        0        0    28443 2024-04-02 06:23:28.503375 airbyte-0.8.4/airbyte/sources/base.py
--rw-r--r--   0        0        0     3718 2024-04-02 06:23:28.503375 airbyte-0.8.4/airbyte/sources/registry.py
--rw-r--r--   0        0        0     5516 2024-04-02 06:23:28.503375 airbyte-0.8.4/airbyte/sources/util.py
--rw-r--r--   0        0        0      987 2024-04-02 06:23:28.503375 airbyte-0.8.4/airbyte/strategies.py
--rw-r--r--   0        0        0     4733 2024-04-02 06:23:28.503375 airbyte-0.8.4/airbyte/types.py
--rw-r--r--   0        0        0     5423 2024-04-02 06:23:28.503375 airbyte-0.8.4/airbyte/validate.py
--rw-r--r--   0        0        0      232 2024-04-02 06:23:28.503375 airbyte-0.8.4/airbyte/version.py
--rw-r--r--   0        0        0      369 2024-04-02 06:23:28.503375 airbyte-0.8.4/airbyte/warnings.py
--rw-r--r--   0        0        0     8366 2024-04-02 06:23:42.691383 airbyte-0.8.4/pyproject.toml
--rw-r--r--   0        0        0     7567 1970-01-01 00:00:00.000000 airbyte-0.8.4/PKG-INFO
+-rw-r--r--   0        0        0     3804 2024-04-03 23:10:43.349270 airbyte-0.9.0/LICENSE.md
+-rw-r--r--   0        0        0     6176 2024-04-03 23:10:43.349270 airbyte-0.9.0/README.md
+-rw-r--r--   0        0        0     1230 2024-04-03 23:10:43.349270 airbyte-0.9.0/airbyte/__init__.py
+-rw-r--r--   0        0        0     2262 2024-04-03 23:10:43.349270 airbyte-0.9.0/airbyte/_batch_handles.py
+-rw-r--r--   0        0        0    16354 2024-04-03 23:10:43.353270 airbyte-0.9.0/airbyte/_executor.py
+-rw-r--r--   0        0        0        0 2024-04-03 23:10:43.353270 airbyte-0.9.0/airbyte/_processors/__init__.py
+-rw-r--r--   0        0        0     9023 2024-04-03 23:10:43.353270 airbyte-0.9.0/airbyte/_processors/base.py
+-rw-r--r--   0        0        0      352 2024-04-03 23:10:43.353270 airbyte-0.9.0/airbyte/_processors/file/__init__.py
+-rw-r--r--   0        0        0     7543 2024-04-03 23:10:43.353270 airbyte-0.9.0/airbyte/_processors/file/base.py
+-rw-r--r--   0        0        0      913 2024-04-03 23:10:43.353270 airbyte-0.9.0/airbyte/_processors/file/jsonl.py
+-rw-r--r--   0        0        0       79 2024-04-03 23:10:43.353270 airbyte-0.9.0/airbyte/_processors/sql/__init__.py
+-rw-r--r--   0        0        0    34793 2024-04-03 23:10:43.353270 airbyte-0.9.0/airbyte/_processors/sql/base.py
+-rw-r--r--   0        0        0     8736 2024-04-03 23:10:43.353270 airbyte-0.9.0/airbyte/_processors/sql/bigquery.py
+-rw-r--r--   0        0        0     3867 2024-04-03 23:10:43.353270 airbyte-0.9.0/airbyte/_processors/sql/duckdb.py
+-rw-r--r--   0        0        0     1235 2024-04-03 23:10:43.353270 airbyte-0.9.0/airbyte/_processors/sql/motherduck.py
+-rw-r--r--   0        0        0      837 2024-04-03 23:10:43.353270 airbyte-0.9.0/airbyte/_processors/sql/postgres.py
+-rw-r--r--   0        0        0     3825 2024-04-03 23:10:43.353270 airbyte-0.9.0/airbyte/_processors/sql/snowflake.py
+-rw-r--r--   0        0        0      420 2024-04-03 23:10:43.353270 airbyte-0.9.0/airbyte/_util/__init__.py
+-rw-r--r--   0        0        0     3855 2024-04-03 23:10:43.353270 airbyte-0.9.0/airbyte/_util/document_rendering.py
+-rw-r--r--   0        0        0     1854 2024-04-03 23:10:43.353270 airbyte-0.9.0/airbyte/_util/google_secrets.py
+-rw-r--r--   0        0        0     3355 2024-04-03 23:10:43.353270 airbyte-0.9.0/airbyte/_util/meta.py
+-rw-r--r--   0        0        0     1596 2024-04-03 23:10:43.353270 airbyte-0.9.0/airbyte/_util/name_normalizers.py
+-rw-r--r--   0        0        0     1683 2024-04-03 23:10:43.353270 airbyte-0.9.0/airbyte/_util/pip_util.py
+-rw-r--r--   0        0        0    10603 2024-04-03 23:10:43.353270 airbyte-0.9.0/airbyte/_util/telemetry.py
+-rw-r--r--   0        0        0      903 2024-04-03 23:10:43.353270 airbyte-0.9.0/airbyte/caches/__init__.py
+-rw-r--r--   0        0        0    10139 2024-04-03 23:10:43.353270 airbyte-0.9.0/airbyte/caches/_catalog_manager.py
+-rw-r--r--   0        0        0     3775 2024-04-03 23:10:43.353270 airbyte-0.9.0/airbyte/caches/base.py
+-rw-r--r--   0        0        0     2124 2024-04-03 23:10:43.353270 airbyte-0.9.0/airbyte/caches/bigquery.py
+-rw-r--r--   0        0        0     1947 2024-04-03 23:10:43.353270 airbyte-0.9.0/airbyte/caches/duckdb.py
+-rw-r--r--   0        0        0      471 2024-04-03 23:10:43.353270 airbyte-0.9.0/airbyte/caches/generic.py
+-rw-r--r--   0        0        0     1169 2024-04-03 23:10:43.353270 airbyte-0.9.0/airbyte/caches/motherduck.py
+-rw-r--r--   0        0        0     1213 2024-04-03 23:10:43.353270 airbyte-0.9.0/airbyte/caches/postgres.py
+-rw-r--r--   0        0        0     1627 2024-04-03 23:10:43.353270 airbyte-0.9.0/airbyte/caches/snowflake.py
+-rw-r--r--   0        0        0     1998 2024-04-03 23:10:43.353270 airbyte-0.9.0/airbyte/caches/util.py
+-rw-r--r--   0        0        0     1341 2024-04-03 23:10:43.353270 airbyte-0.9.0/airbyte/constants.py
+-rw-r--r--   0        0        0      346 2024-04-03 23:10:43.353270 airbyte-0.9.0/airbyte/datasets/__init__.py
+-rw-r--r--   0        0        0     2212 2024-04-03 23:10:43.353270 airbyte-0.9.0/airbyte/datasets/_base.py
+-rw-r--r--   0        0        0      917 2024-04-03 23:10:43.353270 airbyte-0.9.0/airbyte/datasets/_lazy.py
+-rw-r--r--   0        0        0      819 2024-04-03 23:10:43.353270 airbyte-0.9.0/airbyte/datasets/_map.py
+-rw-r--r--   0        0        0     5481 2024-04-03 23:10:43.353270 airbyte-0.9.0/airbyte/datasets/_sql.py
+-rw-r--r--   0        0        0     1861 2024-04-03 23:10:43.353270 airbyte-0.9.0/airbyte/documents.py
+-rw-r--r--   0        0        0     9245 2024-04-03 23:10:43.353270 airbyte-0.9.0/airbyte/exceptions.py
+-rw-r--r--   0        0        0    13834 2024-04-03 23:10:43.353270 airbyte-0.9.0/airbyte/progress.py
+-rw-r--r--   0        0        0        0 2024-04-03 23:10:43.353270 airbyte-0.9.0/airbyte/py.typed
+-rw-r--r--   0        0        0     9044 2024-04-03 23:10:43.353270 airbyte-0.9.0/airbyte/records.py
+-rw-r--r--   0        0        0     1580 2024-04-03 23:10:43.353270 airbyte-0.9.0/airbyte/results.py
+-rw-r--r--   0        0        0     3519 2024-04-03 23:10:43.353270 airbyte-0.9.0/airbyte/secrets.py
+-rw-r--r--   0        0        0      517 2024-04-03 23:10:43.353270 airbyte-0.9.0/airbyte/sources/__init__.py
+-rw-r--r--   0        0        0    28448 2024-04-03 23:10:43.353270 airbyte-0.9.0/airbyte/sources/base.py
+-rw-r--r--   0        0        0     3718 2024-04-03 23:10:43.353270 airbyte-0.9.0/airbyte/sources/registry.py
+-rw-r--r--   0        0        0     5516 2024-04-03 23:10:43.353270 airbyte-0.9.0/airbyte/sources/util.py
+-rw-r--r--   0        0        0      987 2024-04-03 23:10:43.353270 airbyte-0.9.0/airbyte/strategies.py
+-rw-r--r--   0        0        0     5074 2024-04-03 23:10:43.353270 airbyte-0.9.0/airbyte/types.py
+-rw-r--r--   0        0        0     5423 2024-04-03 23:10:43.353270 airbyte-0.9.0/airbyte/validate.py
+-rw-r--r--   0        0        0      232 2024-04-03 23:10:43.353270 airbyte-0.9.0/airbyte/version.py
+-rw-r--r--   0        0        0      369 2024-04-03 23:10:43.353270 airbyte-0.9.0/airbyte/warnings.py
+-rw-r--r--   0        0        0     8366 2024-04-03 23:10:46.949279 airbyte-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0     7567 1970-01-01 00:00:00.000000 airbyte-0.9.0/PKG-INFO
```

### Comparing `airbyte-0.8.4/LICENSE.md` & `airbyte-0.9.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `airbyte-0.8.4/README.md` & `airbyte-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `airbyte-0.8.4/airbyte/__init__.py` & `airbyte-0.9.0/airbyte/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -8,28 +8,30 @@
 from __future__ import annotations
 
 from airbyte import caches, datasets, documents, exceptions, results, secrets, sources
 from airbyte.caches.bigquery import BigQueryCache
 from airbyte.caches.duckdb import DuckDBCache
 from airbyte.caches.util import get_default_cache, new_local_cache
 from airbyte.datasets import CachedDataset
+from airbyte.records import StreamRecord
 from airbyte.results import ReadResult
 from airbyte.secrets import SecretSource, get_secret
 from airbyte.sources import registry
 from airbyte.sources.base import Source
 from airbyte.sources.registry import get_available_connectors
 from airbyte.sources.util import get_source
 
 
 __all__ = [
     # Modules
     "caches",
     "datasets",
     "documents",
     "exceptions",
+    "records",
     "registry",
     "results",
     "secrets",
     "sources",
     # Factories
     "get_available_connectors",
     "get_default_cache",
@@ -39,10 +41,11 @@
     # Classes
     "BigQueryCache",
     "CachedDataset",
     "DuckDBCache",
     "ReadResult",
     "SecretSource",
     "Source",
+    "StreamRecord",
 ]
 
 __docformat__ = "google"
```

### Comparing `airbyte-0.8.4/airbyte/_batch_handles.py` & `airbyte-0.9.0/airbyte/_batch_handles.py`

 * *Files identical despite different names*

### Comparing `airbyte-0.8.4/airbyte/_executor.py` & `airbyte-0.9.0/airbyte/_executor.py`

 * *Files identical despite different names*

### Comparing `airbyte-0.8.4/airbyte/_processors/base.py` & `airbyte-0.9.0/airbyte/_processors/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,17 +34,14 @@
 if TYPE_CHECKING:
     from collections.abc import Iterable, Iterator
 
     from airbyte._batch_handles import BatchHandle
     from airbyte.caches._catalog_manager import CatalogManager
 
 
-DEBUG_MODE = False  # Set to True to enable additional debug logging.
-
-
 class AirbyteMessageParsingError(Exception):
     """Raised when an Airbyte message is invalid or cannot be parsed."""
 
 
 class RecordProcessor(abc.ABC):
     """Abstract base class for classes which can process Airbyte messages from a source.
```

### Comparing `airbyte-0.8.4/airbyte/_processors/file/base.py` & `airbyte-0.9.0/airbyte/_processors/file/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,16 +8,17 @@
 from pathlib import Path
 from typing import IO, TYPE_CHECKING, final
 
 import ulid
 
 from airbyte import exceptions as exc
 from airbyte._batch_handles import BatchHandle
-from airbyte._util.name_normalizers import LowerCaseNormalizer, StreamRecord
+from airbyte._util.name_normalizers import LowerCaseNormalizer
 from airbyte.progress import progress
+from airbyte.records import StreamRecord
 
 
 if TYPE_CHECKING:
     from airbyte_protocol.models import (
         AirbyteRecordMessage,
     )
 
@@ -160,16 +161,16 @@
             # Already at max batch size, so start a new batch.
             batch_handle = self._new_batch(stream_name=stream_name)
 
         if batch_handle.open_file_writer is None:
             raise exc.AirbyteLibInternalError(message="Expected open file writer.")
 
         self._write_record_dict(
-            record_dict=StreamRecord(
-                from_dict=record_msg.data,
+            record_dict=StreamRecord.from_record_message(
+                record_message=record_msg,
                 expected_keys=stream_schema["properties"].keys(),
                 normalizer=LowerCaseNormalizer,
                 prune_extra_fields=self.prune_extra_fields,
             ),
             open_file_writer=batch_handle.open_file_writer,
         )
         batch_handle.increment_record_count()
```

### Comparing `airbyte-0.8.4/airbyte/_processors/file/jsonl.py` & `airbyte-0.9.0/airbyte/_processors/file/jsonl.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     FileWriterBase,
 )
 
 
 if TYPE_CHECKING:
     from pathlib import Path
 
-    from airbyte._util.name_normalizers import StreamRecord
+    from airbyte.records import StreamRecord
 
 
 class JsonlWriter(FileWriterBase):
     """A Jsonl cache implementation."""
 
     default_cache_file_suffix = ".jsonl.gz"
     prune_extra_fields = True
```

### Comparing `airbyte-0.8.4/airbyte/_processors/sql/base.py` & `airbyte-0.9.0/airbyte/_processors/sql/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,43 +28,47 @@
 from sqlalchemy.pool import StaticPool
 from sqlalchemy.sql.elements import TextClause
 
 from airbyte import exceptions as exc
 from airbyte._processors.base import RecordProcessor
 from airbyte._util.name_normalizers import LowerCaseNormalizer
 from airbyte.caches._catalog_manager import CatalogManager
+from airbyte.constants import (
+    AB_EXTRACTED_AT_COLUMN,
+    AB_META_COLUMN,
+    AB_RAW_ID_COLUMN,
+    DEBUG_MODE,
+)
 from airbyte.datasets._sql import CachedDataset
 from airbyte.progress import progress
 from airbyte.strategies import WriteStrategy
 from airbyte.types import SQLTypeConverter
 
 
 if TYPE_CHECKING:
     from collections.abc import Generator
     from pathlib import Path
 
     from sqlalchemy.engine import Connection, Engine
     from sqlalchemy.engine.cursor import CursorResult
     from sqlalchemy.engine.reflection import Inspector
     from sqlalchemy.sql.base import Executable
+    from sqlalchemy.sql.type_api import TypeEngine
 
     from airbyte_protocol.models import (
         AirbyteRecordMessage,
         AirbyteStateMessage,
         ConfiguredAirbyteCatalog,
     )
 
     from airbyte._batch_handles import BatchHandle
     from airbyte._processors.file.base import FileWriterBase
     from airbyte.caches.base import CacheBase
 
 
-DEBUG_MODE = False  # Set to True to enable additional debug logging.
-
-
 class RecordDedupeMode(enum.Enum):
     APPEND = "append"
     REPLACE = "replace"
 
 
 class SQLRuntimeError(Exception):
     """Raised when an SQL operation fails."""
@@ -232,15 +236,15 @@
     def get_pandas_dataframe(
         self,
         stream_name: str,
     ) -> pd.DataFrame:
         """Return a Pandas data frame with the stream's data."""
         table_name = self.get_sql_table_name(stream_name)
         engine = self.get_sql_engine()
-        return pd.read_sql_table(table_name, engine)
+        return pd.read_sql_table(table_name, engine, schema=self.cache.schema_name)
 
     def process_record_message(
         self,
         record_msg: AirbyteRecordMessage,
         stream_schema: dict,
     ) -> None:
         """Write a record to the cache.
@@ -261,14 +265,25 @@
         """This is called automatically whenever a new connection is created.
 
         By default this is a no-op. Subclasses can use this to set connection settings, such as
         timezone, case-sensitivity settings, and other session-level variables.
         """
         pass
 
+    def _invalidate_table_cache(
+        self,
+        table_name: str,
+    ) -> None:
+        """Invalidate the the named table cache.
+
+        This should be called whenever the table schema is known to have changed.
+        """
+        if table_name in self._cached_table_definitions:
+            del self._cached_table_definitions[table_name]
+
     def _get_table_by_name(
         self,
         table_name: str,
         *,
         force_refresh: bool = False,
         shallow_okay: bool = False,
     ) -> sqlalchemy.Table:
@@ -281,15 +296,18 @@
         query. To ignore the cache and force a refresh, set 'force_refresh' to True.
         """
         if force_refresh and shallow_okay:
             raise exc.AirbyteLibInternalError(
                 message="Cannot force refresh and use shallow query at the same time."
             )
 
-        if force_refresh or table_name not in self._cached_table_definitions:
+        if force_refresh and table_name in self._cached_table_definitions:
+            self._invalidate_table_cache(table_name)
+
+        if table_name not in self._cached_table_definitions:
             if shallow_okay:
                 # Return a shallow instance, without column declarations. Do not cache
                 # the table definition in this case.
                 return sqlalchemy.Table(
                     table_name,
                     sqlalchemy.MetaData(schema=self.cache.schema_name),
                 )
@@ -482,17 +500,18 @@
         properties = self.get_stream_properties(stream_name)
         for property_name, json_schema_property_def in properties.items():
             clean_prop_name = self.normalizer.normalize(property_name)
             columns[clean_prop_name] = self.type_converter.to_sql_type(
                 json_schema_property_def,
             )
 
-        # TODO: Add the metadata columns (this breaks tests)
-        # columns["_airbyte_extracted_at"] = sqlalchemy.TIMESTAMP()
-        # columns["_airbyte_loaded_at"] = sqlalchemy.TIMESTAMP()
+        columns[AB_RAW_ID_COLUMN] = self.type_converter_class.get_string_type()
+        columns[AB_EXTRACTED_AT_COLUMN] = sqlalchemy.TIMESTAMP()
+        columns[AB_META_COLUMN] = self.type_converter_class.get_json_type()
+
         return columns
 
     @final
     def write_stream_data(
         self,
         stream_name: str,
         write_strategy: WriteStrategy,
@@ -632,44 +651,74 @@
         This is a generic implementation, which can be overridden by subclasses
         to improve performance.
         """
         temp_table_name = self._create_table_for_loading(stream_name, batch_id)
         for file_path in files:
             dataframe = pd.read_json(file_path, lines=True)
 
+            sql_column_definitions: dict[str, TypeEngine] = self._get_sql_column_definitions(
+                stream_name
+            )
+
             # Remove fields that are not in the schema
             for col_name in dataframe.columns:
-                if col_name not in self.get_stream_properties(stream_name):
-                    dataframe = dataframe.drop(columns=property)
+                if col_name not in sql_column_definitions:
+                    dataframe = dataframe.drop(columns=col_name)
 
             # Pandas will auto-create the table if it doesn't exist, which we don't want.
             if not self._table_exists(temp_table_name):
                 raise exc.AirbyteLibInternalError(
                     message="Table does not exist after creation.",
                     context={
                         "temp_table_name": temp_table_name,
                     },
                 )
 
             # Normalize all column names to lower case.
-            dataframe.columns = Index(
-                [LowerCaseNormalizer.normalize(col) for col in dataframe.columns]
-            )
+            dataframe.columns = Index([self.normalizer.normalize(col) for col in dataframe.columns])
 
             # Write the data to the table.
             dataframe.to_sql(
                 temp_table_name,
                 self.get_sql_alchemy_url(),
                 schema=self.cache.schema_name,
                 if_exists="append",
                 index=False,
-                dtype=self._get_sql_column_definitions(stream_name),
+                dtype=sql_column_definitions,
             )
         return temp_table_name
 
+    def _add_column_to_table(
+        self,
+        table: Table,
+        column_name: str,
+        column_type: sqlalchemy.types.TypeEngine,
+    ) -> None:
+        """Add a column to the given table."""
+        self._execute_sql(
+            text(
+                f"ALTER TABLE {self._fully_qualified(table.name)} "
+                f"ADD COLUMN {column_name} {column_type}"
+            ),
+        )
+
+    def _add_missing_columns_to_table(
+        self,
+        stream_name: str,
+        table_name: str,
+    ) -> None:
+        """Add missing columns to the table."""
+        columns = self._get_sql_column_definitions(stream_name)
+        table = self._get_table_by_name(table_name, force_refresh=True)
+        for column_name, column_type in columns.items():
+            if column_name not in table.columns:
+                self._add_column_to_table(table, column_name, column_type)
+
+        self._invalidate_table_cache(table_name)
+
     @final
     def _write_temp_table_to_final_table(
         self,
         stream_name: str,
         temp_table_name: str,
         final_table_name: str,
         write_strategy: WriteStrategy,
@@ -698,22 +747,30 @@
                 stream_name=stream_name,
                 temp_table_name=temp_table_name,
                 final_table_name=final_table_name,
             )
             return
 
         if write_strategy == WriteStrategy.APPEND:
+            self._add_missing_columns_to_table(
+                stream_name=stream_name,
+                table_name=final_table_name,
+            )
             self._append_temp_table_to_final_table(
                 stream_name=stream_name,
                 temp_table_name=temp_table_name,
                 final_table_name=final_table_name,
             )
             return
 
         if write_strategy == WriteStrategy.MERGE:
+            self._add_missing_columns_to_table(
+                stream_name=stream_name,
+                table_name=final_table_name,
+            )
             if not self.supports_merge_insert:
                 # Fallback to emulated merge if the database does not support merge natively.
                 self._emulated_merge_temp_table_to_final_table(
                     stream_name=stream_name,
                     temp_table_name=temp_table_name,
                     final_table_name=final_table_name,
                 )
```

### Comparing `airbyte-0.8.4/airbyte/_processors/sql/bigquery.py` & `airbyte-0.9.0/airbyte/_processors/sql/bigquery.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,28 +26,33 @@
     from airbyte.caches.base import CacheBase
     from airbyte.caches.bigquery import BigQueryCache
 
 
 class BigQueryTypeConverter(SQLTypeConverter):
     """A class to convert types for BigQuery."""
 
+    @classmethod
+    def get_string_type(cls) -> sqlalchemy.types.TypeEngine:
+        """Return the string type for BigQuery."""
+        return "String"
+
     @overrides
     def to_sql_type(
         self,
         json_schema_property_def: dict[str, str | dict | list],
     ) -> sqlalchemy.types.TypeEngine:
         """Convert a value to a SQL type.
 
         We first call the parent class method to get the type. Then if the type is VARCHAR or
         BIGINT, we replace it with respective BigQuery types.
         """
         sql_type = super().to_sql_type(json_schema_property_def)
         # to-do: replace hardcoded return types with some sort of snowflake Variant equivalent
         if isinstance(sql_type, sqlalchemy.types.VARCHAR):
-            return "String"
+            return self.get_string_type()
         if isinstance(sql_type, sqlalchemy.types.BIGINT):
             return "INT64"
 
         return sql_type.__class__.__name__
 
 
 class BigQuerySqlProcessor(SqlProcessorBase):
```

### Comparing `airbyte-0.8.4/airbyte/_processors/sql/duckdb.py` & `airbyte-0.9.0/airbyte/_processors/sql/duckdb.py`

 * *Files 2% similar despite different names*

```diff
@@ -80,15 +80,14 @@
         We use DuckDB native SQL functions to efficiently read the files and insert
         them into the table in a single operation.
         """
         temp_table_name = self._create_table_for_loading(
             stream_name=stream_name,
             batch_id=batch_id,
         )
-        properties_list = list(self.get_stream_properties(stream_name).keys())
         columns_list = list(self._get_sql_column_definitions(stream_name=stream_name).keys())
         columns_list_str = indent(
             "\n, ".join([self._quote_identifier(col) for col in columns_list]),
             "    ",
         )
         files_list = ", ".join([f"'{f!s}'" for f in files])
         columns_type_map = indent(
@@ -97,15 +96,15 @@
                     self._quote_identifier(self.normalizer.normalize(prop_name))
                     + ": "
                     + str(
                         self._get_sql_column_definitions(stream_name)[
                             self.normalizer.normalize(prop_name)
                         ]
                     )
-                    for prop_name in properties_list
+                    for prop_name in columns_list
                 ]
             ),
             "    ",
         )
         insert_statement = dedent(
             f"""
             INSERT INTO {self.cache.schema_name}.{temp_table_name}
```

### Comparing `airbyte-0.8.4/airbyte/_processors/sql/motherduck.py` & `airbyte-0.9.0/airbyte/_processors/sql/motherduck.py`

 * *Files identical despite different names*

### Comparing `airbyte-0.8.4/airbyte/_processors/sql/postgres.py` & `airbyte-0.9.0/airbyte/_processors/sql/postgres.py`

 * *Files identical despite different names*

### Comparing `airbyte-0.8.4/airbyte/_processors/sql/snowflake.py` & `airbyte-0.9.0/airbyte/_processors/sql/snowflake.py`

 * *Files 6% similar despite different names*

```diff
@@ -36,14 +36,19 @@
         """
         sql_type = super().to_sql_type(json_schema_property_def)
         if isinstance(sql_type, sqlalchemy.types.JSON):
             return VARIANT()
 
         return sql_type
 
+    @staticmethod
+    def get_json_type() -> sqlalchemy.types.TypeEngine:
+        """Get the type to use for nested JSON data."""
+        return VARIANT()
+
 
 class SnowflakeSqlProcessor(SqlProcessorBase):
     """A Snowflake implementation of the cache."""
 
     file_writer_class = JsonlWriter
     type_converter_class = SnowflakeTypeConverter
 
@@ -64,23 +69,22 @@
         def path_str(path: Path) -> str:
             return str(path.absolute()).replace("\\", "\\\\")
 
         put_files_statements = "\n".join(
             [f"PUT 'file://{path_str(file_path)}' {internal_sf_stage_name};" for file_path in files]
         )
         self._execute_sql(put_files_statements)
-        properties_list: list[str] = list(self.get_stream_properties(stream_name).keys())
         columns_list = [
             self._quote_identifier(c)
             for c in list(self._get_sql_column_definitions(stream_name).keys())
         ]
         files_list = ", ".join([f"'{f.name}'" for f in files])
         columns_list_str: str = indent("\n, ".join(columns_list), " " * 12)
         variant_cols_str: str = ("\n" + " " * 21 + ", ").join(
-            [f"$1:{self.normalizer.normalize(col)}" for col in properties_list]
+            [f"$1:{self.normalizer.normalize(col)}" for col in columns_list]
         )
         copy_statement = dedent(
             f"""
             COPY INTO {temp_table_name}
             (
                 {columns_list_str}
             )
```

### Comparing `airbyte-0.8.4/airbyte/_util/document_rendering.py` & `airbyte-0.9.0/airbyte/_util/document_rendering.py`

 * *Files identical despite different names*

### Comparing `airbyte-0.8.4/airbyte/_util/google_secrets.py` & `airbyte-0.9.0/airbyte/_util/google_secrets.py`

 * *Files identical despite different names*

### Comparing `airbyte-0.8.4/airbyte/_util/meta.py` & `airbyte-0.9.0/airbyte/_util/meta.py`

 * *Files identical despite different names*

### Comparing `airbyte-0.8.4/airbyte/_util/pip_util.py` & `airbyte-0.9.0/airbyte/_util/pip_util.py`

 * *Files identical despite different names*

### Comparing `airbyte-0.8.4/airbyte/_util/telemetry.py` & `airbyte-0.9.0/airbyte/_util/telemetry.py`

 * *Files 1% similar despite different names*

```diff
@@ -132,15 +132,15 @@
             )
 
     # File is missing, incomplete, or stale. Create a new one.
     anonymous_user_id = anonymous_user_id or str(ulid.ULID())
     try:
         _ANALYTICS_FILE.parent.mkdir(exist_ok=True, parents=True)
         _ANALYTICS_FILE.write_text(
-            "# This file is used by PyAirbyte to track anonymous usage statistics.\n"
+            "# This file is used by Airbyte to track anonymous usage statistics.\n"
             "# For more information or to opt out, please see\n"
             "# - https://docs.airbyte.com/operator-guides/telemetry\n"
             f"anonymous_user_id: {anonymous_user_id}\n"
         )
     except Exception:
         # Failed to create the analytics file. Likely due to a read-only filesystem.
         issues.append("Failed to write the analytics file. Check filesystem permissions.")
```

### Comparing `airbyte-0.8.4/airbyte/caches/__init__.py` & `airbyte-0.9.0/airbyte/caches/__init__.py`

 * *Files identical despite different names*

### Comparing `airbyte-0.8.4/airbyte/caches/_catalog_manager.py` & `airbyte-0.9.0/airbyte/caches/_catalog_manager.py`

 * *Files identical despite different names*

### Comparing `airbyte-0.8.4/airbyte/caches/base.py` & `airbyte-0.9.0/airbyte/caches/base.py`

 * *Files identical despite different names*

### Comparing `airbyte-0.8.4/airbyte/caches/bigquery.py` & `airbyte-0.9.0/airbyte/caches/bigquery.py`

 * *Files identical despite different names*

### Comparing `airbyte-0.8.4/airbyte/caches/duckdb.py` & `airbyte-0.9.0/airbyte/caches/duckdb.py`

 * *Files identical despite different names*

### Comparing `airbyte-0.8.4/airbyte/caches/motherduck.py` & `airbyte-0.9.0/airbyte/caches/motherduck.py`

 * *Files identical despite different names*

### Comparing `airbyte-0.8.4/airbyte/caches/postgres.py` & `airbyte-0.9.0/airbyte/caches/postgres.py`

 * *Files identical despite different names*

### Comparing `airbyte-0.8.4/airbyte/caches/snowflake.py` & `airbyte-0.9.0/airbyte/caches/snowflake.py`

 * *Files identical despite different names*

### Comparing `airbyte-0.8.4/airbyte/caches/util.py` & `airbyte-0.9.0/airbyte/caches/util.py`

 * *Files identical despite different names*

### Comparing `airbyte-0.8.4/airbyte/datasets/_base.py` & `airbyte-0.9.0/airbyte/datasets/_base.py`

 * *Files identical despite different names*

### Comparing `airbyte-0.8.4/airbyte/datasets/_lazy.py` & `airbyte-0.9.0/airbyte/datasets/_lazy.py`

 * *Files identical despite different names*

### Comparing `airbyte-0.8.4/airbyte/datasets/_map.py` & `airbyte-0.9.0/airbyte/datasets/_map.py`

 * *Files identical despite different names*

### Comparing `airbyte-0.8.4/airbyte/datasets/_sql.py` & `airbyte-0.9.0/airbyte/datasets/_sql.py`

 * *Files identical despite different names*

### Comparing `airbyte-0.8.4/airbyte/documents.py` & `airbyte-0.9.0/airbyte/documents.py`

 * *Files identical despite different names*

### Comparing `airbyte-0.8.4/airbyte/exceptions.py` & `airbyte-0.9.0/airbyte/exceptions.py`

 * *Files identical despite different names*

### Comparing `airbyte-0.8.4/airbyte/progress.py` & `airbyte-0.9.0/airbyte/progress.py`

 * *Files identical despite different names*

### Comparing `airbyte-0.8.4/airbyte/results.py` & `airbyte-0.9.0/airbyte/results.py`

 * *Files identical despite different names*

### Comparing `airbyte-0.8.4/airbyte/secrets.py` & `airbyte-0.9.0/airbyte/secrets.py`

 * *Files identical despite different names*

### Comparing `airbyte-0.8.4/airbyte/sources/__init__.py` & `airbyte-0.9.0/airbyte/sources/__init__.py`

 * *Files identical despite different names*

### Comparing `airbyte-0.8.4/airbyte/sources/base.py` & `airbyte-0.9.0/airbyte/sources/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,25 +26,25 @@
     Status,
     SyncMode,
     TraceType,
     Type,
 )
 
 from airbyte import exceptions as exc
-from airbyte._util.name_normalizers import StreamRecord
 from airbyte._util.telemetry import (
     EventState,
     EventType,
     log_config_validation_result,
     log_source_check_result,
     send_telemetry,
 )
 from airbyte.caches.util import get_default_cache
 from airbyte.datasets._lazy import LazyDataset
 from airbyte.progress import progress
+from airbyte.records import StreamRecord
 from airbyte.results import ReadResult
 from airbyte.strategies import WriteStrategy
 from airbyte.warnings import PyAirbyteDataLossWarning
 
 
 if TYPE_CHECKING:
     from collections.abc import Generator, Iterable, Iterator
@@ -433,16 +433,16 @@
         def _with_logging(records: Iterable[dict[str, Any]]) -> Iterator[dict[str, Any]]:
             self._log_sync_start(cache=None)
             yield from records
             self._log_sync_success(cache=None)
 
         iterator: Iterator[dict[str, Any]] = _with_logging(
             records=(  # Generator comprehension yields StreamRecord objects for each record
-                StreamRecord(
-                    from_dict=record.record.data,
+                StreamRecord.from_record_message(
+                    record_message=record.record,
                     expected_keys=all_properties,
                     prune_extra_fields=True,
                 )
                 for record in self._read_with_catalog(configured_catalog)
                 if record.record
             )
         )
```

### Comparing `airbyte-0.8.4/airbyte/sources/registry.py` & `airbyte-0.9.0/airbyte/sources/registry.py`

 * *Files identical despite different names*

### Comparing `airbyte-0.8.4/airbyte/sources/util.py` & `airbyte-0.9.0/airbyte/sources/util.py`

 * *Files identical despite different names*

### Comparing `airbyte-0.8.4/airbyte/strategies.py` & `airbyte-0.9.0/airbyte/strategies.py`

 * *Files identical despite different names*

### Comparing `airbyte-0.8.4/airbyte/types.py` & `airbyte-0.9.0/airbyte/types.py`

 * *Files 6% similar despite different names*

```diff
@@ -90,19 +90,29 @@
 
     def __init__(
         self,
         conversion_map: dict | None = None,
     ) -> None:
         self.conversion_map = conversion_map or CONVERSION_MAP
 
-    @staticmethod
-    def get_failover_type() -> sqlalchemy.types.TypeEngine:
-        """Get the 'last resort' type to use if no other type is found."""
+    @classmethod
+    def get_string_type(cls) -> sqlalchemy.types.TypeEngine:
+        """Get the type to use for string data."""
         return sqlalchemy.types.VARCHAR()
 
+    @classmethod
+    def get_failover_type(cls) -> sqlalchemy.types.TypeEngine:
+        """Get the 'last resort' type to use if no other type is found."""
+        return cls.get_string_type()
+
+    @classmethod
+    def get_json_type(cls) -> sqlalchemy.types.TypeEngine:
+        """Get the type to use for nested JSON data."""
+        return sqlalchemy.types.JSON()
+
     def to_sql_type(
         self,
         json_schema_property_def: dict[str, str | dict | list],
     ) -> sqlalchemy.types.TypeEngine:
         """Convert a value to a SQL type."""
         try:
             airbyte_type, _ = _get_airbyte_type(json_schema_property_def)
```

### Comparing `airbyte-0.8.4/airbyte/validate.py` & `airbyte-0.9.0/airbyte/validate.py`

 * *Files identical despite different names*

### Comparing `airbyte-0.8.4/pyproject.toml` & `airbyte-0.9.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 description = "PyAirbyte"
 authors = ["Airbyte <contact@airbyte.io>"]
 readme = "README.md"
 packages = [{include = "airbyte"}]
 
 # This project uses dynamic versioning
 # https://github.com/mtkennerly/poetry-dynamic-versioning
-version = "0.8.4"
+version = "0.9.0"
 
 [tool.poetry-dynamic-versioning]
 enable = false
 
 [tool.poetry.dependencies]
 python = ">=3.9,<4.0"
```

### Comparing `airbyte-0.8.4/PKG-INFO` & `airbyte-0.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airbyte
-Version: 0.8.4
+Version: 0.9.0
 Summary: PyAirbyte
 Author: Airbyte
 Author-email: contact@airbyte.io
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

