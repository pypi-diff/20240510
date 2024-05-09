# Comparing `tmp/sparecores_crawler-0.1.2.tar.gz` & `tmp/sparecores_crawler-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sparecores_crawler-0.1.2.tar", last modified: Wed Apr 24 22:22:20 2024, max compression
+gzip compressed data, was "sparecores_crawler-0.1.3.tar", last modified: Thu May  9 22:02:51 2024, max compression
```

## Comparing `sparecores_crawler-0.1.2.tar` & `sparecores_crawler-0.1.3.tar`

### file list

```diff
@@ -1,44 +1,46 @@
-drwxr-xr-x   0 daroczig  (1000) daroczig  (1000)        0 2024-04-24 22:22:20.498400 sparecores_crawler-0.1.2/
--rw-r--r--   0 daroczig  (1000) daroczig  (1000)    16726 2023-12-08 22:12:52.000000 sparecores_crawler-0.1.2/LICENSE
--rw-r--r--   0 daroczig  (1000) daroczig  (1000)       53 2024-04-12 16:09:18.000000 sparecores_crawler-0.1.2/MANIFEST.in
--rw-r--r--   0 daroczig  (1000) daroczig  (1000)     7725 2024-04-24 22:22:20.498400 sparecores_crawler-0.1.2/PKG-INFO
--rw-r--r--   0 daroczig  (1000) daroczig  (1000)     5326 2024-04-04 14:00:10.000000 sparecores_crawler-0.1.2/README.md
--rw-r--r--   0 daroczig  (1000) daroczig  (1000)     3737 2024-04-24 22:21:44.000000 sparecores_crawler-0.1.2/pyproject.toml
--rw-r--r--   0 daroczig  (1000) daroczig  (1000)       38 2024-04-24 22:22:20.498400 sparecores_crawler-0.1.2/setup.cfg
-drwxr-xr-x   0 daroczig  (1000) daroczig  (1000)        0 2024-04-24 22:22:20.485067 sparecores_crawler-0.1.2/src/
-drwxr-xr-x   0 daroczig  (1000) daroczig  (1000)        0 2024-04-24 22:22:20.491734 sparecores_crawler-0.1.2/src/sc_crawler/
--rw-r--r--   0 daroczig  (1000) daroczig  (1000)        0 2024-02-14 13:12:38.000000 sparecores_crawler-0.1.2/src/sc_crawler/__init__.py
-drwxr-xr-x   0 daroczig  (1000) daroczig  (1000)        0 2024-04-24 22:22:20.491734 sparecores_crawler-0.1.2/src/sc_crawler/alembic/
--rw-r--r--   0 daroczig  (1000) daroczig  (1000)     2977 2024-04-24 21:32:55.000000 sparecores_crawler-0.1.2/src/sc_crawler/alembic/env.py
-drwxr-xr-x   0 daroczig  (1000) daroczig  (1000)        0 2024-04-24 22:22:20.491734 sparecores_crawler-0.1.2/src/sc_crawler/alembic/versions/
--rw-r--r--   0 daroczig  (1000) daroczig  (1000)     5929 2024-04-24 21:32:55.000000 sparecores_crawler-0.1.2/src/sc_crawler/alembic/versions/4691089690c2_v0_1_1.py
--rw-r--r--   0 daroczig  (1000) daroczig  (1000)    68592 2024-04-24 21:32:55.000000 sparecores_crawler-0.1.2/src/sc_crawler/alembic/versions/98894dffd37c_v0_1_0.py
--rw-r--r--   0 daroczig  (1000) daroczig  (1000)     3618 2024-04-12 15:45:00.000000 sparecores_crawler-0.1.2/src/sc_crawler/alembic.ini
--rw-r--r--   0 daroczig  (1000) daroczig  (1000)     1185 2024-04-12 16:10:05.000000 sparecores_crawler-0.1.2/src/sc_crawler/alembic_helpers.py
--rw-r--r--   0 daroczig  (1000) daroczig  (1000)    22486 2024-04-12 16:49:26.000000 sparecores_crawler-0.1.2/src/sc_crawler/cli.py
--rw-r--r--   0 daroczig  (1000) daroczig  (1000)     6780 2024-04-10 22:14:16.000000 sparecores_crawler-0.1.2/src/sc_crawler/insert.py
--rw-r--r--   0 daroczig  (1000) daroczig  (1000)     8517 2024-04-04 14:01:05.000000 sparecores_crawler-0.1.2/src/sc_crawler/logger.py
--rw-r--r--   0 daroczig  (1000) daroczig  (1000)     3624 2024-04-24 22:21:44.000000 sparecores_crawler-0.1.2/src/sc_crawler/lookup.py
--rw-r--r--   0 daroczig  (1000) daroczig  (1000)     2201 2024-04-04 14:00:10.000000 sparecores_crawler-0.1.2/src/sc_crawler/str_utils.py
--rw-r--r--   0 daroczig  (1000) daroczig  (1000)    19543 2024-04-23 20:55:29.000000 sparecores_crawler-0.1.2/src/sc_crawler/table_bases.py
--rw-r--r--   0 daroczig  (1000) daroczig  (1000)     4705 2024-04-04 14:00:10.000000 sparecores_crawler-0.1.2/src/sc_crawler/table_fields.py
--rw-r--r--   0 daroczig  (1000) daroczig  (1000)    17017 2024-04-24 22:21:44.000000 sparecores_crawler-0.1.2/src/sc_crawler/tables.py
--rw-r--r--   0 daroczig  (1000) daroczig  (1000)     2730 2024-04-04 14:00:10.000000 sparecores_crawler-0.1.2/src/sc_crawler/tables_scd.py
--rw-r--r--   0 daroczig  (1000) daroczig  (1000)     5156 2024-04-24 22:21:44.000000 sparecores_crawler-0.1.2/src/sc_crawler/utils.py
-drwxr-xr-x   0 daroczig  (1000) daroczig  (1000)        0 2024-04-24 22:22:20.491734 sparecores_crawler-0.1.2/src/sc_crawler/vendors/
--rw-r--r--   0 daroczig  (1000) daroczig  (1000)      116 2024-04-12 15:19:56.000000 sparecores_crawler-0.1.2/src/sc_crawler/vendors/__init__.py
--rw-r--r--   0 daroczig  (1000) daroczig  (1000)    38992 2024-04-24 22:21:44.000000 sparecores_crawler-0.1.2/src/sc_crawler/vendors/aws.py
--rw-r--r--   0 daroczig  (1000) daroczig  (1000)    31391 2024-04-24 22:21:44.000000 sparecores_crawler-0.1.2/src/sc_crawler/vendors/gcp.py
--rw-r--r--   0 daroczig  (1000) daroczig  (1000)    10143 2024-04-24 22:21:44.000000 sparecores_crawler-0.1.2/src/sc_crawler/vendors/hcloud.py
--rw-r--r--   0 daroczig  (1000) daroczig  (1000)     1520 2024-04-24 22:21:44.000000 sparecores_crawler-0.1.2/src/sc_crawler/vendors/vendors.py
-drwxr-xr-x   0 daroczig  (1000) daroczig  (1000)        0 2024-04-24 22:22:20.495067 sparecores_crawler-0.1.2/src/sparecores_crawler.egg-info/
--rw-r--r--   0 daroczig  (1000) daroczig  (1000)     7725 2024-04-24 22:22:20.000000 sparecores_crawler-0.1.2/src/sparecores_crawler.egg-info/PKG-INFO
--rw-r--r--   0 daroczig  (1000) daroczig  (1000)     1042 2024-04-24 22:22:20.000000 sparecores_crawler-0.1.2/src/sparecores_crawler.egg-info/SOURCES.txt
--rw-r--r--   0 daroczig  (1000) daroczig  (1000)        1 2024-04-24 22:22:20.000000 sparecores_crawler-0.1.2/src/sparecores_crawler.egg-info/dependency_links.txt
--rw-r--r--   0 daroczig  (1000) daroczig  (1000)       50 2024-04-24 22:22:20.000000 sparecores_crawler-0.1.2/src/sparecores_crawler.egg-info/entry_points.txt
--rw-r--r--   0 daroczig  (1000) daroczig  (1000)      581 2024-04-24 22:22:20.000000 sparecores_crawler-0.1.2/src/sparecores_crawler.egg-info/requires.txt
--rw-r--r--   0 daroczig  (1000) daroczig  (1000)       11 2024-04-24 22:22:20.000000 sparecores_crawler-0.1.2/src/sparecores_crawler.egg-info/top_level.txt
-drwxr-xr-x   0 daroczig  (1000) daroczig  (1000)        0 2024-04-24 22:22:20.495067 sparecores_crawler-0.1.2/tests/
--rw-r--r--   0 daroczig  (1000) daroczig  (1000)     1391 2024-04-04 14:00:10.000000 sparecores_crawler-0.1.2/tests/test_schemas.py
--rw-r--r--   0 daroczig  (1000) daroczig  (1000)     1316 2024-04-04 14:00:10.000000 sparecores_crawler-0.1.2/tests/test_str_utils.py
--rw-r--r--   0 daroczig  (1000) daroczig  (1000)     1216 2024-03-25 14:01:48.000000 sparecores_crawler-0.1.2/tests/test_utils.py
+drwxr-xr-x   0 daroczig  (1000) daroczig  (1000)        0 2024-05-09 22:02:51.774617 sparecores_crawler-0.1.3/
+-rw-r--r--   0 daroczig  (1000) daroczig  (1000)    16726 2023-12-08 22:12:52.000000 sparecores_crawler-0.1.3/LICENSE
+-rw-r--r--   0 daroczig  (1000) daroczig  (1000)       53 2024-04-12 16:09:18.000000 sparecores_crawler-0.1.3/MANIFEST.in
+-rw-r--r--   0 daroczig  (1000) daroczig  (1000)     7725 2024-05-09 22:02:51.774617 sparecores_crawler-0.1.3/PKG-INFO
+-rw-r--r--   0 daroczig  (1000) daroczig  (1000)     5326 2024-04-04 14:00:10.000000 sparecores_crawler-0.1.3/README.md
+-rw-r--r--   0 daroczig  (1000) daroczig  (1000)     3737 2024-05-07 11:57:49.000000 sparecores_crawler-0.1.3/pyproject.toml
+-rw-r--r--   0 daroczig  (1000) daroczig  (1000)       38 2024-05-09 22:02:51.774617 sparecores_crawler-0.1.3/setup.cfg
+drwxr-xr-x   0 daroczig  (1000) daroczig  (1000)        0 2024-05-09 22:02:51.761283 sparecores_crawler-0.1.3/src/
+drwxr-xr-x   0 daroczig  (1000) daroczig  (1000)        0 2024-05-09 22:02:51.764617 sparecores_crawler-0.1.3/src/sc_crawler/
+-rw-r--r--   0 daroczig  (1000) daroczig  (1000)        0 2024-02-14 13:12:38.000000 sparecores_crawler-0.1.3/src/sc_crawler/__init__.py
+drwxr-xr-x   0 daroczig  (1000) daroczig  (1000)        0 2024-05-09 22:02:51.764617 sparecores_crawler-0.1.3/src/sc_crawler/alembic/
+-rw-r--r--   0 daroczig  (1000) daroczig  (1000)     2977 2024-04-24 21:32:55.000000 sparecores_crawler-0.1.3/src/sc_crawler/alembic/env.py
+drwxr-xr-x   0 daroczig  (1000) daroczig  (1000)        0 2024-05-09 22:02:51.764617 sparecores_crawler-0.1.3/src/sc_crawler/alembic/versions/
+-rw-r--r--   0 daroczig  (1000) daroczig  (1000)     5929 2024-04-24 21:32:55.000000 sparecores_crawler-0.1.3/src/sc_crawler/alembic/versions/4691089690c2_v0_1_1.py
+-rw-r--r--   0 daroczig  (1000) daroczig  (1000)    68592 2024-04-24 21:32:55.000000 sparecores_crawler-0.1.3/src/sc_crawler/alembic/versions/98894dffd37c_v0_1_0.py
+-rw-r--r--   0 daroczig  (1000) daroczig  (1000)     9694 2024-05-07 21:26:31.000000 sparecores_crawler-0.1.3/src/sc_crawler/alembic/versions/f6bf6152039a_v0_1_3_step2.py
+-rw-r--r--   0 daroczig  (1000) daroczig  (1000)    13080 2024-05-09 21:10:36.000000 sparecores_crawler-0.1.3/src/sc_crawler/alembic/versions/f6edf4a96a78_v0_1_3_step1.py
+-rw-r--r--   0 daroczig  (1000) daroczig  (1000)     3618 2024-04-12 15:45:00.000000 sparecores_crawler-0.1.3/src/sc_crawler/alembic.ini
+-rw-r--r--   0 daroczig  (1000) daroczig  (1000)     1185 2024-04-12 16:10:05.000000 sparecores_crawler-0.1.3/src/sc_crawler/alembic_helpers.py
+-rw-r--r--   0 daroczig  (1000) daroczig  (1000)    22486 2024-04-12 16:49:26.000000 sparecores_crawler-0.1.3/src/sc_crawler/cli.py
+-rw-r--r--   0 daroczig  (1000) daroczig  (1000)     6780 2024-04-10 22:14:16.000000 sparecores_crawler-0.1.3/src/sc_crawler/insert.py
+-rw-r--r--   0 daroczig  (1000) daroczig  (1000)     8517 2024-04-04 14:01:05.000000 sparecores_crawler-0.1.3/src/sc_crawler/logger.py
+-rw-r--r--   0 daroczig  (1000) daroczig  (1000)     3624 2024-04-24 22:21:44.000000 sparecores_crawler-0.1.3/src/sc_crawler/lookup.py
+-rw-r--r--   0 daroczig  (1000) daroczig  (1000)     2201 2024-04-04 14:00:10.000000 sparecores_crawler-0.1.3/src/sc_crawler/str_utils.py
+-rw-r--r--   0 daroczig  (1000) daroczig  (1000)    20637 2024-05-07 11:04:13.000000 sparecores_crawler-0.1.3/src/sc_crawler/table_bases.py
+-rw-r--r--   0 daroczig  (1000) daroczig  (1000)     4705 2024-04-04 14:00:10.000000 sparecores_crawler-0.1.3/src/sc_crawler/table_fields.py
+-rw-r--r--   0 daroczig  (1000) daroczig  (1000)    17017 2024-04-24 22:21:44.000000 sparecores_crawler-0.1.3/src/sc_crawler/tables.py
+-rw-r--r--   0 daroczig  (1000) daroczig  (1000)     2730 2024-04-04 14:00:10.000000 sparecores_crawler-0.1.3/src/sc_crawler/tables_scd.py
+-rw-r--r--   0 daroczig  (1000) daroczig  (1000)     5156 2024-04-24 22:21:44.000000 sparecores_crawler-0.1.3/src/sc_crawler/utils.py
+drwxr-xr-x   0 daroczig  (1000) daroczig  (1000)        0 2024-05-09 22:02:51.767950 sparecores_crawler-0.1.3/src/sc_crawler/vendors/
+-rw-r--r--   0 daroczig  (1000) daroczig  (1000)      116 2024-04-12 15:19:56.000000 sparecores_crawler-0.1.3/src/sc_crawler/vendors/__init__.py
+-rw-r--r--   0 daroczig  (1000) daroczig  (1000)    42164 2024-05-09 20:10:59.000000 sparecores_crawler-0.1.3/src/sc_crawler/vendors/aws.py
+-rw-r--r--   0 daroczig  (1000) daroczig  (1000)    35732 2024-05-09 19:59:03.000000 sparecores_crawler-0.1.3/src/sc_crawler/vendors/gcp.py
+-rw-r--r--   0 daroczig  (1000) daroczig  (1000)    11349 2024-05-09 20:06:56.000000 sparecores_crawler-0.1.3/src/sc_crawler/vendors/hcloud.py
+-rw-r--r--   0 daroczig  (1000) daroczig  (1000)     1520 2024-04-24 22:21:44.000000 sparecores_crawler-0.1.3/src/sc_crawler/vendors/vendors.py
+drwxr-xr-x   0 daroczig  (1000) daroczig  (1000)        0 2024-05-09 22:02:51.771283 sparecores_crawler-0.1.3/src/sparecores_crawler.egg-info/
+-rw-r--r--   0 daroczig  (1000) daroczig  (1000)     7725 2024-05-09 22:02:51.000000 sparecores_crawler-0.1.3/src/sparecores_crawler.egg-info/PKG-INFO
+-rw-r--r--   0 daroczig  (1000) daroczig  (1000)     1164 2024-05-09 22:02:51.000000 sparecores_crawler-0.1.3/src/sparecores_crawler.egg-info/SOURCES.txt
+-rw-r--r--   0 daroczig  (1000) daroczig  (1000)        1 2024-05-09 22:02:51.000000 sparecores_crawler-0.1.3/src/sparecores_crawler.egg-info/dependency_links.txt
+-rw-r--r--   0 daroczig  (1000) daroczig  (1000)       50 2024-05-09 22:02:51.000000 sparecores_crawler-0.1.3/src/sparecores_crawler.egg-info/entry_points.txt
+-rw-r--r--   0 daroczig  (1000) daroczig  (1000)      581 2024-05-09 22:02:51.000000 sparecores_crawler-0.1.3/src/sparecores_crawler.egg-info/requires.txt
+-rw-r--r--   0 daroczig  (1000) daroczig  (1000)       11 2024-05-09 22:02:51.000000 sparecores_crawler-0.1.3/src/sparecores_crawler.egg-info/top_level.txt
+drwxr-xr-x   0 daroczig  (1000) daroczig  (1000)        0 2024-05-09 22:02:51.767950 sparecores_crawler-0.1.3/tests/
+-rw-r--r--   0 daroczig  (1000) daroczig  (1000)     1391 2024-04-04 14:00:10.000000 sparecores_crawler-0.1.3/tests/test_schemas.py
+-rw-r--r--   0 daroczig  (1000) daroczig  (1000)     1316 2024-04-04 14:00:10.000000 sparecores_crawler-0.1.3/tests/test_str_utils.py
+-rw-r--r--   0 daroczig  (1000) daroczig  (1000)     1216 2024-03-25 14:01:48.000000 sparecores_crawler-0.1.3/tests/test_utils.py
```

### Comparing `sparecores_crawler-0.1.2/LICENSE` & `sparecores_crawler-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `sparecores_crawler-0.1.2/PKG-INFO` & `sparecores_crawler-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sparecores-crawler
-Version: 0.1.2
+Version: 0.1.3
 Summary: Pull and standardize data on cloud compute resources.
 Author: Attila Nagy, Gergely Daroczi, Balazs Hodobay
 Maintainer-email: Spare Cores team <pkg@sparecores.com>
 Project-URL: repository, https://github.com/SpareCores/sc-crawler
 Project-URL: issues, https://github.com/SpareCores/sc-crawler/issues
 Project-URL: documentation, https://sparecores.github.io/sc-crawler/
 Project-URL: homepage, https://sparecores.com
```

### Comparing `sparecores_crawler-0.1.2/README.md` & `sparecores_crawler-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `sparecores_crawler-0.1.2/pyproject.toml` & `sparecores_crawler-0.1.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "sparecores-crawler"
-version = "0.1.2"
+version = "0.1.3"
 requires-python = ">= 3.7"
 dependencies = [
   "alembic",
   "cachier",
   "pydantic",
   "pydantic_extra_types",
   "rich",
```

### Comparing `sparecores_crawler-0.1.2/src/sc_crawler/alembic/env.py` & `sparecores_crawler-0.1.3/src/sc_crawler/alembic/env.py`

 * *Files identical despite different names*

### Comparing `sparecores_crawler-0.1.2/src/sc_crawler/alembic/versions/4691089690c2_v0_1_1.py` & `sparecores_crawler-0.1.3/src/sc_crawler/alembic/versions/4691089690c2_v0_1_1.py`

 * *Files identical despite different names*

### Comparing `sparecores_crawler-0.1.2/src/sc_crawler/alembic/versions/98894dffd37c_v0_1_0.py` & `sparecores_crawler-0.1.3/src/sc_crawler/alembic/versions/98894dffd37c_v0_1_0.py`

 * *Files identical despite different names*

### Comparing `sparecores_crawler-0.1.2/src/sc_crawler/alembic.ini` & `sparecores_crawler-0.1.3/src/sc_crawler/alembic.ini`

 * *Files identical despite different names*

### Comparing `sparecores_crawler-0.1.2/src/sc_crawler/alembic_helpers.py` & `sparecores_crawler-0.1.3/src/sc_crawler/alembic_helpers.py`

 * *Files identical despite different names*

### Comparing `sparecores_crawler-0.1.2/src/sc_crawler/cli.py` & `sparecores_crawler-0.1.3/src/sc_crawler/cli.py`

 * *Files identical despite different names*

### Comparing `sparecores_crawler-0.1.2/src/sc_crawler/insert.py` & `sparecores_crawler-0.1.3/src/sc_crawler/insert.py`

 * *Files identical despite different names*

### Comparing `sparecores_crawler-0.1.2/src/sc_crawler/logger.py` & `sparecores_crawler-0.1.3/src/sc_crawler/logger.py`

 * *Files identical despite different names*

### Comparing `sparecores_crawler-0.1.2/src/sc_crawler/lookup.py` & `sparecores_crawler-0.1.3/src/sc_crawler/lookup.py`

 * *Files identical despite different names*

### Comparing `sparecores_crawler-0.1.2/src/sc_crawler/str_utils.py` & `sparecores_crawler-0.1.3/src/sc_crawler/str_utils.py`

 * *Files identical despite different names*

### Comparing `sparecores_crawler-0.1.2/src/sc_crawler/table_bases.py` & `sparecores_crawler-0.1.3/src/sc_crawler/table_bases.py`

 * *Files 8% similar despite different names*

```diff
@@ -234,14 +234,30 @@
     name: str = Field(description="Human-friendly name.")
 
 
 class HasDescription(ScModel):
     description: Optional[str] = Field(description="Short description.")
 
 
+class HasApiReference(ScModel):
+    api_reference: str = Field(
+        description=(
+            "How this resource is referenced in the vendor API calls. "
+            "This is usually either the id or name of the resource, "
+            "depening on the vendor and actual API endpoint."
+        )
+    )
+
+
+class HasDisplayName(ScModel):
+    display_name: str = Field(
+        description="Human-friendly reference (usually the id or name) of the resource."
+    )
+
+
 class HasVendorPKFK(ScModel):
     vendor_id: str = Field(
         foreign_key="vendor.vendor_id",
         primary_key=True,
         description="Reference to the Vendor.",
     )
 
@@ -383,15 +399,17 @@
     )
 
 
 class VendorComplianceLinkBase(MetaColumns, VendorComplianceLinkFields):
     pass
 
 
-class DatacenterFields(HasName, HasDatacenterIdPK, HasVendorPKFK):
+class DatacenterFields(
+    HasDisplayName, HasApiReference, HasName, HasDatacenterIdPK, HasVendorPKFK
+):
     aliases: List[str] = Field(
         default=[],
         sa_type=JSON,
         description="List of other commonly used names for the same Datacenter.",
     )
     country_id: str = Field(
         foreign_key="country.country_id",
@@ -406,29 +424,45 @@
     )
     address_line: Optional[str] = Field(
         default=None, description="Optional address line of the Datacenter's location."
     )
     zip_code: Optional[str] = Field(
         default=None, description="Optional ZIP code of the Datacenter's location."
     )
+    lon: Optional[float] = Field(
+        default=None,
+        description="Longitude coordinate of the Datacenter's known or approximate location.",
+    )
+    lat: Optional[float] = Field(
+        default=None,
+        description="Latitude coordinate of the Datacenter's known or approximate location.",
+    )
 
     founding_year: Optional[int] = Field(
         default=None, description="4-digit year when the Datacenter was founded."
     )
     green_energy: Optional[bool] = Field(
         default=None,
         description="If the Datacenter is 100% powered by renewable energy.",
     )
 
 
 class DatacenterBase(MetaColumns, DatacenterFields):
     pass
 
 
-class ZoneBase(MetaColumns, HasName, HasZoneIdPK, HasDatacenterPK, HasVendorPKFK):
+class ZoneBase(
+    MetaColumns,
+    HasDisplayName,
+    HasApiReference,
+    HasName,
+    HasZoneIdPK,
+    HasDatacenterPK,
+    HasVendorPKFK,
+):
     pass
 
 
 class StorageFields(HasDescription, HasName, HasStorageIdPK, HasVendorPKFK):
     storage_type: StorageType = Field(
         description="High-level category of the storage, e.g. HDD or SDD."
     )
@@ -446,15 +480,26 @@
     )
 
 
 class StorageBase(MetaColumns, StorageFields):
     pass
 
 
-class ServerFields(HasDescription, HasName, HasServerIdPK, HasVendorPKFK):
+class ServerFields(
+    HasDescription,
+    HasDisplayName,
+    HasApiReference,
+    HasName,
+    HasServerIdPK,
+    HasVendorPKFK,
+):
+    family: Optional[str] = Field(
+        default=None,
+        description="Server family, e.g. General-purpose machine (GCP), or M5g (AWS).",
+    )
     vcpus: int = Field(
         default=None,
         description="Default number of virtual CPUs (vCPU) of the server.",
     )
     hypervisor: Optional[str] = Field(
         default=None,
         description="Hypervisor of the virtual server, e.g. Xen, KVM, Nitro or Dedicated.",
```

### Comparing `sparecores_crawler-0.1.2/src/sc_crawler/table_fields.py` & `sparecores_crawler-0.1.3/src/sc_crawler/table_fields.py`

 * *Files identical despite different names*

### Comparing `sparecores_crawler-0.1.2/src/sc_crawler/tables.py` & `sparecores_crawler-0.1.3/src/sc_crawler/tables.py`

 * *Files identical despite different names*

### Comparing `sparecores_crawler-0.1.2/src/sc_crawler/tables_scd.py` & `sparecores_crawler-0.1.3/src/sc_crawler/tables_scd.py`

 * *Files identical despite different names*

### Comparing `sparecores_crawler-0.1.2/src/sc_crawler/utils.py` & `sparecores_crawler-0.1.3/src/sc_crawler/utils.py`

 * *Files identical despite different names*

### Comparing `sparecores_crawler-0.1.2/src/sc_crawler/vendors/aws.py` & `sparecores_crawler-0.1.3/src/sc_crawler/vendors/aws.py`

 * *Files 4% similar despite different names*

```diff
@@ -277,16 +277,19 @@
     gpu_info = _get_gpu_of_instance_type(instance_type)
     storage_info = _get_storage_of_instance_type(instance_type)
     network_card = instance_type["NetworkInfo"]["NetworkCards"][0]
     return {
         "server_id": it,
         "vendor_id": vendor.vendor_id,
         "name": it,
+        "api_reference": it,
+        "display_name": it,
         "description": _annotate_instance_type(it),
         "hypervisor": instance_type.get("Hypervisor", None),
+        "family": it.split(".")[0],
         "vcpus": vcpu_info["DefaultVCpus"],
         "cpu_allocation": allocation,
         "cpu_cores": vcpu_info["DefaultCores"],
         "cpu_speed": cpu_info.get("SustainedClockSpeedInGhz", None),
         "cpu_architecture": cpu_info["SupportedArchitectures"][0],
         "cpu_manufacturer": cpu_info.get("Manufacturer", None),
         "memory": instance_type["MemoryInfo"]["SizeInMiB"],
@@ -378,309 +381,390 @@
 
 
 def inventory_datacenters(vendor):
     """List all available AWS datacenters via `boto3` calls.
 
     Some data sources are not available from APIs, and were collected manually:
 
-    - launch date: <https://aws.amazon.com/about-aws/global-infrastructure/regions_az/>
-    - energy source: <https://sustainability.aboutamazon.com/products-services/the-cloud?energyType=true#renewable-energy>
+    - launch date: <https://aws.amazon.com/about-aws/global-infrastructure/regions_az/>,
+    - energy source: <https://sustainability.aboutamazon.com/products-services/the-cloud?energyType=true#renewable-energy>,
+    - lon/lat coordinates: <https://gist.github.com/martinheidegger/88950cb51ee5bdeafd51bc55287b1092> and approximation based on the city when no more accurate data was available.
     """  # noqa: E501
     datacenters = [
         {
             "datacenter_id": "af-south-1",
             "name": "Africa (Cape Town)",
             "vendor_id": vendor.vendor_id,
             "country_id": "ZA",
             "city": "Cape Town",
             "founding_year": 2020,
             "green_energy": False,
+            "lat": -33.914651,
+            "lon": 18.3758801,
         },
         {
             "datacenter_id": "ap-east-1",
             "name": "Asia Pacific (Hong Kong)",
             "vendor_id": vendor.vendor_id,
             "country_id": "HK",
             "city": "Hong Kong",
             "founding_year": 2019,
             "green_energy": False,
+            "lat": 22.2908475,
+            "lon": 114.2723379,
         },
         {
             "datacenter_id": "ap-northeast-1",
             "name": "Asia Pacific (Tokyo)",
             "vendor_id": vendor.vendor_id,
             "country_id": "JP",
             "city": "Tokyo",
             "founding_year": 2011,
             "green_energy": False,
+            "lat": 35.617436,
+            "lon": 139.7459176,
         },
         {
             "datacenter_id": "ap-northeast-2",
             "name": "Asia Pacific (Seoul)",
             "vendor_id": vendor.vendor_id,
             "country_id": "KR",
             "city": "Seoul",
             "founding_year": 2016,
             "green_energy": False,
+            "lat": 37.5616592,
+            "lon": 126.8736237,
         },
         {
             "datacenter_id": "ap-northeast-3",
             "name": "Asia Pacific (Osaka)",
             "vendor_id": vendor.vendor_id,
             "country_id": "JP",
             "city": "Osaka",
             "founding_year": 2021,
             "green_energy": False,
+            "lat": 34.693889,
+            "lon": 135.502222,
         },
         {
             "datacenter_id": "ap-south-1",
             "name": "Asia Pacific (Mumbai)",
             "vendor_id": vendor.vendor_id,
             "country_id": "IN",
             "city": "Mumbai",
             "founding_year": 2016,
             "green_energy": True,
+            "lat": 19.2425503,
+            "lon": 72.9667878,
         },
         {
             "datacenter_id": "ap-south-2",
             "name": "Asia Pacific (Hyderabad)",
             "vendor_id": vendor.vendor_id,
             "country_id": "IN",
             "city": "Hyderabad",
             "founding_year": 2022,
             "green_energy": True,
+            # approximation based on city location
+            "lat": 17.412281,
+            "lon": 78.243237,
         },
         {
             "datacenter_id": "ap-southeast-1",
             "name": "Asia Pacific (Singapore)",
             "vendor_id": vendor.vendor_id,
             "country_id": "SG",
             "city": "Singapore",
             "founding_year": 2010,
             "green_energy": False,
+            "lat": 1.3218269,
+            "lon": 103.6930643,
         },
         {
             "datacenter_id": "ap-southeast-2",
             "name": "Asia Pacific (Sydney)",
             "vendor_id": vendor.vendor_id,
             "country_id": "AU",
             "city": "Sydney",
             "founding_year": 2012,
             "green_energy": False,
+            "lat": -33.9117717,
+            "lon": 151.1907535,
         },
         {
             "datacenter_id": "ap-southeast-3",
             "name": "Asia Pacific (Jakarta)",
             "vendor_id": vendor.vendor_id,
             "country_id": "ID",
             "city": "Jakarta",
             "founding_year": 2021,
             "green_energy": False,
+            "lat": -6.2,
+            "lon": 106.816667,
         },
         {
             "datacenter_id": "ap-southeast-4",
             "name": "Asia Pacific (Melbourne)",
             "vendor_id": vendor.vendor_id,
             "country_id": "AU",
             "city": "Melbourne",
             "founding_year": 2023,
             "green_energy": False,
+            # approximation based on city location
+            "lat": -37.8038607,
+            "lon": 144.7119569,
         },
         {
             "datacenter_id": "ca-central-1",
             "name": "Canada (Central)",
             "vendor_id": vendor.vendor_id,
             "country_id": "CA",
             "city": "Quebec",  # NOTE needs city name
             "founding_year": 2016,
             "green_energy": True,
+            "lat": 45.5,
+            "lon": -73.6,
         },
         {
             "datacenter_id": "ca-west-1",
             "name": "Canada West (Calgary)",
             "vendor_id": vendor.vendor_id,
             "country_id": "CA",
             "city": "Calgary",
             "founding_year": 2023,
             "green_energy": False,
+            # approximation based on city location
+            "lat": -37.8038607,
+            "lon": 144.7119569,
         },
         {
             "datacenter_id": "cn-north-1",
             "name": "China (Beijing)",
             "vendor_id": vendor.vendor_id,
             "country_id": "CN",
             "city": "Beijing",
             "founding_year": 2016,
             "green_energy": True,
+            "lat": 39.8094478,
+            "lon": 116.5783234,
         },
         {
             "datacenter_id": "cn-northwest-1",
             "name": "China (Ningxia)",
             "vendor_id": vendor.vendor_id,
             "country_id": "CN",
             "city": "Ningxia",  # NOTE needs city name
             "founding_year": 2017,
             "green_energy": True,
+            "lat": 37.5024418,
+            "lon": 105.1627193,
         },
         {
             "datacenter_id": "eu-central-1",
             "name": "Europe (Frankfurt)",
             "aliases": ["EU (Frankfurt)"],
             "vendor_id": vendor.vendor_id,
             "country_id": "DE",
             "city": "Frankfurt",
             "founding_year": 2014,
             "green_energy": True,
+            "lat": 50.0992094,
+            "lon": 8.6303932,
         },
         {
             "datacenter_id": "eu-central-2",
             "name": "Europe (Zurich)",
             "vendor_id": vendor.vendor_id,
             "country_id": "CH",
             "city": "Zurich",
             "founding_year": 2022,
             "green_energy": True,
+            # approximation based on city location
+            "lat": 47.3862924,
+            "lon": 8.4448814,
         },
         {
             "datacenter_id": "eu-north-1",
             "name": "Europe (Stockholm)",
             "aliases": ["EU (Stockholm)"],
             "vendor_id": vendor.vendor_id,
             "country_id": "SE",
             "city": "Stockholm",
             "founding_year": 2018,
             "green_energy": True,
+            "lat": 59.326242,
+            "lon": 17.8419717,
         },
         {
             "datacenter_id": "eu-south-1",
             "name": "Europe (Milan)",
             "aliases": ["EU (Milan)"],
             "vendor_id": vendor.vendor_id,
             "country_id": "IT",
             "city": "Milan",
             "founding_year": 2020,
             "green_energy": True,
+            "lat": 45.4628328,
+            "lon": 9.1076927,
         },
         {
             "datacenter_id": "eu-south-2",
             "name": "Europe (Spain)",
             "vendor_id": vendor.vendor_id,
             "country_id": "ES",
             "city": "Aragón",  # NOTE needs city name
             "founding_year": 2022,
             "green_energy": True,
+            # approximation based on city location
+            "lat": 41.7943702,
+            "lon": -0.8516735,
         },
         {
             "datacenter_id": "eu-west-1",
             "name": "Europe (Ireland)",
             "aliases": ["EU (Ireland)"],
             "vendor_id": vendor.vendor_id,
             "country_id": "IE",
             "city": "Dublin",
             "founding_year": 2007,
             "green_energy": True,
+            "lat": 53.4056545,
+            "lon": -6.224503,
         },
         {
             "datacenter_id": "eu-west-2",
             "name": "Europe (London)",
             "aliases": ["EU (London)"],
             "vendor_id": vendor.vendor_id,
             "country_id": "GB",
             "city": "London",
             "founding_year": 2016,
             "green_energy": True,
+            "lat": 51.5085036,
+            "lon": -0.0609266,
         },
         {
             "datacenter_id": "eu-west-3",
             "name": "Europe (Paris)",
             "aliases": ["EU (Paris)"],
             "vendor_id": vendor.vendor_id,
             "country_id": "FR",
             "city": "Paris",
             "founding_year": 2017,
             "green_energy": True,
+            "lat": 48.6009709,
+            "lon": 2.2976644,
         },
         {
             "datacenter_id": "il-central-1",
             "name": "Israel (Tel Aviv)",
             "vendor_id": vendor.vendor_id,
             "country_id": "IL",
             "city": "Tel Aviv",
             "founding_year": 2023,
             "green_energy": False,
+            # approximation based on city location
+            "lat": 32.0491183,
+            "lon": 34.7891105,
         },
         {
             "datacenter_id": "me-central-1",
             "name": "Middle East (UAE)",
             "vendor_id": vendor.vendor_id,
             "country_id": "AE",
-            # NOTE city unknown
+            # NOTE city and state unknown
+            "display_name": "United Arab Emirates",
             "founding_year": 2022,
             "green_energy": False,
+            # approximation based on country
+            "lat": 25.0647937,
+            "lon": 55.1363688,
         },
         {
             "datacenter_id": "me-south-1",
             "name": "Middle East (Bahrain)",
             "vendor_id": vendor.vendor_id,
             "country_id": "BH",
-            # NOTE city unknown
+            # NOTE city and stateunknown
+            "display_name": "Bahrain",
             "founding_year": 2019,
             "green_energy": False,
+            "lat": 25.941298,
+            "lon": 50.3073907,
         },
         {
             "datacenter_id": "sa-east-1",
             "name": "South America (Sao Paulo)",
             "vendor_id": vendor.vendor_id,
             "country_id": "BR",
             "city": "Sao Paulo",
             "founding_year": 2011,
             "green_energy": False,
+            "lat": -23.4925798,
+            "lon": -46.8105593,
         },
         {
             "datacenter_id": "us-east-1",
             "name": "US East (N. Virginia)",
             "vendor_id": vendor.vendor_id,
             "country_id": "US",
             "state": "Northern Virgina",
             # NOTE city unknown
             "founding_year": 2006,
             "green_energy": True,
+            "lat": 38.9940541,
+            "lon": -77.4524237,
         },
         {
             "datacenter_id": "us-east-2",
             "name": "US East (Ohio)",
             "vendor_id": vendor.vendor_id,
             "country_id": "US",
             "state": "Ohio",
             # NOTE city unknown
             "founding_year": 2016,
             "green_energy": True,
+            "lat": 40.0946354,
+            "lon": -82.7541337,
         },
         {
             "datacenter_id": "us-west-1",
             "name": "US West (N. California)",
             "vendor_id": vendor.vendor_id,
             "country_id": "US",
             "state": "California",
             # NOTE city unknown
             "founding_year": 2009,
             "green_energy": True,
+            "lat": 37.443680,
+            "lon": -122.153664,
         },
         {
             "datacenter_id": "us-west-2",
             "name": "US West (Oregon)",
             "vendor_id": vendor.vendor_id,
             "country_id": "US",
             "state": "Oregon",
             # NOTE city unknown
             "founding_year": 2011,
             "green_energy": True,
+            "lat": 45.9174667,
+            "lon": -119.2684488,
         },
     ]
 
+    # add API reference and display names
+    for datacenter in datacenters:
+        datacenter["api_reference"] = datacenter["datacenter_id"]
+        if datacenter.get("display_name") is None:
+            display_name_prefix = datacenter.get("city", datacenter.get("state", ""))
+            datacenter["display_name"] = (
+                f"{display_name_prefix} ({datacenter['country_id']})"
+            )
+
     # look for undocumented (new) regions in AWS
     supported_regions = [d["datacenter_id"] for d in datacenters]
     regions = _boto_describe_regions()
     for region in regions:
         region_name = region["RegionName"]
         if "gov" in region_name:
             next()
@@ -708,14 +792,16 @@
         new = []
         if datacenter.status == "active":
             for zone in _boto_describe_availability_zones(datacenter.datacenter_id):
                 new.append(
                     {
                         "zone_id": zone["ZoneId"],
                         "name": zone["ZoneName"],
+                        "api_reference": zone["ZoneName"],
+                        "display_name": zone["ZoneName"],
                         "datacenter_id": datacenter.datacenter_id,
                         "vendor_id": vendor.vendor_id,
                     }
                 )
         vendor.progress_tracker.advance_task()
         return new
```

### Comparing `sparecores_crawler-0.1.2/src/sc_crawler/vendors/gcp.py` & `sparecores_crawler-0.1.3/src/sc_crawler/vendors/gcp.py`

 * *Files 6% similar despite different names*

```diff
@@ -358,278 +358,394 @@
 
 
 def inventory_datacenters(vendor):
     """List all available GCP regions via API calls.
 
     Some data sources are not available from APIs, and were collected manually:
 
-    - location: <https://cloud.google.com/compute/docs/regions-zones#available> and <https://en.wikipedia.org/wiki/Google_data_centers>
-    - energy carbon data: <https://cloud.google.com/sustainability/region-carbon#data> and <https://github.com/GoogleCloudPlatform/region-carbon-info>
-    - launch dates were collected from [Wikipedia](https://en.wikipedia.org/wiki/Google_Cloud_Platform#Regions_and_zones) and GCP blog posts, such as <https://medium.com/@retomeier/an-annotated-history-of-googles-cloud-platform-90b90f948920> and <https://cloud.google.com/blog/products/infrastructure/introducing-new-google-cloud-regions>
+    - location: <https://cloud.google.com/compute/docs/regions-zones#available> and <https://en.wikipedia.org/wiki/Google_data_centers>,
+    - lon/lat coordinates: <https://en.wikipedia.org/wiki/Google_data_centers#Locations> and approximation based on the city when no more accurate data was available.
+    - energy carbon data: <https://cloud.google.com/sustainability/region-carbon#data> and <https://github.com/GoogleCloudPlatform/region-carbon-info>,
+    - launch dates were collected from [Wikipedia](https://en.wikipedia.org/wiki/Google_Cloud_Platform#Regions_and_zones) and GCP blog posts, such as <https://medium.com/@retomeier/an-annotated-history-of-googles-cloud-platform-90b90f948920> and <https://cloud.google.com/blog/products/infrastructure/introducing-new-google-cloud-regions>.
 
     Note that many GCP datacenters use more than 90% green energy,
     but the related flag in our database is set to `False` as not being 100%.
     """
 
     manual_data = {
         "africa-south1": {
             "country_id": "ZA",
             "city": "Johannesburg",
             # https://cloud.google.com/blog/products/infrastructure/heita-south-africa-new-cloud-region
             "founding_year": 2024,
             "green_energy": False,
+            # approximation based on city
+            "lat": 26.0420631,
+            "long": 28.0589808,
         },
         "asia-east1": {
             "country_id": "TW",
             "state": "Changhua County",
             "founding_year": 2013,
             "green_energy": False,
+            "lat": -33.520515,
+            "long": -70.72169,
         },
         "asia-east2": {
             "country_id": "HK",
             # https://cloud.google.com/blog/products/gcp/gcps-region-in-hong-kong-is-now-open
             "founding_year": 2018,
             "green_energy": False,
+            # approximation based on country
+            "lat": 22.2772377,
+            "long": 114.1703066,
+            "display_name": "Hong Kong",
         },
         "asia-northeast1": {
             "country_id": "JP",
             "city": "Tokyo",
             "state": "Japan",
             "founding_year": 2016,
             "green_energy": False,
+            # approximation based on city
+            "lat": 35.6433846,
+            "lon": 139.7684933,
         },
         "asia-northeast2": {
             "country_id": "JP",
             "city": "Osaka",
             "founding_year": 2019,
             "green_energy": False,
+            # approximation based on city
+            "lat": 34.6696646,
+            "lon": 135.4846612,
         },
         "asia-northeast3": {
             "country_id": "KR",
             "city": "Seoul",
             "founding_year": 2020,
             "green_energy": False,
+            # approximation based on city
+            "lat": 37.5514982,
+            "lon": 126.97784,
         },
         "asia-south1": {
             "country_id": "IN",
             "city": "Mumbai",
             "founding_year": 2017,
             "green_energy": False,
+            # approximation based on city
+            "lat": 19.0709441,
+            "lon": 72.8726468,
         },
         "asia-south2": {
             "country_id": "IN",
             "city": "Delhi",
             "founding_year": 2021,
             "green_energy": False,
+            # approximation based on city
+            "lat": 28.6439839,
+            "lon": 76.9284239,
         },
         "asia-southeast1": {
             "country_id": "SG",
             "city": "Jurong West",
             "founding_year": 2017,
             "green_energy": False,
+            "lat": 1.351333,
+            "lon": 103.709778,
         },
         "asia-southeast2": {
             "country_id": "ID",
             "city": "Jakarta",
             "founding_year": 2020,
             "green_energy": False,
+            # approximation based on city
+            "lat": -6.2297401,
+            "lon": 106.747117,
         },
         "australia-southeast1": {
             "country_id": "AU",
             "city": "Sydney",
             "founding_year": 2017,
             "green_energy": False,
+            # approximation based on city
+            "lat": -33.8375583,
+            "lon": 150.9488095,
         },
         "australia-southeast2": {
             "country_id": "AU",
             "city": "Melbourne",
             "founding_year": 2021,
             "green_energy": False,
+            # approximation based on city
+            "lat": -37.8038607,
+            "lon": 144.7119569,
         },
         "europe-central2": {
             "country_id": "PL",
             "city": "Warsaw",
             "founding_year": 2021,
             "green_energy": False,
+            # approximation based on city
+            "lat": 52.2328871,
+            "lon": 20.8966164,
         },
         "europe-north1": {
             "country_id": "FI",
             "city": "Hamina",
             "founding_year": 2018,
             "green_energy": False,
+            "lat": 60.536578,
+            "lon": 27.117003,
         },
         "europe-southwest1": {
             "country_id": "ES",
             "city": "Madrid",
             "founding_year": 2022,
             "green_energy": False,
+            "lat": 40.519533,
+            "lon": -3.340937,
         },
         "europe-west1": {
             "country_id": "BE",
             "city": "St. Ghislain",
             # https://medium.com/@retomeier/an-annotated-history-of-googles-cloud-platform-90b90f948920
             "founding_year": 2015,
             "green_energy": False,
+            "lat": 50.469333,
+            "lon": 3.865472,
         },
         "europe-west10": {
             "country_id": "DE",
             "city": "Berlin",
             "founding_year": 2023,
             "green_energy": False,
+            # approximation based on city
+            "lat": 52.5105672,
+            "lon": 13.3806972,
         },
         "europe-west12": {
             "country_id": "IT",
             "city": "Turin",
             "founding_year": 2023,
             "green_energy": False,
+            "lat": 45.146729,
+            "lon": 7.742147,
         },
         "europe-west2": {
             "country_id": "GB",
             "city": "London",
             "founding_year": 2017,
             "green_energy": False,
+            # approximation based on city
+            "lat": 51.5090133,
+            "lon": -0.2118157,
         },
         "europe-west3": {
             "country_id": "DE",
             "city": "Frankfurt",
             "founding_year": 2017,
             "green_energy": False,
+            "lat": 50.12263,
+            "lon": 8.974168,
         },
         "europe-west4": {
             "country_id": "NL",
             "city": "Eemshaven",
             "founding_year": 2018,
             "green_energy": False,
+            "lat": 52.790105,
+            "lon": 5.029219,
         },
         "europe-west6": {
             "country_id": "CH",
             "city": "Zurich",
             "founding_year": 2019,
             "green_energy": False,
+            "lat": 47.445926,
+            "lon": 8.210909,
         },
         "europe-west8": {
             "country_id": "IT",
             "city": "Milan",
             "founding_year": 2022,
             "green_energy": False,
+            # approximation based on city
+            "lat": 45.4615551,
+            "lon": 9.1389572,
         },
         "europe-west9": {
             "country_id": "FR",
             "city": "Paris",
             "founding_year": 2022,
             "green_energy": False,
+            # approximation based on city
+            "lat": 48.8641797,
+            "lon": 2.3109137,
         },
         "me-central1": {
             "country_id": "QA",
             "city": "Doha",
             "founding_year": 2023,
             "green_energy": False,
+            # approximation based on city
+            "lat": 25.272868,
+            "lon": 51.4717522,
         },
         "me-central2": {
             "country_id": "SA",
             "city": "Dammam",
             "founding_year": 2023,
             "green_energy": False,
+            # approximation based on city
+            "lat": 26.3826288,
+            "lon": 49.9675732,
         },
         "me-west1": {
             "country_id": "IL",
             "city": "Tel Aviv",
             "founding_year": 2022,
             "green_energy": False,
+            # approximation based on city
+            "lat": 32.0491183,
+            "lon": 34.7891105,
         },
         "northamerica-northeast1": {
             "country_id": "CA",
             "city": "Montréal",
             "founding_year": 2018,
             "green_energy": True,
+            # approximation based on city
+            "lat": 45.4933996,
+            "lon": -73.728239,
         },
         "northamerica-northeast2": {
             "country_id": "CA",
             "city": "Toronto",
             "founding_year": 2021,
             "green_energy": False,
+            # approximation based on city
+            "lat": 43.72666,
+            "lon": -79.5355309,
         },
         "southamerica-east1": {
             "country_id": "BR",
             "city": "Osasco",
             "state": "São Paulo",
             "founding_year": 2017,
             "green_energy": False,
+            # approximation based on city
+            "lat": -23.5267431,
+            "lon": -46.8096539,
         },
         "southamerica-west1": {
             "country_id": "CL",
             "city": "Santiago",
             "founding_year": 2021,
             "green_energy": False,
+            "lat": -33.520515,
+            "lon": -70.721695,
         },
         "us-central1": {
             "country_id": "US",
             "city": "Council Bluffs",
             "state": "Iowa",
             "founding_year": 2009,
             "green_energy": False,
+            "lat": 41.168253,
+            "lon": -95.796125,
         },
         "us-east1": {
             "country_id": "US",
             "city": "Moncks Corner",
             "state": "South Carolina",
             "founding_year": 2015,
             "green_energy": False,
+            "lat": 33.064111,
+            "lon": -80.043361,
         },
         "us-east4": {
             "country_id": "US",
             "city": "Ashburn",
             "state": "Virginia",
             "founding_year": 2017,
             "green_energy": False,
+            "lat": 38.943331,
+            "lon": -77.524336,
         },
         "us-east5": {
             "country_id": "US",
             "city": "Columbus",
             "state": "Ohio",
             "founding_year": 2022,
             "green_energy": False,
+            # approximation based on city
+            "lat": 39.9773124,
+            "lon": -83.0423282,
         },
         "us-south1": {
             "country_id": "US",
             "city": "Dallas",
             "state": "Texas",
             "founding_year": 2022,
             "green_energy": False,
+            "lat": 32.44317,
+            "lon": -97.062324,
         },
         "us-west1": {
             "country_id": "US",
             "city": "The Dalles",
             "state": "Oregon",
             "founding_year": 2016,
             "green_energy": False,
+            "lat": 45.632511,
+            "lon": -121.202267,
         },
         "us-west2": {
             "country_id": "US",
             "city": "Los Angeles",
             "state": "California",
             "founding_year": 2018,
             "green_energy": False,
+            # approximation based on city
+            "lat": 34.0549694,
+            "lon": -118.3753618,
         },
         "us-west3": {
             "country_id": "US",
             "city": "Salt Lake City",
             "state": "Utah",
             "founding_year": 2020,
             "green_energy": False,
+            # approximation based on city
+            "lat": 40.7386099,
+            "lon": -111.9609998,
         },
         "us-west4": {
             "country_id": "US",
             "city": "Las Vegas",
             "state": "Nevada",
             "founding_year": 2020,
             "green_energy": False,
+            "lat": 36.055625,
+            "lon": -115.010226,
         },
     }
 
+    # add API reference and display names
+    for k, v in manual_data.items():
+        v["api_reference"] = k
+        if v.get("display_name") is None:
+            v["display_name"] = v.get("city", v.get("state", ""))
+            if v.get("display_name"):
+                v["display_name"] = v["display_name"] + " (" + v["country_id"] + ")"
+            else:
+                v["display_name"] = v["country_id"]
+
     regions = _regions()
     items = []
     for region in regions:
         if region.name not in manual_data:
             raise KeyError(f"Unknown datacenter metadata for {region.name}")
         item = {
             "vendor_id": vendor.vendor_id,
@@ -651,14 +767,16 @@
             {
                 "vendor_id": vendor.vendor_id,
                 # example `zone.region`:
                 # https://www.googleapis.com/compute/v1/projects/algebraic-pier-412621/regions/us-east4
                 "datacenter_id": datacenters[zone.region.split("/")[-1]].datacenter_id,
                 "zone_id": str(zone.id),
                 "name": zone.name,
+                "api_reference": zone.name,
+                "display_name": zone.name,
             }
         )
     return items
 
 
 def inventory_servers(vendor):
     """List all available GCP servers available in all zones."""
@@ -670,15 +788,18 @@
         zone_servers = []
         for server in _servers(zone.name):
             zone_servers.append(
                 {
                     "vendor_id": vendor.vendor_id,
                     "server_id": str(server.id),
                     "name": server.name,
+                    "api_reference": server.name,
+                    "display_name": server.name,
                     "description": server.description,
+                    "family": server.name.split("-")[0],
                     "vcpus": server.guest_cpus,
                     "hypervisor": None,
                     "cpu_allocation": (
                         CpuAllocation.SHARED
                         if server.is_shared_cpu
                         else CpuAllocation.DEDICATED
                     ),
```

### Comparing `sparecores_crawler-0.1.2/src/sc_crawler/vendors/hcloud.py` & `sparecores_crawler-0.1.3/src/sc_crawler/vendors/hcloud.py`

 * *Files 3% similar despite different names*

```diff
@@ -75,29 +75,62 @@
 
     Not taking the Hetzner unique `name` as id, as it's not
     stated to be unique for other resources, and uniqueness
     for servers might also change in the future.
 
     All datacenters are powered by green energy as per
     <https://www.hetzner.com/unternehmen/umweltschutz/>.
+
+    Lon/lat coordinates were collected by searching for Hetzner
+    locations in the Datacenter's city.
+
     """
+    datacenters = {
+        "2": {  # Nuremberg
+            "lat": 49.4498349,
+            "lon": 11.0128772,
+        },
+        "3": {  # Helsinki
+            "lat": 60.3433291,
+            "lon": 25.02683,
+        },
+        "4": {  # Falkenstein
+            "lat": 50.4793313,
+            "lon": 12.3331105,
+        },
+        "5": {  # Ashburn, VA
+            "lat": 39.0176685,
+            "lon": -77.468102,
+        },
+        "6": {  # Hillsboro, OR
+            "lat": 45.558319,
+            "lon": -122.9306602,
+        },
+    }
+
     items = []
     for datacenter in _client().datacenters.get_all():
         items.append(
             {
                 "vendor_id": vendor.vendor_id,
                 "datacenter_id": str(datacenter.id),
                 "name": datacenter.name,
+                "api_reference": datacenter.name,
+                "display_name": (
+                    datacenter.location.city + f" ({datacenter.location.country})"
+                ),
                 # TODO add datacenter.description
                 "aliases": [datacenter.location.name],
                 "country_id": datacenter.location.country,
                 "state": None,
                 "city": datacenter.location.city,
                 "address_line": None,
                 "zip_code": None,
+                "lat": datacenters[str(datacenter.id)]["lat"],
+                "lon": datacenters[str(datacenter.id)]["lon"],
                 "founding_year": None,
                 "green_energy": True,
             }
         )
     return items
 
 
@@ -112,14 +145,16 @@
     for datacenter in vendor.datacenters:
         items.append(
             {
                 "vendor_id": vendor.vendor_id,
                 "datacenter_id": datacenter.datacenter_id,
                 "zone_id": datacenter.datacenter_id,
                 "name": datacenter.name,
+                "api_reference": datacenter.name,
+                "display_name": datacenter.name,
             }
         )
     return items
 
 
 def inventory_servers(vendor):
     """List all server types from API and manual data entry from the Hetzner Cloud homepage.
@@ -131,15 +166,18 @@
         # collected from https://www.hetzner.com/cloud/
         cpu = _server_cpu(server.name)
         items.append(
             {
                 "vendor_id": vendor.vendor_id,
                 "server_id": str(server.id),
                 "name": server.name,
+                "api_reference": server.name,
+                "display_name": server.name,
                 "description": server.description,
+                "family": server.name.rstrip("0123456789"),
                 "vcpus": server.cores,
                 "hypervisor": None,
                 "cpu_allocation": (
                     CpuAllocation.SHARED
                     if server.cpu_type == "shared"
                     else CpuAllocation.DEDICATED
                 ),
```

### Comparing `sparecores_crawler-0.1.2/src/sc_crawler/vendors/vendors.py` & `sparecores_crawler-0.1.3/src/sc_crawler/vendors/vendors.py`

 * *Files identical despite different names*

### Comparing `sparecores_crawler-0.1.2/src/sparecores_crawler.egg-info/PKG-INFO` & `sparecores_crawler-0.1.3/src/sparecores_crawler.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sparecores-crawler
-Version: 0.1.2
+Version: 0.1.3
 Summary: Pull and standardize data on cloud compute resources.
 Author: Attila Nagy, Gergely Daroczi, Balazs Hodobay
 Maintainer-email: Spare Cores team <pkg@sparecores.com>
 Project-URL: repository, https://github.com/SpareCores/sc-crawler
 Project-URL: issues, https://github.com/SpareCores/sc-crawler/issues
 Project-URL: documentation, https://sparecores.github.io/sc-crawler/
 Project-URL: homepage, https://sparecores.com
```

### Comparing `sparecores_crawler-0.1.2/src/sparecores_crawler.egg-info/SOURCES.txt` & `sparecores_crawler-0.1.3/src/sparecores_crawler.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -14,14 +14,16 @@
 src/sc_crawler/table_fields.py
 src/sc_crawler/tables.py
 src/sc_crawler/tables_scd.py
 src/sc_crawler/utils.py
 src/sc_crawler/alembic/env.py
 src/sc_crawler/alembic/versions/4691089690c2_v0_1_1.py
 src/sc_crawler/alembic/versions/98894dffd37c_v0_1_0.py
+src/sc_crawler/alembic/versions/f6bf6152039a_v0_1_3_step2.py
+src/sc_crawler/alembic/versions/f6edf4a96a78_v0_1_3_step1.py
 src/sc_crawler/vendors/__init__.py
 src/sc_crawler/vendors/aws.py
 src/sc_crawler/vendors/gcp.py
 src/sc_crawler/vendors/hcloud.py
 src/sc_crawler/vendors/vendors.py
 src/sparecores_crawler.egg-info/PKG-INFO
 src/sparecores_crawler.egg-info/SOURCES.txt
```

### Comparing `sparecores_crawler-0.1.2/src/sparecores_crawler.egg-info/requires.txt` & `sparecores_crawler-0.1.3/src/sparecores_crawler.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `sparecores_crawler-0.1.2/tests/test_schemas.py` & `sparecores_crawler-0.1.3/tests/test_schemas.py`

 * *Files identical despite different names*

### Comparing `sparecores_crawler-0.1.2/tests/test_str_utils.py` & `sparecores_crawler-0.1.3/tests/test_str_utils.py`

 * *Files identical despite different names*

### Comparing `sparecores_crawler-0.1.2/tests/test_utils.py` & `sparecores_crawler-0.1.3/tests/test_utils.py`

 * *Files identical despite different names*

