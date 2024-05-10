# Comparing `tmp/nucliadb_utils-3.0.3.post490-py3-none-any.whl.zip` & `tmp/nucliadb_utils-3.0.3.post491-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -60,13 +60,13 @@
 -rw-r--r--  2.0 unx     3917 b- defN 24-May-09 14:25 nucliadb_utils/tests/unit/test_transaction.py
 -rw-r--r--  2.0 unx     5099 b- defN 24-May-09 14:25 nucliadb_utils/tests/unit/test_utilities.py
 -rw-r--r--  2.0 unx      833 b- defN 24-May-09 14:25 nucliadb_utils/tests/unit/storages/__init__.py
 -rw-r--r--  2.0 unx     1924 b- defN 24-May-09 14:25 nucliadb_utils/tests/unit/storages/test_aws.py
 -rw-r--r--  2.0 unx     3554 b- defN 24-May-09 14:25 nucliadb_utils/tests/unit/storages/test_gcs.py
 -rw-r--r--  2.0 unx    17000 b- defN 24-May-09 14:25 nucliadb_utils/tests/unit/storages/test_pg.py
 -rw-r--r--  2.0 unx     6892 b- defN 24-May-09 14:25 nucliadb_utils/tests/unit/storages/test_storage.py
--rw-r--r--  2.0 unx     1975 b- defN 24-May-09 14:26 nucliadb_utils-3.0.3.post490.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-09 14:26 nucliadb_utils-3.0.3.post490.dist-info/WHEEL
--rw-r--r--  2.0 unx       15 b- defN 24-May-09 14:26 nucliadb_utils-3.0.3.post490.dist-info/top_level.txt
--rw-r--r--  2.0 unx        1 b- defN 24-May-09 14:25 nucliadb_utils-3.0.3.post490.dist-info/zip-safe
--rw-rw-r--  2.0 unx     6273 b- defN 24-May-09 14:26 nucliadb_utils-3.0.3.post490.dist-info/RECORD
+-rw-r--r--  2.0 unx     1975 b- defN 24-May-09 14:27 nucliadb_utils-3.0.3.post491.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-09 14:27 nucliadb_utils-3.0.3.post491.dist-info/WHEEL
+-rw-r--r--  2.0 unx       15 b- defN 24-May-09 14:27 nucliadb_utils-3.0.3.post491.dist-info/top_level.txt
+-rw-r--r--  2.0 unx        1 b- defN 24-May-09 14:26 nucliadb_utils-3.0.3.post491.dist-info/zip-safe
+-rw-rw-r--  2.0 unx     6273 b- defN 24-May-09 14:27 nucliadb_utils-3.0.3.post491.dist-info/RECORD
 70 files, 309441 bytes uncompressed, 96898 bytes compressed:  68.7%
```

## zipnote {}

```diff
@@ -189,23 +189,23 @@
 
 Filename: nucliadb_utils/tests/unit/storages/test_pg.py
 Comment: 
 
 Filename: nucliadb_utils/tests/unit/storages/test_storage.py
 Comment: 
 
-Filename: nucliadb_utils-3.0.3.post490.dist-info/METADATA
+Filename: nucliadb_utils-3.0.3.post491.dist-info/METADATA
 Comment: 
 
-Filename: nucliadb_utils-3.0.3.post490.dist-info/WHEEL
+Filename: nucliadb_utils-3.0.3.post491.dist-info/WHEEL
 Comment: 
 
-Filename: nucliadb_utils-3.0.3.post490.dist-info/top_level.txt
+Filename: nucliadb_utils-3.0.3.post491.dist-info/top_level.txt
 Comment: 
 
-Filename: nucliadb_utils-3.0.3.post490.dist-info/zip-safe
+Filename: nucliadb_utils-3.0.3.post491.dist-info/zip-safe
 Comment: 
 
-Filename: nucliadb_utils-3.0.3.post490.dist-info/RECORD
+Filename: nucliadb_utils-3.0.3.post491.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `nucliadb_utils-3.0.3.post490.dist-info/METADATA` & `nucliadb_utils-3.0.3.post491.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nucliadb-utils
-Version: 3.0.3.post490
+Version: 3.0.3.post491
 Home-page: https://nuclia.com
 License: BSD
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -17,16 +17,16 @@
 Requires-Dist: prometheus-client >=0.12.0
 Requires-Dist: types-requests >=2.27.7
 Requires-Dist: mmh3 >=3.0.0
 Requires-Dist: nats-py[nkeys] >=2.6.0
 Requires-Dist: pyjwt >=2.4.0
 Requires-Dist: memorylru >=1.1.2
 Requires-Dist: mrflagly
-Requires-Dist: nucliadb-protos >=3.0.3.post490
-Requires-Dist: nucliadb-telemetry >=3.0.3.post490
+Requires-Dist: nucliadb-protos >=3.0.3.post491
+Requires-Dist: nucliadb-telemetry >=3.0.3.post491
 Provides-Extra: cache
 Requires-Dist: redis >=4.3.4 ; extra == 'cache'
 Requires-Dist: orjson >=3.6.7 ; extra == 'cache'
 Requires-Dist: lru-dict >=1.1.7 ; extra == 'cache'
 Provides-Extra: fastapi
 Requires-Dist: fastapi >=0.95.2 ; extra == 'fastapi'
 Requires-Dist: uvicorn <0.19.0,>=0.16.0 ; extra == 'fastapi'
```

## Comparing `nucliadb_utils-3.0.3.post490.dist-info/RECORD` & `nucliadb_utils-3.0.3.post491.dist-info/RECORD`

 * *Files 2% similar despite different names*

```diff
@@ -59,12 +59,12 @@
 nucliadb_utils/tests/unit/test_transaction.py,sha256=ULVALWbMWEkH2Gq5Q8olEL8k8Kqyh5RAe0Lp9qdF1V4,3917
 nucliadb_utils/tests/unit/test_utilities.py,sha256=uzSFm7HzHGU-PS4-dqjFQxyxgypNAvwKEm0PtBg6Wmg,5099
 nucliadb_utils/tests/unit/storages/__init__.py,sha256=itSI7dtTwFP55YMX4iK7JzdMHS5CQVUiB1XzQu4UBh8,833
 nucliadb_utils/tests/unit/storages/test_aws.py,sha256=GCsB_jwCUNV3Ogt8TZZEmNKAHvOlR0HGU7blrFbtJqs,1924
 nucliadb_utils/tests/unit/storages/test_gcs.py,sha256=2XzJwgNpfjVGjtE-QdZhu3ayuT1EMEXINdM-_SatPCY,3554
 nucliadb_utils/tests/unit/storages/test_pg.py,sha256=sJfUttMSzq8W1XYolAUcMxl_R5HcEzb5fpCklPeMJiY,17000
 nucliadb_utils/tests/unit/storages/test_storage.py,sha256=VFpRq6Q6BjnIrBQCumYzR8DQUacwhxt5CzTKSlqqD24,6892
-nucliadb_utils-3.0.3.post490.dist-info/METADATA,sha256=opoq8dn2HQJqp7kifA99BMZ-ON-p3NvC_znzEAzhwoM,1975
-nucliadb_utils-3.0.3.post490.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-nucliadb_utils-3.0.3.post490.dist-info/top_level.txt,sha256=fE3vJtALTfgh7bcAWcNhcfXkNPp_eVVpbKK-2IYua3E,15
-nucliadb_utils-3.0.3.post490.dist-info/zip-safe,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
-nucliadb_utils-3.0.3.post490.dist-info/RECORD,,
+nucliadb_utils-3.0.3.post491.dist-info/METADATA,sha256=BzEt-_BQy3dPsVK1cvwvjwRZT3OQcpcEpwPrJilRObw,1975
+nucliadb_utils-3.0.3.post491.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+nucliadb_utils-3.0.3.post491.dist-info/top_level.txt,sha256=fE3vJtALTfgh7bcAWcNhcfXkNPp_eVVpbKK-2IYua3E,15
+nucliadb_utils-3.0.3.post491.dist-info/zip-safe,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
+nucliadb_utils-3.0.3.post491.dist-info/RECORD,,
```

