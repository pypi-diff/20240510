# Comparing `tmp/typesense-0.8.0-py2.py3-none-any.whl.zip` & `tmp/typesense-0.9.0-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 19843 bytes, number of entries: 27
+Zip file size: 19841 bytes, number of entries: 27
 -rw-r--r--  2.0 unx        0 b- defN 18-Jan-30 21:30 examples/__init__.py
 -rw-r--r--  2.0 unx     1839 b- defN 20-Oct-21 14:21 examples/alias_operations.py
 -rw-r--r--  2.0 unx     3106 b- defN 20-Oct-24 16:05 examples/collection_operations.py
 -rw-r--r--  2.0 unx     1986 b- defN 20-Oct-21 14:21 examples/curation_operations.py
 -rw-r--r--  2.0 unx     1713 b- defN 20-Oct-21 14:21 examples/index_and_search.py
 -rw-r--r--  2.0 unx     2604 b- defN 20-Oct-21 14:21 examples/key_operations.py
 -rw-r--r--  2.0 unx       91 b- defN 20-Oct-21 14:21 typesense/__init__.py
@@ -17,13 +17,13 @@
 -rw-r--r--  2.0 unx      762 b- defN 20-Oct-24 13:40 typesense/document.py
 -rw-r--r--  2.0 unx     2698 b- defN 20-Oct-25 03:37 typesense/documents.py
 -rw-r--r--  2.0 unx      763 b- defN 20-Oct-21 14:21 typesense/exceptions.py
 -rw-r--r--  2.0 unx      416 b- defN 20-Oct-21 14:21 typesense/key.py
 -rw-r--r--  2.0 unx     1131 b- defN 20-Oct-21 14:21 typesense/keys.py
 -rw-r--r--  2.0 unx      661 b- defN 20-Oct-21 14:21 typesense/override.py
 -rw-r--r--  2.0 unx      967 b- defN 20-Oct-21 14:21 typesense/overrides.py
--rw-r--r--  2.0 unx    11357 b- defN 20-Oct-25 15:10 typesense-0.8.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     1304 b- defN 20-Oct-25 15:10 typesense-0.8.0.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 20-Oct-25 15:10 typesense-0.8.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       19 b- defN 20-Oct-25 15:10 typesense-0.8.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     2134 b- defN 20-Oct-25 15:10 typesense-0.8.0.dist-info/RECORD
-27 files, 46568 bytes uncompressed, 16435 bytes compressed:  64.7%
+-rw-r--r--  2.0 unx    11357 b- defN 21-Jan-02 13:15 typesense-0.9.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1304 b- defN 21-Jan-02 13:15 typesense-0.9.0.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 21-Jan-02 13:15 typesense-0.9.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       19 b- defN 21-Jan-02 13:15 typesense-0.9.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     2134 b- defN 21-Jan-02 13:15 typesense-0.9.0.dist-info/RECORD
+27 files, 46568 bytes uncompressed, 16433 bytes compressed:  64.7%
```

## zipnote {}

```diff
@@ -60,23 +60,23 @@
 
 Filename: typesense/override.py
 Comment: 
 
 Filename: typesense/overrides.py
 Comment: 
 
-Filename: typesense-0.8.0.dist-info/LICENSE
+Filename: typesense-0.9.0.dist-info/LICENSE
 Comment: 
 
-Filename: typesense-0.8.0.dist-info/METADATA
+Filename: typesense-0.9.0.dist-info/METADATA
 Comment: 
 
-Filename: typesense-0.8.0.dist-info/WHEEL
+Filename: typesense-0.9.0.dist-info/WHEEL
 Comment: 
 
-Filename: typesense-0.8.0.dist-info/top_level.txt
+Filename: typesense-0.9.0.dist-info/top_level.txt
 Comment: 
 
-Filename: typesense-0.8.0.dist-info/RECORD
+Filename: typesense-0.9.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `typesense-0.8.0.dist-info/LICENSE` & `typesense-0.9.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `typesense-0.8.0.dist-info/METADATA` & `typesense-0.9.0.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: typesense
-Version: 0.8.0
+Version: 0.9.0
 Summary: Python client for Typesense, an open source and typo tolerant search engine.
 Home-page: https://typesense.org
 Author: Typesense
 Author-email: contact+typesense@wreally.com
 License: Apache 2.0
 Platform: UNKNOWN
 Requires-Python: >=3
```

## Comparing `typesense-0.8.0.dist-info/RECORD` & `typesense-0.9.0.dist-info/RECORD`

 * *Files 4% similar despite different names*

```diff
@@ -16,12 +16,12 @@
 typesense/document.py,sha256=wSUb4mUKiF6vDjQsvgxkbbLlTEh3fPepnDPsBGnaGh0,762
 typesense/documents.py,sha256=3q0VUYRZ3blCEkymIDXsi7e6Vng1hapoplHFnwfU644,2698
 typesense/exceptions.py,sha256=YgyzTKh0IijKDCAM5NgpQ7FOmbbMoT59KSoqgl2vJ2U,763
 typesense/key.py,sha256=m1HoKm7oc5YJwVw6OrbjOVVhhf1iFUBnjfV8T6mD9gM,416
 typesense/keys.py,sha256=l6TQEL2gPIKdsAqYPbSZnkQ-UOyO2bKM_VXyTuMEooo,1131
 typesense/override.py,sha256=KHJPfVR21b48ohKEtivO5z0LxQBBYPZQrY-SIDlAh0M,661
 typesense/overrides.py,sha256=noXOqOjVB4mswr8T5IFbIuyX5zdBEsrnZATaf1OrBAU,967
-typesense-0.8.0.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
-typesense-0.8.0.dist-info/METADATA,sha256=akvGP8vz_UEoKIxUcuhh0-Y1bLoV8cEXcnknMsVRmdE,1304
-typesense-0.8.0.dist-info/WHEEL,sha256=ADKeyaGyKF5DwBNE0sRE5pvW-bSkFMJfBuhzZ3rceP4,110
-typesense-0.8.0.dist-info/top_level.txt,sha256=km6oh6AE4H-aQJ4qwVH2xJJj8hHkIgyUKWAwGHIYAfg,19
-typesense-0.8.0.dist-info/RECORD,,
+typesense-0.9.0.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+typesense-0.9.0.dist-info/METADATA,sha256=RdFPO_wKAlJN0i7IAYA1vvDA8IUp2OlSCFwFfp4vRK4,1304
+typesense-0.9.0.dist-info/WHEEL,sha256=ADKeyaGyKF5DwBNE0sRE5pvW-bSkFMJfBuhzZ3rceP4,110
+typesense-0.9.0.dist-info/top_level.txt,sha256=km6oh6AE4H-aQJ4qwVH2xJJj8hHkIgyUKWAwGHIYAfg,19
+typesense-0.9.0.dist-info/RECORD,,
```

