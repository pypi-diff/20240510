# Comparing `tmp/rdf_doctor-1.1.2-py3-none-any.whl.zip` & `tmp/rdf_doctor-1.1.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 59873 bytes, number of entries: 12
--rw-r--r--  2.0 unx       22 b- defN 24-May-07 07:07 doctor/__init__.py
+Zip file size: 59874 bytes, number of entries: 12
+-rw-r--r--  2.0 unx       22 b- defN 24-May-09 04:59 doctor/__init__.py
 -rw-r--r--  2.0 unx     1754 b- defN 24-May-07 05:38 doctor/consts.py
 -rw-r--r--  2.0 unx    81134 b- defN 24-May-07 05:38 doctor/doctor.py
 -rw-r--r--  2.0 unx   134314 b- defN 24-May-07 05:38 doctor/reference/prefixes.tsv
 -rw-r--r--  2.0 unx       90 b- defN 24-May-07 05:38 doctor/reference/refine-class-uris.tsv
 -rw-r--r--  2.0 unx      577 b- defN 24-May-07 05:38 doctor/reference/refine-prefix-uris.tsv
--rw-r--r--  2.0 unx     1061 b- defN 24-May-07 07:16 rdf_doctor-1.1.2.dist-info/LICENSE
--rw-r--r--  2.0 unx    10651 b- defN 24-May-07 07:16 rdf_doctor-1.1.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-07 07:16 rdf_doctor-1.1.2.dist-info/WHEEL
--rw-r--r--  2.0 unx       52 b- defN 24-May-07 07:16 rdf_doctor-1.1.2.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        7 b- defN 24-May-07 07:16 rdf_doctor-1.1.2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      995 b- defN 24-May-07 07:16 rdf_doctor-1.1.2.dist-info/RECORD
-12 files, 230749 bytes uncompressed, 58193 bytes compressed:  74.8%
+-rw-r--r--  2.0 unx     1061 b- defN 24-May-09 05:01 rdf_doctor-1.1.3.dist-info/LICENSE
+-rw-r--r--  2.0 unx    10651 b- defN 24-May-09 05:01 rdf_doctor-1.1.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-09 05:01 rdf_doctor-1.1.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx       52 b- defN 24-May-09 05:01 rdf_doctor-1.1.3.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        7 b- defN 24-May-09 05:01 rdf_doctor-1.1.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      995 b- defN 24-May-09 05:01 rdf_doctor-1.1.3.dist-info/RECORD
+12 files, 230749 bytes uncompressed, 58194 bytes compressed:  74.8%
```

## zipnote {}

```diff
@@ -12,26 +12,26 @@
 
 Filename: doctor/reference/refine-class-uris.tsv
 Comment: 
 
 Filename: doctor/reference/refine-prefix-uris.tsv
 Comment: 
 
-Filename: rdf_doctor-1.1.2.dist-info/LICENSE
+Filename: rdf_doctor-1.1.3.dist-info/LICENSE
 Comment: 
 
-Filename: rdf_doctor-1.1.2.dist-info/METADATA
+Filename: rdf_doctor-1.1.3.dist-info/METADATA
 Comment: 
 
-Filename: rdf_doctor-1.1.2.dist-info/WHEEL
+Filename: rdf_doctor-1.1.3.dist-info/WHEEL
 Comment: 
 
-Filename: rdf_doctor-1.1.2.dist-info/entry_points.txt
+Filename: rdf_doctor-1.1.3.dist-info/entry_points.txt
 Comment: 
 
-Filename: rdf_doctor-1.1.2.dist-info/top_level.txt
+Filename: rdf_doctor-1.1.3.dist-info/top_level.txt
 Comment: 
 
-Filename: rdf_doctor-1.1.2.dist-info/RECORD
+Filename: rdf_doctor-1.1.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## doctor/__init__.py

```diff
@@ -1 +1 @@
-__version__ = "1.1.2"
+__version__ = "1.1.3"
```

## Comparing `rdf_doctor-1.1.2.dist-info/LICENSE` & `rdf_doctor-1.1.3.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `rdf_doctor-1.1.2.dist-info/METADATA` & `rdf_doctor-1.1.3.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rdf-doctor
-Version: 1.1.2
+Version: 1.1.3
 Summary: Validate RDF data, report problems, and support creation of more accurate data
 Home-page: https://github.com/dbcls/rdf-doctor
 Author: DBCLS
 License: MIT
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

## Comparing `rdf_doctor-1.1.2.dist-info/RECORD` & `rdf_doctor-1.1.3.dist-info/RECORD`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-doctor/__init__.py,sha256=5SgGjThsHu_ITn8V83BvCziqCwxdXxTQqcC3KQMHPfM,22
+doctor/__init__.py,sha256=u9ExJqoMv3fQc8WmLTw4I2FnQo6u4xRrBc6DLy6G1IE,22
 doctor/consts.py,sha256=U8KOzdPFgMuf_nMul1Vw9qtAvKtZbu8WLwkiYD49IAs,1754
 doctor/doctor.py,sha256=Z8YHopV7U7kpliAh54FxESObTfSHBpczC-iXFHRwfsQ,81134
 doctor/reference/prefixes.tsv,sha256=_1hW0wBl6K1YvcM8stdiEdD4elzST_ecJqQEvhD9Auk,134314
 doctor/reference/refine-class-uris.tsv,sha256=pd_nOSjR7bia96u9hhcjhBg9J6LUAuDFlyy-JE9tsys,90
 doctor/reference/refine-prefix-uris.tsv,sha256=KY5PZ4WCaLeB0APNBjAWq7_Q5Whc6FLg9ncX7BSPeuw,577
-rdf_doctor-1.1.2.dist-info/LICENSE,sha256=e5qMQtuffizvdi23h6MoQ37f3xmNY0VBq8V0tgWuZNg,1061
-rdf_doctor-1.1.2.dist-info/METADATA,sha256=QGhHrL6ZWSA4EXyrjGEOY5OmAMyfVTSqF79bUK10Y8w,10651
-rdf_doctor-1.1.2.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-rdf_doctor-1.1.2.dist-info/entry_points.txt,sha256=1vHyYdY5pMK7zOINHh2ymwU_Uid1YzZx7Vte5tjHCls,52
-rdf_doctor-1.1.2.dist-info/top_level.txt,sha256=8awHkjBkPxJ8N_ygAwmuUTUz5ZKfy9aqNcWTSI_Ma_8,7
-rdf_doctor-1.1.2.dist-info/RECORD,,
+rdf_doctor-1.1.3.dist-info/LICENSE,sha256=e5qMQtuffizvdi23h6MoQ37f3xmNY0VBq8V0tgWuZNg,1061
+rdf_doctor-1.1.3.dist-info/METADATA,sha256=DFDmWv-Bt7hel-RUgxCKQ0AGLOd1rH2B8BsCP9E-luU,10651
+rdf_doctor-1.1.3.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+rdf_doctor-1.1.3.dist-info/entry_points.txt,sha256=1vHyYdY5pMK7zOINHh2ymwU_Uid1YzZx7Vte5tjHCls,52
+rdf_doctor-1.1.3.dist-info/top_level.txt,sha256=8awHkjBkPxJ8N_ygAwmuUTUz5ZKfy9aqNcWTSI_Ma_8,7
+rdf_doctor-1.1.3.dist-info/RECORD,,
```

