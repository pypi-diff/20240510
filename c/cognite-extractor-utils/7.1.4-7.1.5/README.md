# Comparing `tmp/cognite_extractor_utils-7.1.4.tar.gz` & `tmp/cognite_extractor_utils-7.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cognite_extractor_utils-7.1.4.tar", max compression
+gzip compressed data, was "cognite_extractor_utils-7.1.5.tar", max compression
```

## Comparing `cognite_extractor_utils-7.1.4.tar` & `cognite_extractor_utils-7.1.5.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0    10173 2024-05-08 06:27:50.724296 cognite_extractor_utils-7.1.4/LICENSE
--rw-r--r--   0        0        0     4090 2024-05-08 06:27:50.724296 cognite_extractor_utils-7.1.4/README.md
--rw-r--r--   0        0        0      739 2024-05-08 06:27:50.724296 cognite_extractor_utils-7.1.4/cognite/extractorutils/__init__.py
--rw-r--r--   0        0        0     1558 2024-05-08 06:27:50.724296 cognite_extractor_utils-7.1.4/cognite/extractorutils/_inner_util.py
--rw-r--r--   0        0        0    16391 2024-05-08 06:27:50.724296 cognite_extractor_utils-7.1.4/cognite/extractorutils/base.py
--rw-r--r--   0        0        0     3059 2024-05-08 06:27:50.724296 cognite_extractor_utils-7.1.4/cognite/extractorutils/configtools/__init__.py
--rw-r--r--   0        0        0     4739 2024-05-08 06:27:50.724296 cognite_extractor_utils-7.1.4/cognite/extractorutils/configtools/_util.py
--rw-r--r--   0        0        0    21564 2024-05-08 06:27:50.724296 cognite_extractor_utils-7.1.4/cognite/extractorutils/configtools/elements.py
--rw-r--r--   0        0        0    16317 2024-05-08 06:27:50.724296 cognite_extractor_utils-7.1.4/cognite/extractorutils/configtools/loaders.py
--rw-r--r--   0        0        0     1084 2024-05-08 06:27:50.724296 cognite_extractor_utils-7.1.4/cognite/extractorutils/exceptions.py
--rw-r--r--   0        0        0    15509 2024-05-08 06:27:50.724296 cognite_extractor_utils-7.1.4/cognite/extractorutils/metrics.py
--rw-r--r--   0        0        0        0 2024-05-08 06:27:50.724296 cognite_extractor_utils-7.1.4/cognite/extractorutils/py.typed
--rw-r--r--   0        0        0    18667 2024-05-08 06:27:50.724296 cognite_extractor_utils-7.1.4/cognite/extractorutils/statestore.py
--rw-r--r--   0        0        0     3605 2024-05-08 06:27:50.724296 cognite_extractor_utils-7.1.4/cognite/extractorutils/threading.py
--rw-r--r--   0        0        0     3110 2024-05-08 06:27:50.724296 cognite_extractor_utils-7.1.4/cognite/extractorutils/uploader/__init__.py
--rw-r--r--   0        0        0     5304 2024-05-08 06:27:50.728296 cognite_extractor_utils-7.1.4/cognite/extractorutils/uploader/_base.py
--rw-r--r--   0        0        0     3247 2024-05-08 06:27:50.728296 cognite_extractor_utils-7.1.4/cognite/extractorutils/uploader/_metrics.py
--rw-r--r--   0        0        0     5628 2024-05-08 06:27:50.728296 cognite_extractor_utils-7.1.4/cognite/extractorutils/uploader/assets.py
--rw-r--r--   0        0        0     5680 2024-05-08 06:27:50.728296 cognite_extractor_utils-7.1.4/cognite/extractorutils/uploader/events.py
--rw-r--r--   0        0        0    18417 2024-05-08 06:27:50.728296 cognite_extractor_utils-7.1.4/cognite/extractorutils/uploader/files.py
--rw-r--r--   0        0        0     6738 2024-05-08 06:27:50.728296 cognite_extractor_utils-7.1.4/cognite/extractorutils/uploader/raw.py
--rw-r--r--   0        0        0    26817 2024-05-08 06:27:50.728296 cognite_extractor_utils-7.1.4/cognite/extractorutils/uploader/time_series.py
--rw-r--r--   0        0        0     7732 2024-05-08 06:27:50.728296 cognite_extractor_utils-7.1.4/cognite/extractorutils/uploader_extractor.py
--rw-r--r--   0        0        0     1020 2024-05-08 06:27:50.728296 cognite_extractor_utils-7.1.4/cognite/extractorutils/uploader_types.py
--rw-r--r--   0        0        0    17198 2024-05-08 06:27:50.728296 cognite_extractor_utils-7.1.4/cognite/extractorutils/util.py
--rw-r--r--   0        0        0     2088 2024-05-08 06:27:50.728296 cognite_extractor_utils-7.1.4/pyproject.toml
--rw-r--r--   0        0        0     5446 1970-01-01 00:00:00.000000 cognite_extractor_utils-7.1.4/PKG-INFO
+-rw-r--r--   0        0        0    10173 2024-05-10 08:27:23.972598 cognite_extractor_utils-7.1.5/LICENSE
+-rw-r--r--   0        0        0     4090 2024-05-10 08:27:23.972598 cognite_extractor_utils-7.1.5/README.md
+-rw-r--r--   0        0        0      739 2024-05-10 08:27:23.972598 cognite_extractor_utils-7.1.5/cognite/extractorutils/__init__.py
+-rw-r--r--   0        0        0     1558 2024-05-10 08:27:23.972598 cognite_extractor_utils-7.1.5/cognite/extractorutils/_inner_util.py
+-rw-r--r--   0        0        0    16391 2024-05-10 08:27:23.972598 cognite_extractor_utils-7.1.5/cognite/extractorutils/base.py
+-rw-r--r--   0        0        0     3059 2024-05-10 08:27:23.972598 cognite_extractor_utils-7.1.5/cognite/extractorutils/configtools/__init__.py
+-rw-r--r--   0        0        0     4739 2024-05-10 08:27:23.972598 cognite_extractor_utils-7.1.5/cognite/extractorutils/configtools/_util.py
+-rw-r--r--   0        0        0    21564 2024-05-10 08:27:23.972598 cognite_extractor_utils-7.1.5/cognite/extractorutils/configtools/elements.py
+-rw-r--r--   0        0        0    16317 2024-05-10 08:27:23.972598 cognite_extractor_utils-7.1.5/cognite/extractorutils/configtools/loaders.py
+-rw-r--r--   0        0        0     1084 2024-05-10 08:27:23.972598 cognite_extractor_utils-7.1.5/cognite/extractorutils/exceptions.py
+-rw-r--r--   0        0        0    15509 2024-05-10 08:27:23.972598 cognite_extractor_utils-7.1.5/cognite/extractorutils/metrics.py
+-rw-r--r--   0        0        0        0 2024-05-10 08:27:23.972598 cognite_extractor_utils-7.1.5/cognite/extractorutils/py.typed
+-rw-r--r--   0        0        0    18667 2024-05-10 08:27:23.972598 cognite_extractor_utils-7.1.5/cognite/extractorutils/statestore.py
+-rw-r--r--   0        0        0     3605 2024-05-10 08:27:23.972598 cognite_extractor_utils-7.1.5/cognite/extractorutils/threading.py
+-rw-r--r--   0        0        0     3110 2024-05-10 08:27:23.972598 cognite_extractor_utils-7.1.5/cognite/extractorutils/uploader/__init__.py
+-rw-r--r--   0        0        0     5304 2024-05-10 08:27:23.972598 cognite_extractor_utils-7.1.5/cognite/extractorutils/uploader/_base.py
+-rw-r--r--   0        0        0     3247 2024-05-10 08:27:23.972598 cognite_extractor_utils-7.1.5/cognite/extractorutils/uploader/_metrics.py
+-rw-r--r--   0        0        0     5628 2024-05-10 08:27:23.972598 cognite_extractor_utils-7.1.5/cognite/extractorutils/uploader/assets.py
+-rw-r--r--   0        0        0     5680 2024-05-10 08:27:23.972598 cognite_extractor_utils-7.1.5/cognite/extractorutils/uploader/events.py
+-rw-r--r--   0        0        0    18329 2024-05-10 08:27:23.972598 cognite_extractor_utils-7.1.5/cognite/extractorutils/uploader/files.py
+-rw-r--r--   0        0        0     6738 2024-05-10 08:27:23.972598 cognite_extractor_utils-7.1.5/cognite/extractorutils/uploader/raw.py
+-rw-r--r--   0        0        0    26817 2024-05-10 08:27:23.972598 cognite_extractor_utils-7.1.5/cognite/extractorutils/uploader/time_series.py
+-rw-r--r--   0        0        0     7732 2024-05-10 08:27:23.972598 cognite_extractor_utils-7.1.5/cognite/extractorutils/uploader_extractor.py
+-rw-r--r--   0        0        0     1020 2024-05-10 08:27:23.972598 cognite_extractor_utils-7.1.5/cognite/extractorutils/uploader_types.py
+-rw-r--r--   0        0        0    17198 2024-05-10 08:27:23.976598 cognite_extractor_utils-7.1.5/cognite/extractorutils/util.py
+-rw-r--r--   0        0        0     2088 2024-05-10 08:27:23.976598 cognite_extractor_utils-7.1.5/pyproject.toml
+-rw-r--r--   0        0        0     5446 1970-01-01 00:00:00.000000 cognite_extractor_utils-7.1.5/PKG-INFO
```

### Comparing `cognite_extractor_utils-7.1.4/LICENSE` & `cognite_extractor_utils-7.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `cognite_extractor_utils-7.1.4/README.md` & `cognite_extractor_utils-7.1.5/README.md`

 * *Files identical despite different names*

### Comparing `cognite_extractor_utils-7.1.4/cognite/extractorutils/__init__.py` & `cognite_extractor_utils-7.1.5/cognite/extractorutils/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -12,9 +12,9 @@
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
 """
 Cognite extractor utils is a Python package that simplifies the development of new extractors.
 """
 
-__version__ = "7.1.4"
+__version__ = "7.1.5"
 from .base import Extractor
```

### Comparing `cognite_extractor_utils-7.1.4/cognite/extractorutils/_inner_util.py` & `cognite_extractor_utils-7.1.5/cognite/extractorutils/_inner_util.py`

 * *Files identical despite different names*

### Comparing `cognite_extractor_utils-7.1.4/cognite/extractorutils/base.py` & `cognite_extractor_utils-7.1.5/cognite/extractorutils/base.py`

 * *Files identical despite different names*

### Comparing `cognite_extractor_utils-7.1.4/cognite/extractorutils/configtools/__init__.py` & `cognite_extractor_utils-7.1.5/cognite/extractorutils/configtools/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_extractor_utils-7.1.4/cognite/extractorutils/configtools/_util.py` & `cognite_extractor_utils-7.1.5/cognite/extractorutils/configtools/_util.py`

 * *Files identical despite different names*

### Comparing `cognite_extractor_utils-7.1.4/cognite/extractorutils/configtools/elements.py` & `cognite_extractor_utils-7.1.5/cognite/extractorutils/configtools/elements.py`

 * *Files identical despite different names*

### Comparing `cognite_extractor_utils-7.1.4/cognite/extractorutils/configtools/loaders.py` & `cognite_extractor_utils-7.1.5/cognite/extractorutils/configtools/loaders.py`

 * *Files identical despite different names*

### Comparing `cognite_extractor_utils-7.1.4/cognite/extractorutils/exceptions.py` & `cognite_extractor_utils-7.1.5/cognite/extractorutils/exceptions.py`

 * *Files identical despite different names*

### Comparing `cognite_extractor_utils-7.1.4/cognite/extractorutils/metrics.py` & `cognite_extractor_utils-7.1.5/cognite/extractorutils/metrics.py`

 * *Files identical despite different names*

### Comparing `cognite_extractor_utils-7.1.4/cognite/extractorutils/statestore.py` & `cognite_extractor_utils-7.1.5/cognite/extractorutils/statestore.py`

 * *Files identical despite different names*

### Comparing `cognite_extractor_utils-7.1.4/cognite/extractorutils/threading.py` & `cognite_extractor_utils-7.1.5/cognite/extractorutils/threading.py`

 * *Files identical despite different names*

### Comparing `cognite_extractor_utils-7.1.4/cognite/extractorutils/uploader/__init__.py` & `cognite_extractor_utils-7.1.5/cognite/extractorutils/uploader/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_extractor_utils-7.1.4/cognite/extractorutils/uploader/_base.py` & `cognite_extractor_utils-7.1.5/cognite/extractorutils/uploader/_base.py`

 * *Files identical despite different names*

### Comparing `cognite_extractor_utils-7.1.4/cognite/extractorutils/uploader/_metrics.py` & `cognite_extractor_utils-7.1.5/cognite/extractorutils/uploader/_metrics.py`

 * *Files identical despite different names*

### Comparing `cognite_extractor_utils-7.1.4/cognite/extractorutils/uploader/assets.py` & `cognite_extractor_utils-7.1.5/cognite/extractorutils/uploader/assets.py`

 * *Files identical despite different names*

### Comparing `cognite_extractor_utils-7.1.4/cognite/extractorutils/uploader/events.py` & `cognite_extractor_utils-7.1.5/cognite/extractorutils/uploader/events.py`

 * *Files identical despite different names*

### Comparing `cognite_extractor_utils-7.1.4/cognite/extractorutils/uploader/files.py` & `cognite_extractor_utils-7.1.5/cognite/extractorutils/uploader/files.py`

 * *Files 2% similar despite different names*

```diff
@@ -247,78 +247,80 @@
             exceptions=retries,
             cancellation_token=self.cancellation_token,
             tries=RETRIES,
             delay=RETRY_DELAY,
             max_delay=RETRY_MAX_DELAY,
             backoff=RETRY_BACKOFF_FACTOR,
         )
-        def _upload_single(read_file: Callable[[], BinaryIO], file_meta: FileMetadata) -> None:
+        def upload_file(read_file: Callable[[], BinaryIO], file_meta: FileMetadata) -> None:
+            with read_file() as file:
+                size = super_len(file)
+                if size == 0:
+                    # upload just the file metadata witout data
+                    file_meta, _url = self.cdf_client.files.create(
+                        file_metadata=file_meta, overwrite=self.overwrite_existing
+                    )
+                elif size >= self.max_single_chunk_file_size:
+                    # The minimum chunk size is 4000MiB.
+                    chunks = ChunkedStream(file, self.max_file_chunk_size, size)
+                    self.logger.debug(
+                        f"File {file_meta.external_id} is larger than 5GiB ({size})"
+                        f", uploading in {chunks.chunk_count} chunks"
+                    )
+                    with self.cdf_client.files.multipart_upload_session(
+                        file_meta.name if file_meta.name is not None else "",
+                        parts=chunks.chunk_count,
+                        overwrite=self.overwrite_existing,
+                        external_id=file_meta.external_id,
+                        source=file_meta.source,
+                        mime_type=file_meta.mime_type,
+                        metadata=file_meta.metadata,
+                        directory=file_meta.directory,
+                        asset_ids=file_meta.asset_ids,
+                        data_set_id=file_meta.data_set_id,
+                        labels=file_meta.labels,
+                        geo_location=file_meta.geo_location,
+                        source_created_time=file_meta.source_created_time,
+                        source_modified_time=file_meta.source_modified_time,
+                        security_categories=file_meta.security_categories,
+                    ) as session:
+                        while chunks.next_chunk():
+                            session.upload_part(chunks.current_chunk, chunks)
+                        file_meta = session.file_metadata
+                else:
+                    file_meta = self.cdf_client.files.upload_bytes(
+                        file,
+                        file_meta.name if file_meta.name is not None else "",
+                        overwrite=self.overwrite_existing,
+                        external_id=file_meta.external_id,
+                        source=file_meta.source,
+                        mime_type=file_meta.mime_type,
+                        metadata=file_meta.metadata,
+                        directory=file_meta.directory,
+                        asset_ids=file_meta.asset_ids,
+                        data_set_id=file_meta.data_set_id,
+                        labels=file_meta.labels,
+                        geo_location=file_meta.geo_location,
+                        source_created_time=file_meta.source_created_time,
+                        source_modified_time=file_meta.source_modified_time,
+                        security_categories=file_meta.security_categories,
+                    )
+
+            if self.post_upload_function:
+                try:
+                    self.post_upload_function([file_meta])
+                except Exception as e:
+                    self.logger.error("Error in upload callback: %s", str(e))
+
+        def wrapped_upload(read_file: Callable[[], BinaryIO], file_meta: FileMetadata) -> None:
             try:
-                # Upload file
-                with read_file() as file:
-                    size = super_len(file)
-                    if size == 0:
-                        # upload just the file metadata witout data
-                        file_meta, _url = self.cdf_client.files.create(
-                            file_metadata=file_meta, overwrite=self.overwrite_existing
-                        )
-                    elif size >= self.max_single_chunk_file_size:
-                        # The minimum chunk size is 4000MiB.
-                        chunks = ChunkedStream(file, self.max_file_chunk_size, size)
-                        self.logger.debug(
-                            f"File {file_meta.external_id} is larger than 5GiB ({size})"
-                            f", uploading in {chunks.chunk_count} chunks"
-                        )
-                        with self.cdf_client.files.multipart_upload_session(
-                            file_meta.name if file_meta.name is not None else "",
-                            parts=chunks.chunk_count,
-                            overwrite=self.overwrite_existing,
-                            external_id=file_meta.external_id,
-                            source=file_meta.source,
-                            mime_type=file_meta.mime_type,
-                            metadata=file_meta.metadata,
-                            directory=file_meta.directory,
-                            asset_ids=file_meta.asset_ids,
-                            data_set_id=file_meta.data_set_id,
-                            labels=file_meta.labels,
-                            geo_location=file_meta.geo_location,
-                            source_created_time=file_meta.source_created_time,
-                            source_modified_time=file_meta.source_modified_time,
-                            security_categories=file_meta.security_categories,
-                        ) as session:
-                            while chunks.next_chunk():
-                                session.upload_part(chunks.current_chunk, chunks)
-                            file_meta = session.file_metadata
-                    else:
-                        file_meta = self.cdf_client.files.upload_bytes(
-                            file,
-                            file_meta.name if file_meta.name is not None else "",
-                            overwrite=self.overwrite_existing,
-                            external_id=file_meta.external_id,
-                            source=file_meta.source,
-                            mime_type=file_meta.mime_type,
-                            metadata=file_meta.metadata,
-                            directory=file_meta.directory,
-                            asset_ids=file_meta.asset_ids,
-                            data_set_id=file_meta.data_set_id,
-                            labels=file_meta.labels,
-                            geo_location=file_meta.geo_location,
-                            source_created_time=file_meta.source_created_time,
-                            source_modified_time=file_meta.source_modified_time,
-                            security_categories=file_meta.security_categories,
-                        )
-
-                if self.post_upload_function:
-                    try:
-                        self.post_upload_function([file_meta])
-                    except Exception as e:
-                        self.logger.error("Error in upload callback: %s", str(e))
+                upload_file(read_file, file_meta)
 
             except Exception as e:
-                self.logger.exception("Unexpected error while uploading file")
+                self.logger.exception(f"Unexpected error while uploading file: {file_meta.external_id}")
                 self.errors.append(e)
 
             finally:
                 with self.lock:
                     self.files_written.inc()
                     self.upload_queue_size -= 1
                     self.queue_size.set(self.upload_queue_size)
@@ -327,15 +329,15 @@
 
         if self.upload_queue_size >= self.threshold:
             with self._full_queue:
                 while not self._full_queue.wait(timeout=2) and not self.cancellation_token.is_cancelled:
                     pass
 
         with self.lock:
-            self.upload_queue.append(self._pool.submit(_upload_single, read_file, file_meta))
+            self.upload_queue.append(self._pool.submit(wrapped_upload, read_file, file_meta))
             self.upload_queue_size += 1
             self.files_queued.inc()
             self.queue_size.set(self.upload_queue_size)
 
     def upload(self, fail_on_errors: bool = True, timeout: Optional[float] = None) -> None:
         """
         Wait for all uploads to finish
```

### Comparing `cognite_extractor_utils-7.1.4/cognite/extractorutils/uploader/raw.py` & `cognite_extractor_utils-7.1.5/cognite/extractorutils/uploader/raw.py`

 * *Files identical despite different names*

### Comparing `cognite_extractor_utils-7.1.4/cognite/extractorutils/uploader/time_series.py` & `cognite_extractor_utils-7.1.5/cognite/extractorutils/uploader/time_series.py`

 * *Files identical despite different names*

### Comparing `cognite_extractor_utils-7.1.4/cognite/extractorutils/uploader_extractor.py` & `cognite_extractor_utils-7.1.5/cognite/extractorutils/uploader_extractor.py`

 * *Files identical despite different names*

### Comparing `cognite_extractor_utils-7.1.4/cognite/extractorutils/uploader_types.py` & `cognite_extractor_utils-7.1.5/cognite/extractorutils/uploader_types.py`

 * *Files identical despite different names*

### Comparing `cognite_extractor_utils-7.1.4/cognite/extractorutils/util.py` & `cognite_extractor_utils-7.1.5/cognite/extractorutils/util.py`

 * *Files identical despite different names*

### Comparing `cognite_extractor_utils-7.1.4/pyproject.toml` & `cognite_extractor_utils-7.1.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cognite-extractor-utils"
-version = "7.1.4"
+version = "7.1.5"
 description = "Utilities for easier development of extractors for CDF"
 authors = ["Mathias Lohne <mathias.lohne@cognite.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 repository = "https://github.com/cognitedata/python-extractor-utils"
 
 packages = [
```

### Comparing `cognite_extractor_utils-7.1.4/PKG-INFO` & `cognite_extractor_utils-7.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cognite-extractor-utils
-Version: 7.1.4
+Version: 7.1.5
 Summary: Utilities for easier development of extractors for CDF
 Home-page: https://github.com/cognitedata/python-extractor-utils
 License: Apache-2.0
 Author: Mathias Lohne
 Author-email: mathias.lohne@cognite.com
 Requires-Python: >=3.8.0,<4.0.0
 Classifier: License :: OSI Approved :: Apache Software License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cognite-extractor-utils Version: 7.1.4 Summary:
+Metadata-Version: 2.1 Name: cognite-extractor-utils Version: 7.1.5 Summary:
 Utilities for easier development of extractors for CDF Home-page: https://
 github.com/cognitedata/python-extractor-utils License: Apache-2.0 Author:
 Mathias Lohne Author-email: mathias.lohne@cognite.com Requires-Python:
 >=3.8.0,<4.0.0 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
```

