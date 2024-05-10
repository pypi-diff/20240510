# Comparing `tmp/dwclib-2024.4.4.tar.gz` & `tmp/dwclib-2024.5.10.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dwclib-2024.4.4.tar", max compression
+gzip compressed data, was "dwclib-2024.5.10.tar", max compression
```

## Comparing `dwclib-2024.4.4.tar` & `dwclib-2024.5.10.tar`

### file list

```diff
@@ -1,27 +1,57 @@
--rw-r--r--   0        0        0      753 2022-06-09 12:54:18.472933 dwclib-2024.4.4/LICENSE
--rw-r--r--   0        0        0     1679 2024-04-04 20:35:20.780494 dwclib-2024.4.4/README.md
--rw-r--r--   0        0        0      737 2024-04-04 20:31:28.610432 dwclib-2024.4.4/pyproject.toml
--rw-r--r--   0        0        0      508 2023-10-15 18:21:30.585978 dwclib-2024.4.4/src/dwclib/__init__.py
--rw-r--r--   0        0        0       59 2023-06-19 11:43:33.517768 dwclib-2024.4.4/src/dwclib/alerts/__init__.py
--rw-r--r--   0        0        0     2636 2024-04-04 20:36:22.769018 dwclib-2024.4.4/src/dwclib/alerts/alerts.py
--rw-r--r--   0        0        0        0 2023-06-19 11:43:33.517768 dwclib-2024.4.4/src/dwclib/assets/__init__.py
--rw-r--r--   0        0        0   173360 2023-06-19 11:43:33.517768 dwclib-2024.4.4/src/dwclib/assets/alert_ref.csv
--rw-r--r--   0        0        0     1346 2023-06-20 11:00:59.901656 dwclib-2024.4.4/src/dwclib/common/db.py
--rw-r--r--   0        0        0     1315 2023-10-15 18:14:41.791832 dwclib-2024.4.4/src/dwclib/common/meta.py
--rw-r--r--   0        0        0     2197 2024-04-04 20:21:52.604945 dwclib-2024.4.4/src/dwclib/common/numerics.py
--rw-r--r--   0        0        0     1298 2023-06-20 14:18:49.043435 dwclib-2024.4.4/src/dwclib/common/wave_unfold.py
--rw-r--r--   0        0        0     2060 2024-04-04 20:22:17.465118 dwclib-2024.4.4/src/dwclib/common/waves.py
--rw-r--r--   0        0        0      153 2023-06-19 11:43:33.517768 dwclib-2024.4.4/src/dwclib/dask/__init__.py
--rw-r--r--   0        0        0      981 2024-01-13 15:37:07.253914 dwclib-2024.4.4/src/dwclib/dask/generic.py
--rw-r--r--   0        0        0      791 2023-06-20 14:21:34.423133 dwclib-2024.4.4/src/dwclib/dask/numerics.py
--rw-r--r--   0        0        0      788 2023-06-20 14:21:42.655119 dwclib-2024.4.4/src/dwclib/dask/waves.py
--rw-r--r--   0        0        0     1419 2023-06-19 11:43:33.517768 dwclib-2024.4.4/src/dwclib/dask/waves_convert.py
--rw-r--r--   0        0        0       77 2023-10-15 18:21:07.681856 dwclib-2024.4.4/src/dwclib/enumerations/__init__.py
--rw-r--r--   0        0        0     3214 2024-04-04 20:28:55.460956 dwclib-2024.4.4/src/dwclib/enumerations/enumerations.py
--rw-r--r--   0        0        0       65 2023-06-19 11:43:33.517768 dwclib-2024.4.4/src/dwclib/numerics/__init__.py
--rw-r--r--   0        0        0     1530 2023-10-15 18:28:14.976170 dwclib-2024.4.4/src/dwclib/numerics/numerics.py
--rw-r--r--   0        0        0       95 2023-06-19 11:43:33.517768 dwclib-2024.4.4/src/dwclib/patients/__init__.py
--rw-r--r--   0        0        0     5350 2024-04-04 20:25:50.818998 dwclib-2024.4.4/src/dwclib/patients/patients.py
--rw-r--r--   0        0        0       56 2023-06-19 11:43:33.517768 dwclib-2024.4.4/src/dwclib/waves/__init__.py
--rw-r--r--   0        0        0     1365 2023-08-18 09:13:01.184641 dwclib-2024.4.4/src/dwclib/waves/waves.py
--rw-r--r--   0        0        0     2478 1970-01-01 00:00:00.000000 dwclib-2024.4.4/PKG-INFO
+-rw-r--r--   0        0        0      753 2022-06-09 12:54:18.472933 dwclib-2024.5.10/LICENSE
+-rw-r--r--   0        0        0     1757 2024-05-10 16:09:07.955034 dwclib-2024.5.10/README.md
+-rw-r--r--   0        0        0      738 2024-05-10 16:09:21.267201 dwclib-2024.5.10/pyproject.toml
+-rw-r--r--   0        0        0      508 2023-10-15 18:21:30.585978 dwclib-2024.5.10/src/dwclib/__init__.py
+-rw-r--r--   0        0        0       59 2023-06-19 11:43:33.517768 dwclib-2024.5.10/src/dwclib/alerts/__init__.py
+-rw-r--r--   0        0        0      209 2023-03-03 14:53:03.991353 dwclib-2024.5.10/src/dwclib/alerts/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      242 2024-04-04 20:13:00.428806 dwclib-2024.5.10/src/dwclib/alerts/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     2713 2023-03-03 15:13:33.244081 dwclib-2024.5.10/src/dwclib/alerts/__pycache__/alerts.cpython-310.pyc
+-rw-r--r--   0        0        0     5319 2024-04-29 13:05:36.551103 dwclib-2024.5.10/src/dwclib/alerts/__pycache__/alerts.cpython-311.pyc
+-rw-r--r--   0        0        0     2565 2024-04-29 13:05:13.790584 dwclib-2024.5.10/src/dwclib/alerts/alerts.py
+-rw-r--r--   0        0        0        0 2023-06-19 11:43:33.517768 dwclib-2024.5.10/src/dwclib/assets/__init__.py
+-rw-r--r--   0        0        0      145 2023-03-03 14:53:04.279357 dwclib-2024.5.10/src/dwclib/assets/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      161 2024-04-04 20:13:00.780810 dwclib-2024.5.10/src/dwclib/assets/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0   173360 2023-06-19 11:43:33.517768 dwclib-2024.5.10/src/dwclib/assets/alert_ref.csv
+-rw-r--r--   0        0        0     1283 2023-03-03 14:53:04.279357 dwclib-2024.5.10/src/dwclib/common/__pycache__/db.cpython-310.pyc
+-rw-r--r--   0        0        0     2184 2024-04-04 20:13:00.780810 dwclib-2024.5.10/src/dwclib/common/__pycache__/db.cpython-311.pyc
+-rw-r--r--   0        0        0     1336 2023-03-03 14:53:04.283357 dwclib-2024.5.10/src/dwclib/common/__pycache__/meta.cpython-310.pyc
+-rw-r--r--   0        0        0     2620 2024-04-04 20:24:27.362030 dwclib-2024.5.10/src/dwclib/common/__pycache__/meta.cpython-311.pyc
+-rw-r--r--   0        0        0     2139 2023-03-03 14:53:04.479359 dwclib-2024.5.10/src/dwclib/common/__pycache__/numerics.cpython-310.pyc
+-rw-r--r--   0        0        0     4582 2024-04-29 13:02:34.619014 dwclib-2024.5.10/src/dwclib/common/__pycache__/numerics.cpython-311.pyc
+-rw-r--r--   0        0        0     1576 2023-03-03 14:53:04.483359 dwclib-2024.5.10/src/dwclib/common/__pycache__/wave_unfold.cpython-310.pyc
+-rw-r--r--   0        0        0     2684 2024-04-04 20:24:27.566032 dwclib-2024.5.10/src/dwclib/common/__pycache__/wave_unfold.cpython-311.pyc
+-rw-r--r--   0        0        0     1927 2023-03-03 14:53:04.791363 dwclib-2024.5.10/src/dwclib/common/__pycache__/waves.cpython-310.pyc
+-rw-r--r--   0        0        0     4313 2024-04-29 13:02:34.623014 dwclib-2024.5.10/src/dwclib/common/__pycache__/waves.cpython-311.pyc
+-rw-r--r--   0        0        0     1346 2023-06-20 11:00:59.901656 dwclib-2024.5.10/src/dwclib/common/db.py
+-rw-r--r--   0        0        0     1315 2023-10-15 18:14:41.791832 dwclib-2024.5.10/src/dwclib/common/meta.py
+-rw-r--r--   0        0        0     2134 2024-04-08 20:16:14.250281 dwclib-2024.5.10/src/dwclib/common/numerics.py
+-rw-r--r--   0        0        0     1298 2023-06-20 14:18:49.043435 dwclib-2024.5.10/src/dwclib/common/wave_unfold.py
+-rw-r--r--   0        0        0     1999 2024-04-08 20:16:29.258575 dwclib-2024.5.10/src/dwclib/common/waves.py
+-rw-r--r--   0        0        0      153 2023-06-19 11:43:33.517768 dwclib-2024.5.10/src/dwclib/dask/__init__.py
+-rw-r--r--   0        0        0      981 2024-01-13 15:37:07.253914 dwclib-2024.5.10/src/dwclib/dask/generic.py
+-rw-r--r--   0        0        0      791 2023-06-20 14:21:34.423133 dwclib-2024.5.10/src/dwclib/dask/numerics.py
+-rw-r--r--   0        0        0      788 2023-06-20 14:21:42.655119 dwclib-2024.5.10/src/dwclib/dask/waves.py
+-rw-r--r--   0        0        0     1419 2023-06-19 11:43:33.517768 dwclib-2024.5.10/src/dwclib/dask/waves_convert.py
+-rw-r--r--   0        0        0       77 2023-10-15 18:21:07.681856 dwclib-2024.5.10/src/dwclib/enumerations/__init__.py
+-rw-r--r--   0        0        0      261 2024-04-04 20:24:27.362030 dwclib-2024.5.10/src/dwclib/enumerations/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     6006 2024-04-29 13:02:34.331007 dwclib-2024.5.10/src/dwclib/enumerations/__pycache__/enumerations.cpython-311.pyc
+-rw-r--r--   0        0        0     3113 2024-04-08 20:16:52.419020 dwclib-2024.5.10/src/dwclib/enumerations/enumerations.py
+-rw-r--r--   0        0        0       65 2023-06-19 11:43:33.517768 dwclib-2024.5.10/src/dwclib/numerics/__init__.py
+-rw-r--r--   0        0        0      215 2023-03-03 14:53:04.283357 dwclib-2024.5.10/src/dwclib/numerics/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      249 2024-04-04 20:24:27.562032 dwclib-2024.5.10/src/dwclib/numerics/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     1459 2023-03-03 14:53:04.283357 dwclib-2024.5.10/src/dwclib/numerics/__pycache__/numerics.cpython-310.pyc
+-rw-r--r--   0        0        0     2359 2024-04-04 20:24:27.562032 dwclib-2024.5.10/src/dwclib/numerics/__pycache__/numerics.cpython-311.pyc
+-rw-r--r--   0        0        0     1530 2023-10-15 18:28:14.976170 dwclib-2024.5.10/src/dwclib/numerics/numerics.py
+-rw-r--r--   0        0        0      149 2024-05-10 15:54:29.155738 dwclib-2024.5.10/src/dwclib/patients/__init__.py
+-rw-r--r--   0        0        0      245 2023-03-03 14:53:04.479359 dwclib-2024.5.10/src/dwclib/patients/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      319 2024-05-10 15:54:35.407797 dwclib-2024.5.10/src/dwclib/patients/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     3395 2023-03-03 14:53:04.483359 dwclib-2024.5.10/src/dwclib/patients/__pycache__/patients.cpython-310.pyc
+-rw-r--r--   0        0        0    11202 2024-05-10 15:58:12.541860 dwclib-2024.5.10/src/dwclib/patients/__pycache__/patients.cpython-311.pyc
+-rw-r--r--   0        0        0     7641 2024-05-10 16:08:19.246414 dwclib-2024.5.10/src/dwclib/patients/patients.py
+-rw-r--r--   0        0        0       56 2023-06-19 11:43:33.517768 dwclib-2024.5.10/src/dwclib/waves/__init__.py
+-rw-r--r--   0        0        0      206 2023-03-03 14:53:04.483359 dwclib-2024.5.10/src/dwclib/waves/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      239 2024-04-04 20:24:27.566032 dwclib-2024.5.10/src/dwclib/waves/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     1722 2023-03-03 14:53:04.483359 dwclib-2024.5.10/src/dwclib/waves/__pycache__/waves.cpython-310.pyc
+-rw-r--r--   0        0        0     2938 2024-04-04 20:24:27.566032 dwclib-2024.5.10/src/dwclib/waves/__pycache__/waves.cpython-311.pyc
+-rw-r--r--   0        0        0     1365 2023-08-18 09:13:01.184641 dwclib-2024.5.10/src/dwclib/waves/waves.py
+-rw-r--r--   0        0        0     2557 1970-01-01 00:00:00.000000 dwclib-2024.5.10/PKG-INFO
```

### Comparing `dwclib-2024.4.4/LICENSE` & `dwclib-2024.5.10/LICENSE`

 * *Files identical despite different names*

### Comparing `dwclib-2024.4.4/README.md` & `dwclib-2024.5.10/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -10,14 +10,17 @@
 Installation through conda greatly simplifies dependency management.
 
 Additionally, Microsoft SQL Server drivers are needed and will need to be installed seperately.
 See here for more information: https://github.com/mkleehammer/pyodbc/wiki
 
 
 ## Changelog
+- 2024.5.10
+    - Support searching patients directly in DWC without DWCmeta
+
 - 2024.4.4
     - Support querying enumerations
     - Update dependencies
 
 - 2023.6.21
     - Remove all occurences of naive datetime since dask now support tz-aware
     - New config file syntax to be compatible with other libraries
```

### Comparing `dwclib-2024.4.4/pyproject.toml` & `dwclib-2024.5.10/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "dwclib"
-version = "2024.4.4"
+version = "2024.5.10"
 description = "Python wrapper to DataWarehouse Connect"
 authors = ["Jona Joachim <jona@joachim.cc>"]
 license = "ISC"
 readme = "README.md"
 repository = "https://github.com/larib-data/dwclib"
 
 [tool.poetry.dependencies]
```

### Comparing `dwclib-2024.4.4/src/dwclib/alerts/alerts.py` & `dwclib-2024.5.10/src/dwclib/alerts/alerts.py`

 * *Files 12% similar despite different names*

```diff
@@ -31,30 +31,28 @@
     dtend: Union[str, datetime],
     patientids: Union[None, str, List[str]],
 ) -> pd.DataFrame:
     engine = create_engine(uri)
     q = build_alerts_query(engine, dtbegin, dtend, patientids)
 
     with engine.connect() as conn:
-        df = pd.read_sql(q, conn, index_col="AlertId")
+        df = pd.read_sql(q, conn, index_col="begin")
     engine.dispose()
 
     metadf = load_alerts_meta()
     metadf = metadf[["source_label", "mdc_alert", "alert_kind", "severity"]]
     dfr = df.join(metadf, on=["Source", "Code"])
     return dfr.drop(columns=["Source", "Code"])
 
 
 def build_alerts_query(engine, dtbegin, dtend, patientids):
     dbmeta = MetaData(schema="_Export")
-    dbmeta.reflect(bind=engine)
-    at = Table("Alert_", dbmeta, autoload=True, autoload_with=engine)
+    at = Table("Alert_", dbmeta, autoload_with=engine)
 
     aq = select(
-        at.c.AlertId,
         func.min(at.c.TimeStamp).label("begin"),
         func.max(at.c.TimeStamp).label("end"),
         func.max(at.c.Source).label("Source"),
         func.max(at.c.Code).label("Code"),
         func.max(at.c.Label).label("alert_label"),
     )
     aq = aq.with_hint(at, "WITH (NOLOCK)")
```

### Comparing `dwclib-2024.4.4/src/dwclib/assets/alert_ref.csv` & `dwclib-2024.5.10/src/dwclib/assets/alert_ref.csv`

 * *Files identical despite different names*

### Comparing `dwclib-2024.4.4/src/dwclib/common/db.py` & `dwclib-2024.5.10/src/dwclib/common/db.py`

 * *Files identical despite different names*

### Comparing `dwclib-2024.4.4/src/dwclib/common/meta.py` & `dwclib-2024.5.10/src/dwclib/common/meta.py`

 * *Files identical despite different names*

### Comparing `dwclib-2024.4.4/src/dwclib/common/numerics.py` & `dwclib-2024.5.10/src/dwclib/common/numerics.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,64 +1,62 @@
 from datetime import datetime
 from typing import List, Union
 
 import pandas as pd
+from dwclib.common.meta import numerics_meta
 from pandas.api.types import is_list_like
 from sqlalchemy import MetaData, Table, create_engine, join, select
 
-from dwclib.common.meta import numerics_meta
-
 
 def run_numerics_query(
     uri: str,
     dtbegin: Union[str, datetime],
     dtend: Union[str, datetime],
     patientids: Union[None, str, List[str]],
     labels: List[str],
     sublabels: List[str],
 ) -> pd.DataFrame:
     engine = create_engine(uri)
     q = build_numerics_query(engine, dtbegin, dtend, patientids, labels, sublabels)
 
     with engine.connect() as conn:
-        df = pd.read_sql(q, conn, index_col='TimeStamp')
+        df = pd.read_sql(q, conn, index_col="TimeStamp")
     engine.dispose()
     if len(df) == 0:
         return numerics_meta
     else:
         df.index = pd.to_datetime(df.index, utc=True)
         return df.astype(numerics_meta.dtypes.to_dict(), copy=False)
 
 
 def build_numerics_query(engine, dtbegin, dtend, patientids, labels, sublabels):
-    dbmeta = MetaData(schema='_Export')
-    dbmeta.reflect(bind=engine)
-    nnt = Table('Numeric_', dbmeta, autoload=True, autoload_with=engine)
-    nvt = Table('NumericValue_', dbmeta, autoload=True, autoload_with=engine)
+    dbmeta = MetaData(schema="_Export")
+    nnt = Table("Numeric_", dbmeta, autoload_with=engine)
+    nvt = Table("NumericValue_", dbmeta, autoload_with=engine)
 
     nn = select(nnt.c.TimeStamp, nnt.c.Id, nnt.c.Label, nnt.c.SubLabel)
-    nn = nn.with_hint(nnt, 'WITH (NOLOCK)')
+    nn = nn.with_hint(nnt, "WITH (NOLOCK)")
     nn = nn.where(nnt.c.TimeStamp >= dtbegin)
     nn = nn.where(nnt.c.TimeStamp < dtend)
     if labels:
         nn = nn.where(nnt.c.Label.in_(labels))
     if sublabels:
         nn = nn.where(nnt.c.SubLabel.in_(sublabels))
-    nn = nn.cte('Numeric')
+    nn = nn.cte("Numeric")
 
     nv = select(nvt.c.TimeStamp, nvt.c.NumericId, nvt.c.Value, nvt.c.PatientId)
-    nv = nv.with_hint(nvt, 'WITH (NOLOCK)')
+    nv = nv.with_hint(nvt, "WITH (NOLOCK)")
     nv = nv.where(nvt.c.TimeStamp >= dtbegin)
     nv = nv.where(nvt.c.TimeStamp < dtend)
     nv = nv.where(nvt.c.Value.is_not(None))
     if patientids:
         if is_list_like(patientids):
             nv = nv.where(nvt.c.PatientId.in_(patientids))
         else:
             nv = nv.where(nvt.c.PatientId == patientids)
-    nv = nv.cte('NumericValue')
+    nv = nv.cte("NumericValue")
 
     j = join(nv, nn, nv.c.NumericId == nn.c.Id)
     q = select(
         nv.c.TimeStamp, nv.c.PatientId, nn.c.Label, nn.c.SubLabel, nv.c.Value
     ).select_from(j)
     return q
```

### Comparing `dwclib-2024.4.4/src/dwclib/common/wave_unfold.py` & `dwclib-2024.5.10/src/dwclib/common/wave_unfold.py`

 * *Files identical despite different names*

### Comparing `dwclib-2024.4.4/src/dwclib/common/waves.py` & `dwclib-2024.5.10/src/dwclib/common/waves.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,57 +1,57 @@
 import pandas as pd
-from dwclib.common.meta import waves_meta
 from sqlalchemy import MetaData, Table, create_engine, join, select
 
+from dwclib.common.meta import waves_meta
+
 
 def run_waves_query(uri, dtbegin, dtend, patientid, labels):
     engine = create_engine(uri)
     q = build_waves_query(engine, dtbegin, dtend, patientid, labels)
 
     with engine.connect() as conn:
-        df = pd.read_sql(q, conn, index_col='TimeStamp')
+        df = pd.read_sql(q, conn, index_col="TimeStamp")
     engine.dispose()
     if len(df) == 0:
         return waves_meta
     else:
         df.index = pd.to_datetime(df.index, utc=True)
         return df.astype(waves_meta.dtypes.to_dict(), copy=False)
 
 
 def build_waves_query(engine, dtbegin, dtend, patientid, labels):
-    dbmeta = MetaData(schema='_Export')
-    dbmeta.reflect(bind=engine)
-    wwt = Table('Wave_', dbmeta, autoload=True, autoload_with=engine)
-    wst = Table('WaveSample_', dbmeta, autoload=True, autoload_with=engine)
+    dbmeta = MetaData(schema="_Export")
+    wwt = Table("Wave_", dbmeta, autoload_with=engine)
+    wst = Table("WaveSample_", dbmeta, autoload_with=engine)
 
     ww = select(
         wwt.c.TimeStamp,
         wwt.c.Id,
         wwt.c.Label,
         wwt.c.SamplePeriod,
-        wwt.c.CalibrationAbsUpper.label('CAU'),
-        wwt.c.CalibrationAbsLower.label('CAL'),
-        wwt.c.CalibrationScaledUpper.label('CSU'),
-        wwt.c.CalibrationScaledLower.label('CSL'),
+        wwt.c.CalibrationAbsUpper.label("CAU"),
+        wwt.c.CalibrationAbsLower.label("CAL"),
+        wwt.c.CalibrationScaledUpper.label("CSU"),
+        wwt.c.CalibrationScaledLower.label("CSL"),
     )
-    ww = ww.with_hint(wwt, 'WITH (NOLOCK)')
+    ww = ww.with_hint(wwt, "WITH (NOLOCK)")
     ww = ww.where(wwt.c.TimeStamp >= dtbegin)
     ww = ww.where(wwt.c.TimeStamp < dtend)
     if labels:
         ww = ww.where(wwt.c.Label.in_(labels))
-    ww = ww.cte('Wave')
+    ww = ww.cte("Wave")
 
     ws = select(wst.c.TimeStamp, wst.c.WaveId, wst.c.WaveSamples, wst.c.PatientId)
-    ws = ws.with_hint(wst, 'WITH (NOLOCK)')
+    ws = ws.with_hint(wst, "WITH (NOLOCK)")
     ws = ws.where(wst.c.TimeStamp >= dtbegin)
     ws = ws.where(wst.c.TimeStamp < dtend)
     ws = ws.where(wst.c.WaveSamples.is_not(None))
     if patientid:
         ws = ws.where(wst.c.PatientId == patientid)
-    ws = ws.cte('WaveSample')
+    ws = ws.cte("WaveSample")
 
     j = join(ws, ww, ws.c.WaveId == ww.c.Id)
     q = select(
         ws.c.TimeStamp,
         ws.c.PatientId,
         ww.c.Label,
         ws.c.WaveSamples,
```

### Comparing `dwclib-2024.4.4/src/dwclib/dask/generic.py` & `dwclib-2024.5.10/src/dwclib/dask/generic.py`

 * *Files identical despite different names*

### Comparing `dwclib-2024.4.4/src/dwclib/dask/numerics.py` & `dwclib-2024.5.10/src/dwclib/dask/numerics.py`

 * *Files identical despite different names*

### Comparing `dwclib-2024.4.4/src/dwclib/dask/waves.py` & `dwclib-2024.5.10/src/dwclib/dask/waves.py`

 * *Files identical despite different names*

### Comparing `dwclib-2024.4.4/src/dwclib/dask/waves_convert.py` & `dwclib-2024.5.10/src/dwclib/dask/waves_convert.py`

 * *Files identical despite different names*

### Comparing `dwclib-2024.4.4/src/dwclib/enumerations/enumerations.py` & `dwclib-2024.5.10/src/dwclib/enumerations/enumerations.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,31 +20,31 @@
     if not uri:
         uri = dwcuri
     if labels is None:
         labels = []
     if is_list_like(patientids) and len(patientids) == 1:
         patientids = patientids[0]
     df = run_enumerations_query(uri, dtbegin, dtend, patientids, labels)
-    df = df.dropna(axis=0, how='any', subset=['Value'])
+    df = df.dropna(axis=0, how="any", subset=["Value"])
     if not len(df.index):
         return enumerations_meta
     if pivot:
         df = pivot_enumerations(df)
     single_patient = patientids is not None and not is_list_like(patientids)
     if single_patient:
         df.columns = df.columns.droplevel(0)
     return df
 
 
 def pivot_enumerations(df: pd.DataFrame) -> Optional[pd.DataFrame]:
     df = df.pivot_table(
         index=df.index,
-        columns=['PatientId', 'Label'],
-        values='Value',
-        aggfunc='max',
+        columns=["PatientId", "Label"],
+        values="Value",
+        aggfunc="max",
     )
     return df
 
 
 def run_enumerations_query(
     uri: str,
     dtbegin: Union[str, datetime],
@@ -52,50 +52,44 @@
     patientids: Union[None, str, List[str]],
     labels: List[str],
 ) -> pd.DataFrame:
     engine = create_engine(uri)
     q = build_enumerations_query(engine, dtbegin, dtend, patientids, labels)
 
     with engine.connect() as conn:
-        df = pd.read_sql(q, conn, index_col='TimeStamp')
+        df = pd.read_sql(q, conn, index_col="TimeStamp")
     engine.dispose()
     if len(df) == 0:
         return enumerations_meta
     else:
         df.index = pd.to_datetime(df.index, utc=True)
         return df.astype(enumerations_meta.dtypes.to_dict(), copy=False)
 
 
 def build_enumerations_query(engine, dtbegin, dtend, patientids, labels):
-    dbmeta = MetaData(schema='_Export')
-    dbmeta.reflect(bind=engine)
-    eet = Table('Enumeration_', dbmeta, autoload=True, autoload_with=engine)
-    evt = Table(
-        'EnumerationValue_',
-        dbmeta,
-        autoload=True,
-        autoload_with=engine,
-    )
+    dbmeta = MetaData(schema="_Export")
+    eet = Table("Enumeration_", dbmeta, autoload_with=engine)
+    evt = Table("EnumerationValue_", dbmeta, autoload_with=engine)
 
     ee = select(eet.c.TimeStamp, eet.c.Id, eet.c.Label)
-    ee = ee.with_hint(eet, 'WITH (NOLOCK)')
+    ee = ee.with_hint(eet, "WITH (NOLOCK)")
     ee = ee.where(eet.c.TimeStamp >= dtbegin)
     ee = ee.where(eet.c.TimeStamp < dtend)
     if labels:
         ee = ee.where(eet.c.Label.in_(labels))
-    ee = ee.cte('Enumeration')
+    ee = ee.cte("Enumeration")
 
     ev = select(evt.c.TimeStamp, evt.c.EnumerationId, evt.c.Value, evt.c.PatientId)
-    ev = ev.with_hint(evt, 'WITH (NOLOCK)')
+    ev = ev.with_hint(evt, "WITH (NOLOCK)")
     ev = ev.where(evt.c.TimeStamp >= dtbegin)
     ev = ev.where(evt.c.TimeStamp < dtend)
     ev = ev.where(evt.c.Value.is_not(None))
     if patientids:
         if is_list_like(patientids):
             ev = ev.where(evt.c.PatientId.in_(patientids))
         else:
             ev = ev.where(evt.c.PatientId == patientids)
-    ev = ev.cte('EnumerationValue')
+    ev = ev.cte("EnumerationValue")
 
     j = join(ev, ee, ev.c.EnumerationId == ee.c.Id)
     q = select(ev.c.TimeStamp, ev.c.PatientId, ee.c.Label, ev.c.Value).select_from(j)
     return q
```

### Comparing `dwclib-2024.4.4/src/dwclib/numerics/numerics.py` & `dwclib-2024.5.10/src/dwclib/numerics/numerics.py`

 * *Files identical despite different names*

### Comparing `dwclib-2024.4.4/src/dwclib/patients/patients.py` & `dwclib-2024.5.10/src/dwclib/patients/patients.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from typing import List, Optional
 
 import pandas as pd
 from sqlalchemy import MetaData, Table, asc, create_engine, func, or_, select
 
-
-from dwclib.common.db import pguri
+from dwclib.common.db import dwcuri, pguri
 
 
 def read_patient(*args, **kwargs) -> Optional[pd.Series]:
     """Reads a single patient from DWCmeta database.
 
     Retrieves a pandas series consisting of the patient which matches the search criteria.
 
@@ -92,15 +91,60 @@
         numericlabels,
         numericsublabels,
     )
     if limit:
         q = q.limit(limit)
     engine = create_engine(uri)
     with engine.connect() as conn:
-        df = pd.read_sql(q, conn, index_col='patientid')
+        df = pd.read_sql(q, conn, index_col="patientid")
+    return df
+
+
+def read_patients_dwc_native(
+    patientid: str = None,
+    dtbegin: str = None,
+    dtend: str = None,
+    clinicalunit: str = None,
+    bedlabel: str = None,
+    uri: Optional[str] = None,
+    limit: Optional[int] = None,
+) -> pd.DataFrame:
+    """Reads patients from DWC database with the need of dwcmeta.
+
+    Retrieves a pandas dataframe consisting of individual patients which match the search criteria.
+
+    Args:
+        patientid: A DWC patient identifier
+        dtbegin: The beginning of available data samples
+        dtend: The end of available data samples
+        clinicalunit: The clinical unit the patient belongs to
+        bedlabel: The bed / room in which the patient stays
+        uri: Optional sqlalchemy URI for the database if not provided in the config file
+        limit: Maximum number of returned results
+
+    Returns:
+        A pandas dataframe with each row corresponding to an individual patient stay, indexed by unique DWC patient identifiers.
+    """
+    if not uri:
+        uri = dwcuri
+
+    q = build_query_dwc_native(
+        uri,
+        patientid,
+        dtbegin,
+        dtend,
+        clinicalunit,
+        bedlabel,
+    )
+
+    if limit:
+        q = q.limit(limit)
+    engine = create_engine(uri)
+    with engine.connect() as conn:
+        df = pd.read_sql(q, conn, index_col="patientid")
     return df
 
 
 def build_query(
     uri,
     patientid,
     name,
@@ -112,33 +156,32 @@
     bedlabel,
     wavelabels,
     numericlabels,
     numericsublabels,
 ):
     pgdb = create_engine(uri)
     pgmeta = MetaData()
-    pgmeta.reflect(bind=pgdb)
-    t_patients = Table('patients', pgmeta, autoload_with=pgdb)
+    t_patients = Table("patients", pgmeta, autoload_with=pgdb)
     p = t_patients.c
-    t_patientlabels = Table('patientlabels', pgmeta, autoload_with=pgdb)
+    t_patientlabels = Table("patientlabels", pgmeta, autoload_with=pgdb)
     pl = t_patientlabels.c
 
     if name or firstname:
         # Build a subquery to allow approximate name search
         fields = [t_patients]
         if name:
             fields.append(
                 func.levenshtein(func.lower(p.lastname), func.lower(name)).label(
-                    'd_name'
+                    "d_name"
                 )
             )
         if firstname:
             fields.append(
                 func.levenshtein(func.lower(p.firstname), func.lower(firstname)).label(
-                    'd_firstname'
+                    "d_firstname"
                 )
             )
         t_patients = select(*fields).cte()  # Replace Patients table with CTE
         p = t_patients.c
 
     q = select(t_patients, pl.numericlabels, pl.numericsublabels, pl.wavelabels)
     q = q.select_from(
@@ -165,7 +208,44 @@
     if numericlabels:
         q = q.where(pl.numericlabels.contains(numericlabels))
     if numericsublabels:
         q = q.where(pl.numericsublabels.contains(numericsublabels))
     if wavelabels:
         q = q.where(pl.wavelabels.contains(wavelabels))
     return q
+
+
+def build_query_dwc_native(
+    uri,
+    patientid,
+    dtbegin,
+    dtend,
+    clinicalunit,
+    bedlabel,
+):
+    dwcdb = create_engine(uri)
+    meta = MetaData(schema="_Export")
+    t_patients = Table("Patient_", meta, autoload_with=dwcdb)
+    p = t_patients.c
+
+    q = select(
+        p.Id.label("patientid"),
+        func.min(p.Timestamp).label("data_begin"),
+        func.max(p.Timestamp).label("data_end"),
+        func.max(p.BedLabel).label("bedlabel"),
+        func.max(p.AdmitState).label("admitstate"),
+        func.max(p.ClinicalUnit).label("clinicalunit"),
+        func.max(p.Gender).label("gender"),
+    )
+    q = q.group_by(p.Id)
+
+    if patientid:
+        q = q.where(p.Id == patientid)
+    if bedlabel:
+        q = q.where(p.BedLabel == bedlabel)
+    if clinicalunit:
+        q = q.where(p.ClinicalUnit == clinicalunit)
+    if dtbegin:
+        q = q.where(p.Timestamp >= dtbegin)
+    if dtend:
+        q = q.where(p.Timestamp <= dtend)
+    return q
```

### Comparing `dwclib-2024.4.4/src/dwclib/waves/waves.py` & `dwclib-2024.5.10/src/dwclib/waves/waves.py`

 * *Files identical despite different names*

### Comparing `dwclib-2024.4.4/PKG-INFO` & `dwclib-2024.5.10/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dwclib
-Version: 2024.4.4
+Version: 2024.5.10
 Summary: Python wrapper to DataWarehouse Connect
 Home-page: https://github.com/larib-data/dwclib
 License: ISC
 Author: Jona Joachim
 Author-email: jona@joachim.cc
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved
@@ -33,14 +33,17 @@
 Installation through conda greatly simplifies dependency management.
 
 Additionally, Microsoft SQL Server drivers are needed and will need to be installed seperately.
 See here for more information: https://github.com/mkleehammer/pyodbc/wiki
 
 
 ## Changelog
+- 2024.5.10
+    - Support searching patients directly in DWC without DWCmeta
+
 - 2024.4.4
     - Support querying enumerations
     - Update dependencies
 
 - 2023.6.21
     - Remove all occurences of naive datetime since dask now support tz-aware
     - New config file syntax to be compatible with other libraries
```

