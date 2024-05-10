# Comparing `tmp/watchmen_pipeline_kernel-16.6.8.tar.gz` & `tmp/watchmen_pipeline_kernel-16.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "watchmen_pipeline_kernel-16.6.8.tar", max compression
+gzip compressed data, was "watchmen_pipeline_kernel-16.6.9.tar", max compression
```

## Comparing `watchmen_pipeline_kernel-16.6.8.tar` & `watchmen_pipeline_kernel-16.6.9.tar`

### file list

```diff
@@ -1,44 +1,44 @@
--rw-r--r--   0        0        0     1061 2024-01-08 07:58:02.524594 watchmen_pipeline_kernel-16.6.8/LICENSE
--rw-r--r--   0        0        0     1165 2024-01-08 07:58:02.524594 watchmen_pipeline_kernel-16.6.8/pyproject.toml
--rw-r--r--   0        0        0        0 2024-01-08 07:58:02.524594 watchmen_pipeline_kernel-16.6.8/src/watchmen_pipeline_kernel/__init__.py
--rw-r--r--   0        0        0       75 2024-01-08 07:58:02.524594 watchmen_pipeline_kernel-16.6.8/src/watchmen_pipeline_kernel/boot/__init__.py
--rw-r--r--   0        0        0      643 2024-01-08 07:58:02.524594 watchmen_pipeline_kernel-16.6.8/src/watchmen_pipeline_kernel/boot/boot.py
--rw-r--r--   0        0        0       40 2024-01-08 07:58:02.524594 watchmen_pipeline_kernel-16.6.8/src/watchmen_pipeline_kernel/cache/__init__.py
--rw-r--r--   0        0        0      203 2024-01-08 07:58:02.524594 watchmen_pipeline_kernel-16.6.8/src/watchmen_pipeline_kernel/cache/cache_service.py
--rw-r--r--   0        0        0     1626 2024-01-08 07:58:02.524594 watchmen_pipeline_kernel-16.6.8/src/watchmen_pipeline_kernel/cache/compiled_pipeline_cache.py
--rw-r--r--   0        0        0      518 2024-01-08 07:58:02.524594 watchmen_pipeline_kernel-16.6.8/src/watchmen_pipeline_kernel/common/__init__.py
--rw-r--r--   0        0        0       48 2024-01-08 07:58:02.524594 watchmen_pipeline_kernel-16.6.8/src/watchmen_pipeline_kernel/common/exception.py
--rw-r--r--   0        0        0     3032 2024-01-08 07:58:02.524594 watchmen_pipeline_kernel-16.6.8/src/watchmen_pipeline_kernel/common/settings.py
--rw-r--r--   0        0        0      335 2024-01-08 07:58:02.524594 watchmen_pipeline_kernel-16.6.8/src/watchmen_pipeline_kernel/external_writer/__init__.py
--rw-r--r--   0        0        0      617 2024-01-08 07:58:02.524594 watchmen_pipeline_kernel-16.6.8/src/watchmen_pipeline_kernel/external_writer/elastic_search_writer.py
--rw-r--r--   0        0        0      763 2024-01-08 07:58:02.524594 watchmen_pipeline_kernel-16.6.8/src/watchmen_pipeline_kernel/external_writer/prebuilt_writers.py
--rw-r--r--   0        0        0     1895 2024-01-08 07:58:02.524594 watchmen_pipeline_kernel-16.6.8/src/watchmen_pipeline_kernel/external_writer/standard_writer.py
--rw-r--r--   0        0        0       68 2024-01-08 07:58:02.524594 watchmen_pipeline_kernel-16.6.8/src/watchmen_pipeline_kernel/monitor_log/__init__.py
--rw-r--r--   0        0        0     5489 2024-01-08 07:58:02.524594 watchmen_pipeline_kernel-16.6.8/src/watchmen_pipeline_kernel/monitor_log/monitor_log_data_service.py
--rw-r--r--   0        0        0      200 2024-01-08 07:58:02.524594 watchmen_pipeline_kernel-16.6.8/src/watchmen_pipeline_kernel/pipeline/__init__.py
--rw-r--r--   0        0        0     2119 2024-01-08 07:58:02.524594 watchmen_pipeline_kernel-16.6.8/src/watchmen_pipeline_kernel/pipeline/monitor_log_invoker.py
--rw-r--r--   0        0        0     3124 2024-01-08 07:58:02.524594 watchmen_pipeline_kernel-16.6.8/src/watchmen_pipeline_kernel/pipeline/pipeline_invoker.py
--rw-r--r--   0        0        0     6391 2024-01-08 07:58:02.524594 watchmen_pipeline_kernel-16.6.8/src/watchmen_pipeline_kernel/pipeline/pipeline_trigger.py
--rw-r--r--   0        0        0     1726 2024-01-08 07:58:02.524594 watchmen_pipeline_kernel-16.6.8/src/watchmen_pipeline_kernel/pipeline/pipelines_dispatcher.py
--rw-r--r--   0        0        0     2152 2024-01-08 07:58:02.524594 watchmen_pipeline_kernel-16.6.8/src/watchmen_pipeline_kernel/pipeline/sql_performance_invoker.py
--rw-r--r--   0        0        0       53 2024-01-08 07:58:02.524594 watchmen_pipeline_kernel-16.6.8/src/watchmen_pipeline_kernel/pipeline_schema/__init__.py
--rw-r--r--   0        0        0    40076 2024-01-08 07:58:02.524594 watchmen_pipeline_kernel-16.6.8/src/watchmen_pipeline_kernel/pipeline_schema/compiled_action.py
--rw-r--r--   0        0        0     7260 2024-01-08 07:58:02.524594 watchmen_pipeline_kernel-16.6.8/src/watchmen_pipeline_kernel/pipeline_schema/compiled_pipeline.py
--rw-r--r--   0        0        0     3967 2024-01-08 07:58:02.524594 watchmen_pipeline_kernel-16.6.8/src/watchmen_pipeline_kernel/pipeline_schema/compiled_single_unit.py
--rw-r--r--   0        0        0     3395 2024-01-08 07:58:02.524594 watchmen_pipeline_kernel-16.6.8/src/watchmen_pipeline_kernel/pipeline_schema/compiled_stage.py
--rw-r--r--   0        0        0     4440 2024-01-08 07:58:02.524594 watchmen_pipeline_kernel-16.6.8/src/watchmen_pipeline_kernel/pipeline_schema/compiled_unit.py
--rw-r--r--   0        0        0     7884 2024-01-08 07:58:02.524594 watchmen_pipeline_kernel-16.6.8/src/watchmen_pipeline_kernel/pipeline_schema/distributed_compiled_unit.py
--rw-r--r--   0        0        0     2206 2024-01-08 07:58:02.524594 watchmen_pipeline_kernel-16.6.8/src/watchmen_pipeline_kernel/pipeline_schema/pipeline_context.py
--rw-r--r--   0        0        0      191 2024-01-08 07:58:02.524594 watchmen_pipeline_kernel-16.6.8/src/watchmen_pipeline_kernel/pipeline_schema_interface/__init__.py
--rw-r--r--   0        0        0      804 2024-01-08 07:58:02.524594 watchmen_pipeline_kernel-16.6.8/src/watchmen_pipeline_kernel/pipeline_schema_interface/compiled_pipeline.py
--rw-r--r--   0        0        0      208 2024-01-08 07:58:02.524594 watchmen_pipeline_kernel-16.6.8/src/watchmen_pipeline_kernel/pipeline_schema_interface/create_queue_pipeline.py
--rw-r--r--   0        0        0      428 2024-01-08 07:58:02.524594 watchmen_pipeline_kernel-16.6.8/src/watchmen_pipeline_kernel/pipeline_schema_interface/pipeline_context.py
--rw-r--r--   0        0        0      292 2024-01-08 07:58:02.524594 watchmen_pipeline_kernel-16.6.8/src/watchmen_pipeline_kernel/pipeline_schema_interface/topic_storages.py
--rw-r--r--   0        0        0       47 2024-01-08 07:58:02.524594 watchmen_pipeline_kernel-16.6.8/src/watchmen_pipeline_kernel/topic/__init__.py
--rw-r--r--   0        0        0     1378 2024-01-08 07:58:02.524594 watchmen_pipeline_kernel-16.6.8/src/watchmen_pipeline_kernel/topic/topic_helper.py
--rw-r--r--   0        0        0      412 2024-01-08 07:58:02.524594 watchmen_pipeline_kernel-16.6.8/src/watchmen_pipeline_kernel/topic_snapshot/__init__.py
--rw-r--r--   0        0        0     5022 2024-01-08 07:58:02.524594 watchmen_pipeline_kernel-16.6.8/src/watchmen_pipeline_kernel/topic_snapshot/scheduler_launcher.py
--rw-r--r--   0        0        0     1907 2024-01-08 07:58:02.524594 watchmen_pipeline_kernel-16.6.8/src/watchmen_pipeline_kernel/topic_snapshot/scheduler_registrar.py
--rw-r--r--   0        0        0    14101 2024-01-08 07:58:02.524594 watchmen_pipeline_kernel-16.6.8/src/watchmen_pipeline_kernel/topic_snapshot/scheduler_runner.py
--rw-r--r--   0        0        0     6352 2024-01-08 07:58:02.524594 watchmen_pipeline_kernel-16.6.8/src/watchmen_pipeline_kernel/topic_snapshot/utils.py
--rw-r--r--   0        0        0     1298 1970-01-01 00:00:00.000000 watchmen_pipeline_kernel-16.6.8/PKG-INFO
+-rw-r--r--   0        0        0     1061 2024-02-01 01:32:37.255323 watchmen_pipeline_kernel-16.6.9/LICENSE
+-rw-r--r--   0        0        0     1165 2024-02-01 01:32:37.255323 watchmen_pipeline_kernel-16.6.9/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-02-01 01:32:37.255323 watchmen_pipeline_kernel-16.6.9/src/watchmen_pipeline_kernel/__init__.py
+-rw-r--r--   0        0        0       75 2024-02-01 01:32:37.255323 watchmen_pipeline_kernel-16.6.9/src/watchmen_pipeline_kernel/boot/__init__.py
+-rw-r--r--   0        0        0      643 2024-02-01 01:32:37.255323 watchmen_pipeline_kernel-16.6.9/src/watchmen_pipeline_kernel/boot/boot.py
+-rw-r--r--   0        0        0       40 2024-02-01 01:32:37.255323 watchmen_pipeline_kernel-16.6.9/src/watchmen_pipeline_kernel/cache/__init__.py
+-rw-r--r--   0        0        0      203 2024-02-01 01:32:37.255323 watchmen_pipeline_kernel-16.6.9/src/watchmen_pipeline_kernel/cache/cache_service.py
+-rw-r--r--   0        0        0     1626 2024-02-01 01:32:37.255323 watchmen_pipeline_kernel-16.6.9/src/watchmen_pipeline_kernel/cache/compiled_pipeline_cache.py
+-rw-r--r--   0        0        0      518 2024-02-01 01:32:37.255323 watchmen_pipeline_kernel-16.6.9/src/watchmen_pipeline_kernel/common/__init__.py
+-rw-r--r--   0        0        0       48 2024-02-01 01:32:37.255323 watchmen_pipeline_kernel-16.6.9/src/watchmen_pipeline_kernel/common/exception.py
+-rw-r--r--   0        0        0     3032 2024-02-01 01:32:37.255323 watchmen_pipeline_kernel-16.6.9/src/watchmen_pipeline_kernel/common/settings.py
+-rw-r--r--   0        0        0      335 2024-02-01 01:32:37.255323 watchmen_pipeline_kernel-16.6.9/src/watchmen_pipeline_kernel/external_writer/__init__.py
+-rw-r--r--   0        0        0      617 2024-02-01 01:32:37.255323 watchmen_pipeline_kernel-16.6.9/src/watchmen_pipeline_kernel/external_writer/elastic_search_writer.py
+-rw-r--r--   0        0        0      763 2024-02-01 01:32:37.255323 watchmen_pipeline_kernel-16.6.9/src/watchmen_pipeline_kernel/external_writer/prebuilt_writers.py
+-rw-r--r--   0        0        0     1895 2024-02-01 01:32:37.255323 watchmen_pipeline_kernel-16.6.9/src/watchmen_pipeline_kernel/external_writer/standard_writer.py
+-rw-r--r--   0        0        0       68 2024-02-01 01:32:37.255323 watchmen_pipeline_kernel-16.6.9/src/watchmen_pipeline_kernel/monitor_log/__init__.py
+-rw-r--r--   0        0        0     5489 2024-02-01 01:32:37.255323 watchmen_pipeline_kernel-16.6.9/src/watchmen_pipeline_kernel/monitor_log/monitor_log_data_service.py
+-rw-r--r--   0        0        0      200 2024-02-01 01:32:37.259323 watchmen_pipeline_kernel-16.6.9/src/watchmen_pipeline_kernel/pipeline/__init__.py
+-rw-r--r--   0        0        0     2119 2024-02-01 01:32:37.259323 watchmen_pipeline_kernel-16.6.9/src/watchmen_pipeline_kernel/pipeline/monitor_log_invoker.py
+-rw-r--r--   0        0        0     3124 2024-02-01 01:32:37.259323 watchmen_pipeline_kernel-16.6.9/src/watchmen_pipeline_kernel/pipeline/pipeline_invoker.py
+-rw-r--r--   0        0        0     6391 2024-02-01 01:32:37.259323 watchmen_pipeline_kernel-16.6.9/src/watchmen_pipeline_kernel/pipeline/pipeline_trigger.py
+-rw-r--r--   0        0        0     1221 2024-02-01 01:32:37.259323 watchmen_pipeline_kernel-16.6.9/src/watchmen_pipeline_kernel/pipeline/pipelines_dispatcher.py
+-rw-r--r--   0        0        0     2152 2024-02-01 01:32:37.259323 watchmen_pipeline_kernel-16.6.9/src/watchmen_pipeline_kernel/pipeline/sql_performance_invoker.py
+-rw-r--r--   0        0        0       53 2024-02-01 01:32:37.259323 watchmen_pipeline_kernel-16.6.9/src/watchmen_pipeline_kernel/pipeline_schema/__init__.py
+-rw-r--r--   0        0        0    40076 2024-02-01 01:32:37.259323 watchmen_pipeline_kernel-16.6.9/src/watchmen_pipeline_kernel/pipeline_schema/compiled_action.py
+-rw-r--r--   0        0        0     7260 2024-02-01 01:32:37.259323 watchmen_pipeline_kernel-16.6.9/src/watchmen_pipeline_kernel/pipeline_schema/compiled_pipeline.py
+-rw-r--r--   0        0        0     3967 2024-02-01 01:32:37.259323 watchmen_pipeline_kernel-16.6.9/src/watchmen_pipeline_kernel/pipeline_schema/compiled_single_unit.py
+-rw-r--r--   0        0        0     3395 2024-02-01 01:32:37.259323 watchmen_pipeline_kernel-16.6.9/src/watchmen_pipeline_kernel/pipeline_schema/compiled_stage.py
+-rw-r--r--   0        0        0     4440 2024-02-01 01:32:37.259323 watchmen_pipeline_kernel-16.6.9/src/watchmen_pipeline_kernel/pipeline_schema/compiled_unit.py
+-rw-r--r--   0        0        0     7884 2024-02-01 01:32:37.259323 watchmen_pipeline_kernel-16.6.9/src/watchmen_pipeline_kernel/pipeline_schema/distributed_compiled_unit.py
+-rw-r--r--   0        0        0     2206 2024-02-01 01:32:37.259323 watchmen_pipeline_kernel-16.6.9/src/watchmen_pipeline_kernel/pipeline_schema/pipeline_context.py
+-rw-r--r--   0        0        0      191 2024-02-01 01:32:37.259323 watchmen_pipeline_kernel-16.6.9/src/watchmen_pipeline_kernel/pipeline_schema_interface/__init__.py
+-rw-r--r--   0        0        0      804 2024-02-01 01:32:37.259323 watchmen_pipeline_kernel-16.6.9/src/watchmen_pipeline_kernel/pipeline_schema_interface/compiled_pipeline.py
+-rw-r--r--   0        0        0      208 2024-02-01 01:32:37.259323 watchmen_pipeline_kernel-16.6.9/src/watchmen_pipeline_kernel/pipeline_schema_interface/create_queue_pipeline.py
+-rw-r--r--   0        0        0      428 2024-02-01 01:32:37.259323 watchmen_pipeline_kernel-16.6.9/src/watchmen_pipeline_kernel/pipeline_schema_interface/pipeline_context.py
+-rw-r--r--   0        0        0      292 2024-02-01 01:32:37.259323 watchmen_pipeline_kernel-16.6.9/src/watchmen_pipeline_kernel/pipeline_schema_interface/topic_storages.py
+-rw-r--r--   0        0        0       47 2024-02-01 01:32:37.259323 watchmen_pipeline_kernel-16.6.9/src/watchmen_pipeline_kernel/topic/__init__.py
+-rw-r--r--   0        0        0     1378 2024-02-01 01:32:37.259323 watchmen_pipeline_kernel-16.6.9/src/watchmen_pipeline_kernel/topic/topic_helper.py
+-rw-r--r--   0        0        0      412 2024-02-01 01:32:37.259323 watchmen_pipeline_kernel-16.6.9/src/watchmen_pipeline_kernel/topic_snapshot/__init__.py
+-rw-r--r--   0        0        0     5022 2024-02-01 01:32:37.259323 watchmen_pipeline_kernel-16.6.9/src/watchmen_pipeline_kernel/topic_snapshot/scheduler_launcher.py
+-rw-r--r--   0        0        0     1907 2024-02-01 01:32:37.259323 watchmen_pipeline_kernel-16.6.9/src/watchmen_pipeline_kernel/topic_snapshot/scheduler_registrar.py
+-rw-r--r--   0        0        0    14101 2024-02-01 01:32:37.259323 watchmen_pipeline_kernel-16.6.9/src/watchmen_pipeline_kernel/topic_snapshot/scheduler_runner.py
+-rw-r--r--   0        0        0     6352 2024-02-01 01:32:37.259323 watchmen_pipeline_kernel-16.6.9/src/watchmen_pipeline_kernel/topic_snapshot/utils.py
+-rw-r--r--   0        0        0     1298 1970-01-01 00:00:00.000000 watchmen_pipeline_kernel-16.6.9/PKG-INFO
```

### Comparing `watchmen_pipeline_kernel-16.6.8/LICENSE` & `watchmen_pipeline_kernel-16.6.9/LICENSE`

 * *Files identical despite different names*

### Comparing `watchmen_pipeline_kernel-16.6.8/pyproject.toml` & `watchmen_pipeline_kernel-16.6.9/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 [tool.poetry]
 name = "watchmen-pipeline-kernel"
-version = "16.6.8"
+version = "16.6.9"
 description = ""
 authors = ["botlikes <75356972+botlikes456@users.noreply.github.com>"]
 license = "MIT"
 packages = [
     { include = "watchmen_pipeline_kernel", from = "src" }
 ]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 dask = "^2022.9.1"
 distributed = "^2022.9.1"
 APScheduler = "^3.9.1"
-watchmen-data-kernel = "16.6.8"
-watchmen-storage-mysql = { version = "16.6.8", optional = true }
-watchmen-storage-oracle = { version = "16.6.8", optional = true }
-watchmen-storage-mongodb = { version = "16.6.8", optional = true }
-watchmen-storage-mssql = { version = "16.6.8", optional = true }
-watchmen-storage-postgresql = { version = "16.6.8", optional = true }
+watchmen-data-kernel = "16.6.9"
+watchmen-storage-mysql = { version = "16.6.9", optional = true }
+watchmen-storage-oracle = { version = "16.6.9", optional = true }
+watchmen-storage-mongodb = { version = "16.6.9", optional = true }
+watchmen-storage-mssql = { version = "16.6.9", optional = true }
+watchmen-storage-postgresql = { version = "16.6.9", optional = true }
 requests = { version = "^2.27.1", optional = true }
 
 [tool.poetry.dev-dependencies]
 
 [tool.poetry.extras]
 mysql = ["watchmen-storage-mysql"]
 oracle = ["watchmen-storage-oracle"]
```

### Comparing `watchmen_pipeline_kernel-16.6.8/src/watchmen_pipeline_kernel/boot/boot.py` & `watchmen_pipeline_kernel-16.6.9/src/watchmen_pipeline_kernel/boot/boot.py`

 * *Files identical despite different names*

### Comparing `watchmen_pipeline_kernel-16.6.8/src/watchmen_pipeline_kernel/cache/compiled_pipeline_cache.py` & `watchmen_pipeline_kernel-16.6.9/src/watchmen_pipeline_kernel/cache/compiled_pipeline_cache.py`

 * *Files identical despite different names*

### Comparing `watchmen_pipeline_kernel-16.6.8/src/watchmen_pipeline_kernel/common/__init__.py` & `watchmen_pipeline_kernel-16.6.9/src/watchmen_pipeline_kernel/common/__init__.py`

 * *Files identical despite different names*

### Comparing `watchmen_pipeline_kernel-16.6.8/src/watchmen_pipeline_kernel/common/settings.py` & `watchmen_pipeline_kernel-16.6.9/src/watchmen_pipeline_kernel/common/settings.py`

 * *Files identical despite different names*

### Comparing `watchmen_pipeline_kernel-16.6.8/src/watchmen_pipeline_kernel/external_writer/elastic_search_writer.py` & `watchmen_pipeline_kernel-16.6.9/src/watchmen_pipeline_kernel/external_writer/elastic_search_writer.py`

 * *Files identical despite different names*

### Comparing `watchmen_pipeline_kernel-16.6.8/src/watchmen_pipeline_kernel/external_writer/prebuilt_writers.py` & `watchmen_pipeline_kernel-16.6.9/src/watchmen_pipeline_kernel/external_writer/prebuilt_writers.py`

 * *Files identical despite different names*

### Comparing `watchmen_pipeline_kernel-16.6.8/src/watchmen_pipeline_kernel/external_writer/standard_writer.py` & `watchmen_pipeline_kernel-16.6.9/src/watchmen_pipeline_kernel/external_writer/standard_writer.py`

 * *Files identical despite different names*

### Comparing `watchmen_pipeline_kernel-16.6.8/src/watchmen_pipeline_kernel/monitor_log/monitor_log_data_service.py` & `watchmen_pipeline_kernel-16.6.9/src/watchmen_pipeline_kernel/monitor_log/monitor_log_data_service.py`

 * *Files identical despite different names*

### Comparing `watchmen_pipeline_kernel-16.6.8/src/watchmen_pipeline_kernel/pipeline/monitor_log_invoker.py` & `watchmen_pipeline_kernel-16.6.9/src/watchmen_pipeline_kernel/pipeline/monitor_log_invoker.py`

 * *Files identical despite different names*

### Comparing `watchmen_pipeline_kernel-16.6.8/src/watchmen_pipeline_kernel/pipeline/pipeline_invoker.py` & `watchmen_pipeline_kernel-16.6.9/src/watchmen_pipeline_kernel/pipeline/pipeline_invoker.py`

 * *Files identical despite different names*

### Comparing `watchmen_pipeline_kernel-16.6.8/src/watchmen_pipeline_kernel/pipeline/pipeline_trigger.py` & `watchmen_pipeline_kernel-16.6.9/src/watchmen_pipeline_kernel/pipeline/pipeline_trigger.py`

 * *Files identical despite different names*

### Comparing `watchmen_pipeline_kernel-16.6.8/src/watchmen_pipeline_kernel/pipeline/pipelines_dispatcher.py` & `watchmen_pipeline_kernel-16.6.9/src/watchmen_pipeline_kernel/pipeline/pipelines_dispatcher.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,45 +1,31 @@
 import logging
 from typing import Callable, List, Optional
 
 from watchmen_model.pipeline_kernel import PipelineMonitorLog
-from watchmen_pipeline_kernel.common import PipelineKernelException, ask_pipeline_recursion_limit
+from watchmen_pipeline_kernel.common import PipelineKernelException
 from watchmen_pipeline_kernel.pipeline_schema import RuntimePipelineContext
 from watchmen_pipeline_kernel.topic import RuntimeTopicStorages
 
 
 logger = logging.getLogger(__name__)
 
 
 class PipelinesDispatcher:
 	def __init__(self, contexts: List[RuntimePipelineContext], storages: RuntimeTopicStorages):
 		self.contexts = contexts
 		self.storages = storages
-		self.pipelineRecursionLimit = ask_pipeline_recursion_limit()
 
-	def start(self, handle_monitor_log: Callable[[PipelineMonitorLog, bool], None], limit: int = None) -> None:
-		context = self.next_context()
-		if context is None:
-			# no context needs to be invoked
-			return None
-		created_contexts = context.start(self.storages, handle_monitor_log)
-		if len(created_contexts) != 0:
-			# noinspection PyTypeChecker
-			self.contexts.extend(created_contexts)
-		# invoke next
-		try:
-			if limit is None:
-				self.start(handle_monitor_log, self.pipelineRecursionLimit)
-			elif limit == 0:
-				raise RecursionError("maximum recursion depth exceeded in comparison")
-			else:
-				self.start(handle_monitor_log, limit-1)
-		except RecursionError as e:
-			logger.error(e, exc_info=True, stack_info=True)
-			raise e
+	def start(self, handle_monitor_log: Callable[[PipelineMonitorLog, bool], None]) -> None:
+		while self.contexts:
+			context = self.next_context()
+			created_contexts = context.start(self.storages, handle_monitor_log)
+			if len(created_contexts) != 0:
+				# noinspection PyTypeChecker
+				self.contexts.extend(created_contexts)
 
 	def next_context(self) -> Optional[RuntimePipelineContext]:
 		if len(self.contexts) == 0:
 			return None
 		# get next context
 		context = self.contexts[0]
 		if context is None:
```

### Comparing `watchmen_pipeline_kernel-16.6.8/src/watchmen_pipeline_kernel/pipeline/sql_performance_invoker.py` & `watchmen_pipeline_kernel-16.6.9/src/watchmen_pipeline_kernel/pipeline/sql_performance_invoker.py`

 * *Files identical despite different names*

### Comparing `watchmen_pipeline_kernel-16.6.8/src/watchmen_pipeline_kernel/pipeline_schema/compiled_action.py` & `watchmen_pipeline_kernel-16.6.9/src/watchmen_pipeline_kernel/pipeline_schema/compiled_action.py`

 * *Files identical despite different names*

### Comparing `watchmen_pipeline_kernel-16.6.8/src/watchmen_pipeline_kernel/pipeline_schema/compiled_pipeline.py` & `watchmen_pipeline_kernel-16.6.9/src/watchmen_pipeline_kernel/pipeline_schema/compiled_pipeline.py`

 * *Files identical despite different names*

### Comparing `watchmen_pipeline_kernel-16.6.8/src/watchmen_pipeline_kernel/pipeline_schema/compiled_single_unit.py` & `watchmen_pipeline_kernel-16.6.9/src/watchmen_pipeline_kernel/pipeline_schema/compiled_single_unit.py`

 * *Files identical despite different names*

### Comparing `watchmen_pipeline_kernel-16.6.8/src/watchmen_pipeline_kernel/pipeline_schema/compiled_stage.py` & `watchmen_pipeline_kernel-16.6.9/src/watchmen_pipeline_kernel/pipeline_schema/compiled_stage.py`

 * *Files identical despite different names*

### Comparing `watchmen_pipeline_kernel-16.6.8/src/watchmen_pipeline_kernel/pipeline_schema/compiled_unit.py` & `watchmen_pipeline_kernel-16.6.9/src/watchmen_pipeline_kernel/pipeline_schema/compiled_unit.py`

 * *Files identical despite different names*

### Comparing `watchmen_pipeline_kernel-16.6.8/src/watchmen_pipeline_kernel/pipeline_schema/distributed_compiled_unit.py` & `watchmen_pipeline_kernel-16.6.9/src/watchmen_pipeline_kernel/pipeline_schema/distributed_compiled_unit.py`

 * *Files identical despite different names*

### Comparing `watchmen_pipeline_kernel-16.6.8/src/watchmen_pipeline_kernel/pipeline_schema/pipeline_context.py` & `watchmen_pipeline_kernel-16.6.9/src/watchmen_pipeline_kernel/pipeline_schema/pipeline_context.py`

 * *Files identical despite different names*

### Comparing `watchmen_pipeline_kernel-16.6.8/src/watchmen_pipeline_kernel/pipeline_schema_interface/compiled_pipeline.py` & `watchmen_pipeline_kernel-16.6.9/src/watchmen_pipeline_kernel/pipeline_schema_interface/compiled_pipeline.py`

 * *Files identical despite different names*

### Comparing `watchmen_pipeline_kernel-16.6.8/src/watchmen_pipeline_kernel/topic/topic_helper.py` & `watchmen_pipeline_kernel-16.6.9/src/watchmen_pipeline_kernel/topic/topic_helper.py`

 * *Files identical despite different names*

### Comparing `watchmen_pipeline_kernel-16.6.8/src/watchmen_pipeline_kernel/topic_snapshot/scheduler_launcher.py` & `watchmen_pipeline_kernel-16.6.9/src/watchmen_pipeline_kernel/topic_snapshot/scheduler_launcher.py`

 * *Files identical despite different names*

### Comparing `watchmen_pipeline_kernel-16.6.8/src/watchmen_pipeline_kernel/topic_snapshot/scheduler_registrar.py` & `watchmen_pipeline_kernel-16.6.9/src/watchmen_pipeline_kernel/topic_snapshot/scheduler_registrar.py`

 * *Files identical despite different names*

### Comparing `watchmen_pipeline_kernel-16.6.8/src/watchmen_pipeline_kernel/topic_snapshot/scheduler_runner.py` & `watchmen_pipeline_kernel-16.6.9/src/watchmen_pipeline_kernel/topic_snapshot/scheduler_runner.py`

 * *Files identical despite different names*

### Comparing `watchmen_pipeline_kernel-16.6.8/src/watchmen_pipeline_kernel/topic_snapshot/utils.py` & `watchmen_pipeline_kernel-16.6.9/src/watchmen_pipeline_kernel/topic_snapshot/utils.py`

 * *Files identical despite different names*

### Comparing `watchmen_pipeline_kernel-16.6.8/PKG-INFO` & `watchmen_pipeline_kernel-16.6.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: watchmen-pipeline-kernel
-Version: 16.6.8
+Version: 16.6.9
 Summary: 
 License: MIT
 Author: botlikes
 Author-email: 75356972+botlikes456@users.noreply.github.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -19,13 +19,13 @@
 Provides-Extra: oracle
 Provides-Extra: postgresql
 Provides-Extra: standard-ext-writer
 Requires-Dist: APScheduler (>=3.9.1,<4.0.0)
 Requires-Dist: dask (>=2022.9.1,<2023.0.0)
 Requires-Dist: distributed (>=2022.9.1,<2023.0.0)
 Requires-Dist: requests (>=2.27.1,<3.0.0) ; extra == "standard-ext-writer"
-Requires-Dist: watchmen-data-kernel (==16.6.8)
-Requires-Dist: watchmen-storage-mongodb (==16.6.8) ; extra == "mongodb"
-Requires-Dist: watchmen-storage-mssql (==16.6.8) ; extra == "mssql"
-Requires-Dist: watchmen-storage-mysql (==16.6.8) ; extra == "mysql"
-Requires-Dist: watchmen-storage-oracle (==16.6.8) ; extra == "oracle"
-Requires-Dist: watchmen-storage-postgresql (==16.6.8) ; extra == "postgresql"
+Requires-Dist: watchmen-data-kernel (==16.6.9)
+Requires-Dist: watchmen-storage-mongodb (==16.6.9) ; extra == "mongodb"
+Requires-Dist: watchmen-storage-mssql (==16.6.9) ; extra == "mssql"
+Requires-Dist: watchmen-storage-mysql (==16.6.9) ; extra == "mysql"
+Requires-Dist: watchmen-storage-oracle (==16.6.9) ; extra == "oracle"
+Requires-Dist: watchmen-storage-postgresql (==16.6.9) ; extra == "postgresql"
```

