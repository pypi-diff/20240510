# Comparing `tmp/nucliadb_telemetry-3.0.3.post490-py3-none-any.whl.zip` & `tmp/nucliadb_telemetry-3.0.3.post491-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 73937 bytes, number of entries: 49
+Zip file size: 73927 bytes, number of entries: 49
 -rw-r--r--  2.0 unx      899 b- defN 24-May-09 14:25 nucliadb_telemetry/__init__.py
 -rw-r--r--  2.0 unx    12171 b- defN 24-May-09 14:25 nucliadb_telemetry/batch_span.py
 -rw-r--r--  2.0 unx     1254 b- defN 24-May-09 14:25 nucliadb_telemetry/common.py
 -rw-r--r--  2.0 unx     2456 b- defN 24-May-09 14:25 nucliadb_telemetry/context.py
 -rw-r--r--  2.0 unx     4485 b- defN 24-May-09 14:25 nucliadb_telemetry/errors.py
 -rw-r--r--  2.0 unx    15114 b- defN 24-May-09 14:25 nucliadb_telemetry/grpc.py
 -rw-r--r--  2.0 unx     5350 b- defN 24-May-09 14:25 nucliadb_telemetry/grpc_metrics.py
@@ -40,12 +40,12 @@
 -rw-r--r--  2.0 unx     6982 b- defN 24-May-09 14:25 nucliadb_telemetry/tests/unit/test_metrics.py
 -rw-r--r--  2.0 unx     5175 b- defN 24-May-09 14:25 nucliadb_telemetry/tests/unit/test_tikv_instrumentation.py
 -rw-r--r--  2.0 unx      833 b- defN 24-May-09 14:25 nucliadb_telemetry/tests/unit/fastapi/__init__.py
 -rw-r--r--  2.0 unx     1608 b- defN 24-May-09 14:25 nucliadb_telemetry/tests/unit/fastapi/test_context.py
 -rw-r--r--  2.0 unx     1381 b- defN 24-May-09 14:25 nucliadb_telemetry/tests/unit/fastapi/test_fastapi.py
 -rw-r--r--  2.0 unx     2290 b- defN 24-May-09 14:25 nucliadb_telemetry/tests/unit/fastapi/test_tracing.py
 -rw-r--r--  2.0 unx     1369 b- defN 24-May-09 14:25 nucliadb_telemetry/tests/unit/fastapi/test_utils.py
--rw-r--r--  2.0 unx    11397 b- defN 24-May-09 14:26 nucliadb_telemetry-3.0.3.post490.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-09 14:26 nucliadb_telemetry-3.0.3.post490.dist-info/WHEEL
--rw-r--r--  2.0 unx       19 b- defN 24-May-09 14:26 nucliadb_telemetry-3.0.3.post490.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     4724 b- defN 24-May-09 14:26 nucliadb_telemetry-3.0.3.post490.dist-info/RECORD
-49 files, 215709 bytes uncompressed, 66205 bytes compressed:  69.3%
+-rw-r--r--  2.0 unx    11397 b- defN 24-May-09 14:27 nucliadb_telemetry-3.0.3.post491.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-09 14:27 nucliadb_telemetry-3.0.3.post491.dist-info/WHEEL
+-rw-r--r--  2.0 unx       19 b- defN 24-May-09 14:27 nucliadb_telemetry-3.0.3.post491.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     4724 b- defN 24-May-09 14:27 nucliadb_telemetry-3.0.3.post491.dist-info/RECORD
+49 files, 215709 bytes uncompressed, 66195 bytes compressed:  69.3%
```

## zipnote {}

```diff
@@ -129,20 +129,20 @@
 
 Filename: nucliadb_telemetry/tests/unit/fastapi/test_tracing.py
 Comment: 
 
 Filename: nucliadb_telemetry/tests/unit/fastapi/test_utils.py
 Comment: 
 
-Filename: nucliadb_telemetry-3.0.3.post490.dist-info/METADATA
+Filename: nucliadb_telemetry-3.0.3.post491.dist-info/METADATA
 Comment: 
 
-Filename: nucliadb_telemetry-3.0.3.post490.dist-info/WHEEL
+Filename: nucliadb_telemetry-3.0.3.post491.dist-info/WHEEL
 Comment: 
 
-Filename: nucliadb_telemetry-3.0.3.post490.dist-info/top_level.txt
+Filename: nucliadb_telemetry-3.0.3.post491.dist-info/top_level.txt
 Comment: 
 
-Filename: nucliadb_telemetry-3.0.3.post490.dist-info/RECORD
+Filename: nucliadb_telemetry-3.0.3.post491.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `nucliadb_telemetry-3.0.3.post490.dist-info/METADATA` & `nucliadb_telemetry-3.0.3.post491.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nucliadb-telemetry
-Version: 3.0.3.post490
+Version: 3.0.3.post491
 Summary: NucliaDB Telemetry Library Python process
 Home-page: https://github.com/nuclia/nucliadb
 Author: nucliadb Authors
 Author-email: nucliadb@nuclia.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -21,32 +21,32 @@
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: pydantic
 Requires-Dist: prometheus-client >=0.12.0
 Requires-Dist: orjson >=3.6.7
 Requires-Dist: wrapt >=1.14.1
 Provides-Extra: all
-Requires-Dist: opentelemetry-instrumentation-fastapi >=0.42b0 ; extra == 'all'
-Requires-Dist: opentelemetry-proto ==1.21.0 ; extra == 'all'
 Requires-Dist: opentelemetry-exporter-jaeger ==1.21.0 ; extra == 'all'
-Requires-Dist: fastapi ; extra == 'all'
+Requires-Dist: opentelemetry-instrumentation-fastapi >=0.42b0 ; extra == 'all'
 Requires-Dist: grpcio-reflection <1.63.0,>=1.44.0 ; extra == 'all'
-Requires-Dist: grpcio <1.63.0,>=1.44.0 ; extra == 'all'
-Requires-Dist: opentelemetry-api ==1.21.0 ; extra == 'all'
-Requires-Dist: nats-py[nkeys] >=2.5.0 ; extra == 'all'
-Requires-Dist: opentelemetry-propagator-b3 ==1.21.0 ; extra == 'all'
-Requires-Dist: opentelemetry-sdk ==1.21.0 ; extra == 'all'
-Requires-Dist: grpcio-tools <1.63.0,>=1.44.0 ; extra == 'all'
+Requires-Dist: opentelemetry-proto ==1.21.0 ; extra == 'all'
 Requires-Dist: grpcio-testing <1.63.0,>=1.44.0 ; extra == 'all'
-Requires-Dist: grpcio-status <1.63.0,>=1.44.0 ; extra == 'all'
 Requires-Dist: tikv-client >=0.0.3 ; extra == 'all'
-Requires-Dist: grpcio-channelz <1.63.0,>=1.44.0 ; extra == 'all'
 Requires-Dist: opentelemetry-instrumentation-aiohttp-client >=0.42b0 ; extra == 'all'
-Requires-Dist: grpcio-health-checking <1.63.0,>=1.44.0 ; extra == 'all'
 Requires-Dist: opentelemetry-semantic-conventions >=0.42b0 ; extra == 'all'
+Requires-Dist: grpcio-channelz <1.63.0,>=1.44.0 ; extra == 'all'
+Requires-Dist: grpcio-status <1.63.0,>=1.44.0 ; extra == 'all'
+Requires-Dist: grpcio-health-checking <1.63.0,>=1.44.0 ; extra == 'all'
+Requires-Dist: opentelemetry-api ==1.21.0 ; extra == 'all'
+Requires-Dist: grpcio <1.63.0,>=1.44.0 ; extra == 'all'
+Requires-Dist: nats-py[nkeys] >=2.5.0 ; extra == 'all'
+Requires-Dist: fastapi ; extra == 'all'
+Requires-Dist: opentelemetry-sdk ==1.21.0 ; extra == 'all'
+Requires-Dist: opentelemetry-propagator-b3 ==1.21.0 ; extra == 'all'
+Requires-Dist: grpcio-tools <1.63.0,>=1.44.0 ; extra == 'all'
 Provides-Extra: fastapi
 Requires-Dist: fastapi ; extra == 'fastapi'
 Requires-Dist: opentelemetry-sdk ==1.21.0 ; extra == 'fastapi'
 Requires-Dist: opentelemetry-api ==1.21.0 ; extra == 'fastapi'
 Requires-Dist: opentelemetry-proto ==1.21.0 ; extra == 'fastapi'
 Requires-Dist: opentelemetry-exporter-jaeger ==1.21.0 ; extra == 'fastapi'
 Requires-Dist: opentelemetry-propagator-b3 ==1.21.0 ; extra == 'fastapi'
```

## Comparing `nucliadb_telemetry-3.0.3.post490.dist-info/RECORD` & `nucliadb_telemetry-3.0.3.post491.dist-info/RECORD`

 * *Files 6% similar despite different names*

```diff
@@ -39,11 +39,11 @@
 nucliadb_telemetry/tests/unit/test_metrics.py,sha256=PiTZ3SpAErhx8VHqWgTK48Hgz1tNAPCFhSwN4GU0c_8,6982
 nucliadb_telemetry/tests/unit/test_tikv_instrumentation.py,sha256=WN7f5LHpeIusIrmqQ3qbaHmebP2BZCtDvuCdJVj2wYA,5175
 nucliadb_telemetry/tests/unit/fastapi/__init__.py,sha256=itSI7dtTwFP55YMX4iK7JzdMHS5CQVUiB1XzQu4UBh8,833
 nucliadb_telemetry/tests/unit/fastapi/test_context.py,sha256=7cSVXByQaR-7KzalWou6I9cB1hUhFy7YtqY0a4RGRjo,1608
 nucliadb_telemetry/tests/unit/fastapi/test_fastapi.py,sha256=xpo1Bm_BacUNfY6saT1wpf7G--24cphCBglU3Y5AkDY,1381
 nucliadb_telemetry/tests/unit/fastapi/test_tracing.py,sha256=GOurw4CtxqiR5_tx1rWUEoI6lj-Ft6A0eLnN598KHyY,2290
 nucliadb_telemetry/tests/unit/fastapi/test_utils.py,sha256=A5aVJlzksVgIG3A8KJQHVah2BEc4c91Fif997HnHtN4,1369
-nucliadb_telemetry-3.0.3.post490.dist-info/METADATA,sha256=4zJ0xPKCiGs3Nwq_6ebWcS5HHGc7wYWOlbZsuZJZib0,11397
-nucliadb_telemetry-3.0.3.post490.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-nucliadb_telemetry-3.0.3.post490.dist-info/top_level.txt,sha256=3qEHI_5ttqQIL2gkNYwSlKsFyBBiEzDiIy9UKISzOaQ,19
-nucliadb_telemetry-3.0.3.post490.dist-info/RECORD,,
+nucliadb_telemetry-3.0.3.post491.dist-info/METADATA,sha256=cjk0fKu7akGNcPtbKOtOdeCmzAdMMkf8zt_7llwcxgw,11397
+nucliadb_telemetry-3.0.3.post491.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+nucliadb_telemetry-3.0.3.post491.dist-info/top_level.txt,sha256=3qEHI_5ttqQIL2gkNYwSlKsFyBBiEzDiIy9UKISzOaQ,19
+nucliadb_telemetry-3.0.3.post491.dist-info/RECORD,,
```

