# Comparing `tmp/fsspec_dnanexus-0.2.3-py3-none-any.whl.zip` & `tmp/fsspec_dnanexus-0.2.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,20 @@
-Zip file size: 22149 bytes, number of entries: 14
--rw-r--r--  2.0 unx     1960 b- defN 23-Dec-07 13:10 fsspec_dnanexus/__init__.py
--rw-r--r--  2.0 unx    31105 b- defN 23-Dec-07 13:07 fsspec_dnanexus/core.py
--rw-r--r--  2.0 unx      535 b- defN 23-Dec-07 13:07 fsspec_dnanexus/utils.py
--rw-r--r--  2.0 unx        0 b- defN 23-Dec-07 13:07 fsspec_dnanexus/factories/__init__.py
--rw-r--r--  2.0 unx     9866 b- defN 23-Dec-07 13:07 fsspec_dnanexus/factories/dxdispatchers.py
--rw-r--r--  2.0 unx     1980 b- defN 23-Dec-07 13:07 fsspec_dnanexus/factories/dxfactory.py
--rw-r--r--  2.0 unx      347 b- defN 23-Dec-07 13:07 fsspec_dnanexus/factories/dxpandas_on_python.py
--rw-r--r--  2.0 unx    11113 b- defN 23-Dec-07 13:07 fsspec_dnanexus/factories/dxpandas_on_ray.py
--rw-r--r--  2.0 unx     1064 b- defN 23-Dec-07 13:16 fsspec_dnanexus-0.2.3.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx     7732 b- defN 23-Dec-07 13:16 fsspec_dnanexus-0.2.3.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Dec-07 13:16 fsspec_dnanexus-0.2.3.dist-info/WHEEL
--rw-r--r--  2.0 unx       55 b- defN 23-Dec-07 13:16 fsspec_dnanexus-0.2.3.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       16 b- defN 23-Dec-07 13:16 fsspec_dnanexus-0.2.3.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1268 b- defN 23-Dec-07 13:16 fsspec_dnanexus-0.2.3.dist-info/RECORD
-14 files, 67133 bytes uncompressed, 19997 bytes compressed:  70.2%
+Zip file size: 29620 bytes, number of entries: 18
+-rw-r--r--  2.0 unx     1960 b- defN 24-May-10 08:00 fsspec_dnanexus/__init__.py
+-rw-r--r--  2.0 unx    31105 b- defN 24-May-10 07:59 fsspec_dnanexus/core.py
+-rw-r--r--  2.0 unx    21901 b- defN 23-Aug-08 08:02 fsspec_dnanexus/dxfactory.py
+-rw-r--r--  2.0 unx      535 b- defN 23-Oct-03 15:17 fsspec_dnanexus/utils.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Sep-14 05:19 fsspec_dnanexus/factories/__init__.py
+-rw-r--r--  2.0 unx     9866 b- defN 24-May-10 07:59 fsspec_dnanexus/factories/dxdispatchers.py
+-rw-r--r--  2.0 unx     1980 b- defN 23-Sep-14 05:19 fsspec_dnanexus/factories/dxfactory.py
+-rw-r--r--  2.0 unx      347 b- defN 23-Sep-14 05:19 fsspec_dnanexus/factories/dxpandas_on_python.py
+-rw-r--r--  2.0 unx    11113 b- defN 23-Sep-14 05:19 fsspec_dnanexus/factories/dxpandas_on_ray.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Aug-15 08:25 tests/__init__.py
+-rw-r--r--  2.0 unx      971 b- defN 23-Sep-14 05:19 tests/conftest.py
+-rw-r--r--  2.0 unx     6932 b- defN 23-Sep-14 05:19 tests/testutils.py
+-rw-r--r--  2.0 unx     1064 b- defN 24-May-10 10:50 fsspec_dnanexus-0.2.4.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx     7795 b- defN 24-May-10 10:50 fsspec_dnanexus-0.2.4.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-10 10:50 fsspec_dnanexus-0.2.4.dist-info/WHEEL
+-rw-r--r--  2.0 unx       55 b- defN 24-May-10 10:50 fsspec_dnanexus-0.2.4.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       22 b- defN 24-May-10 10:50 fsspec_dnanexus-0.2.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1573 b- defN 24-May-10 10:50 fsspec_dnanexus-0.2.4.dist-info/RECORD
+18 files, 97311 bytes uncompressed, 27004 bytes compressed:  72.2%
```

## zipnote {}

```diff
@@ -1,13 +1,16 @@
 Filename: fsspec_dnanexus/__init__.py
 Comment: 
 
 Filename: fsspec_dnanexus/core.py
 Comment: 
 
+Filename: fsspec_dnanexus/dxfactory.py
+Comment: 
+
 Filename: fsspec_dnanexus/utils.py
 Comment: 
 
 Filename: fsspec_dnanexus/factories/__init__.py
 Comment: 
 
 Filename: fsspec_dnanexus/factories/dxdispatchers.py
@@ -18,26 +21,35 @@
 
 Filename: fsspec_dnanexus/factories/dxpandas_on_python.py
 Comment: 
 
 Filename: fsspec_dnanexus/factories/dxpandas_on_ray.py
 Comment: 
 
-Filename: fsspec_dnanexus-0.2.3.dist-info/LICENSE.txt
+Filename: tests/__init__.py
+Comment: 
+
+Filename: tests/conftest.py
+Comment: 
+
+Filename: tests/testutils.py
+Comment: 
+
+Filename: fsspec_dnanexus-0.2.4.dist-info/LICENSE.txt
 Comment: 
 
-Filename: fsspec_dnanexus-0.2.3.dist-info/METADATA
+Filename: fsspec_dnanexus-0.2.4.dist-info/METADATA
 Comment: 
 
-Filename: fsspec_dnanexus-0.2.3.dist-info/WHEEL
+Filename: fsspec_dnanexus-0.2.4.dist-info/WHEEL
 Comment: 
 
-Filename: fsspec_dnanexus-0.2.3.dist-info/entry_points.txt
+Filename: fsspec_dnanexus-0.2.4.dist-info/entry_points.txt
 Comment: 
 
-Filename: fsspec_dnanexus-0.2.3.dist-info/top_level.txt
+Filename: fsspec_dnanexus-0.2.4.dist-info/top_level.txt
 Comment: 
 
-Filename: fsspec_dnanexus-0.2.3.dist-info/RECORD
+Filename: fsspec_dnanexus-0.2.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## fsspec_dnanexus/__init__.py

```diff
@@ -6,15 +6,15 @@
                 DXPathExtractor, \
                 DXBufferedFileOnRay, \
                 DXBufferedFile, \
                 logger
 
 from .factories import dxfactory
 
-__version__ = "0.2.3"
+__version__ = "0.2.4"
 
 def init_for_modin_on_ray(n_partitions: int = None):
     def init_ray_cluster() -> None:
         import ray._private.services as services
         
         dx_job_id = os.environ.get('DX_JOB_ID')
         try:
```

## Comparing `fsspec_dnanexus-0.2.3.dist-info/LICENSE.txt` & `fsspec_dnanexus-0.2.4.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `fsspec_dnanexus-0.2.3.dist-info/METADATA` & `fsspec_dnanexus-0.2.4.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: fsspec-dnanexus
-Version: 0.2.3
+Version: 0.2.4
 Summary: fsspec backend for the DNAnexus platform
 Maintainer: DNAnexus-xVantage
 Maintainer-email: tphan@dnanexus.com
 License: MIT
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
-Requires-Dist: dxpy (==0.363.0)
-Requires-Dist: fsspec (==2023.9.2)
-Requires-Dist: botocore (<1.32.0,>=1.31.53)
+Requires-Dist: dxpy ==0.363.0
+Requires-Dist: fsspec ==2024.3.1
+Requires-Dist: botocore <1.34.70,>=1.34.41
 
 # fsspec_dnanexus
 [fsspec backend](https://filesystem-spec.readthedocs.io/en/latest/) for [DNAnexus](https://dnanexus.com)
 
 
 ## Installation
 
@@ -160,14 +160,17 @@
     os.environ["FSSPEC_DNANEXUS_LOGGING_LEVEL"] = "DEBUG"
 
 Valid logging levels are listed here: https://docs.python.org/3/library/logging.html#levels
 
 
 ## Changelog
 
+#### 0.2.4 (2024-05-10)
+* Fixed: Dependencies conflicted with s3fs
+
 #### 0.2.3 (2023-12-07)
 * Fixed: reading and writing hidden files
 
 #### 0.2.2 (2023-11-15)
 * Fixed: using modin 0.24 no longer resulted in single node reads
 * Fixed: resolved package conflicts
```

## Comparing `fsspec_dnanexus-0.2.3.dist-info/RECORD` & `fsspec_dnanexus-0.2.4.dist-info/RECORD`

 * *Files 21% similar despite different names*

```diff
@@ -1,14 +1,18 @@
-fsspec_dnanexus/__init__.py,sha256=MjYEkNdRp_WhZ3oV-HgRUhfu6QyQNH1ZtVS959YZfzU,1960
+fsspec_dnanexus/__init__.py,sha256=vvAiForSBceUNTjbz3HB6-dEE6NT-ZJ7ZZt-FQNVaIE,1960
 fsspec_dnanexus/core.py,sha256=_WNFM6W1W4avNEfWw_98Ugluaim7n24MHk5dZOoOuMg,31105
+fsspec_dnanexus/dxfactory.py,sha256=8yBF1uHhG9AmmxxVrwba10P-8LcfjhFiIAreXvxqVt8,21901
 fsspec_dnanexus/utils.py,sha256=byZVNTAGQTw3pJNU8RtJoQYuX1iYSt1m7j29NgpFD5U,535
 fsspec_dnanexus/factories/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 fsspec_dnanexus/factories/dxdispatchers.py,sha256=XBWUKiK33Da3Bv6WRwhrQBBdadXaVYP1GKtBXc4Zt60,9866
 fsspec_dnanexus/factories/dxfactory.py,sha256=vnE3FUQqNXMBaGlmi0btkBycNQ4O_6sjuuzykxzQf1U,1980
 fsspec_dnanexus/factories/dxpandas_on_python.py,sha256=4oJo3NxGmCVVrXVSVSRTmjA_fzpBG06IPb9nYGTgoAk,347
 fsspec_dnanexus/factories/dxpandas_on_ray.py,sha256=v6yr6zYGny0C4pg8x0yxMyqM9CVbDIEhEmQ6r2XwEPQ,11113
-fsspec_dnanexus-0.2.3.dist-info/LICENSE.txt,sha256=xw5rRrmGcck7yjci2gFi_mdLQMqoJ4z_wj9V-v1f8kc,1064
-fsspec_dnanexus-0.2.3.dist-info/METADATA,sha256=b7qKZickOVKkR2AX4ihijP4NphgI06uaihqAuiIwgZo,7732
-fsspec_dnanexus-0.2.3.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-fsspec_dnanexus-0.2.3.dist-info/entry_points.txt,sha256=zedbecJMg3jDda3NJosZuAeXyQcyvjjtxoPOUzaxvpA,55
-fsspec_dnanexus-0.2.3.dist-info/top_level.txt,sha256=fhiQuqx3PFbiSpzgyHwTk5k8oC2um96uzf3YTKNwpIE,16
-fsspec_dnanexus-0.2.3.dist-info/RECORD,,
+tests/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+tests/conftest.py,sha256=F7C8gCc4VqFy2ztd8LX6iunLWsI_HFf9waSe_he7ezI,971
+tests/testutils.py,sha256=rWIRDkiLi1AS9TmkJbsg-ja9saO7VY6sv7676Bx6vzY,6932
+fsspec_dnanexus-0.2.4.dist-info/LICENSE.txt,sha256=xw5rRrmGcck7yjci2gFi_mdLQMqoJ4z_wj9V-v1f8kc,1064
+fsspec_dnanexus-0.2.4.dist-info/METADATA,sha256=xG6gXdapHNVdSz5R42po2X3_5SByEaWx2PbsjiQukhs,7795
+fsspec_dnanexus-0.2.4.dist-info/WHEEL,sha256=yQN5g4mg4AybRjkgi-9yy4iQEFibGQmlz78Pik5Or-A,92
+fsspec_dnanexus-0.2.4.dist-info/entry_points.txt,sha256=zedbecJMg3jDda3NJosZuAeXyQcyvjjtxoPOUzaxvpA,55
+fsspec_dnanexus-0.2.4.dist-info/top_level.txt,sha256=opvw21JKM4ouM--vSpw9SVxLEeIg4M3Cxovw6vlvPzg,22
+fsspec_dnanexus-0.2.4.dist-info/RECORD,,
```

