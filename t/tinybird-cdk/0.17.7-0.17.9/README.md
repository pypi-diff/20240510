# Comparing `tmp/tinybird_cdk-0.17.7.tar.gz` & `tmp/tinybird_cdk-0.17.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tinybird_cdk-0.17.7.tar", last modified: Fri Apr 19 14:00:09 2024, max compression
+gzip compressed data, was "tinybird_cdk-0.17.9.tar", last modified: Fri Apr 19 14:33:50 2024, max compression
```

## Comparing `tinybird_cdk-0.17.7.tar` & `tinybird_cdk-0.17.9.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:00:09.291656 tinybird_cdk-0.17.7/
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-19 14:00:04.000000 tinybird_cdk-0.17.7/DESCRIPTION.md
--rw-r--r--   0 runner    (1001) docker     (127)     1031 2024-04-19 14:00:09.291656 tinybird_cdk-0.17.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    26052 2024-04-19 14:00:04.000000 tinybird_cdk-0.17.7/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      635 2024-04-19 14:00:04.000000 tinybird_cdk-0.17.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-19 14:00:04.000000 tinybird_cdk-0.17.7/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)      361 2024-04-19 14:00:04.000000 tinybird_cdk-0.17.7/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 14:00:09.291656 tinybird_cdk-0.17.7/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:00:09.283656 tinybird_cdk-0.17.7/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1970 2024-04-19 14:00:04.000000 tinybird_cdk-0.17.7/tests/test_gcp.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:00:09.287656 tinybird_cdk-0.17.7/tinybird_cdk/
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-04-19 14:00:04.000000 tinybird_cdk-0.17.7/tinybird_cdk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:00:09.287656 tinybird_cdk-0.17.7/tinybird_cdk/cloud/
--rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-04-19 14:00:04.000000 tinybird_cdk-0.17.7/tinybird_cdk/cloud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2025 2024-04-19 14:00:04.000000 tinybird_cdk-0.17.7/tinybird_cdk/cloud/abstract_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1474 2024-04-19 14:00:04.000000 tinybird_cdk-0.17.7/tinybird_cdk/cloud/gcp.py
--rw-r--r--   0 runner    (1001) docker     (127)     4159 2024-04-19 14:00:04.000000 tinybird_cdk-0.17.7/tinybird_cdk/cloud/gcs.py
--rw-r--r--   0 runner    (1001) docker     (127)     4946 2024-04-19 14:00:04.000000 tinybird_cdk-0.17.7/tinybird_cdk/cloud/s3.py
--rw-r--r--   0 runner    (1001) docker     (127)      764 2024-04-19 14:00:04.000000 tinybird_cdk-0.17.7/tinybird_cdk/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     7729 2024-04-19 14:00:04.000000 tinybird_cdk-0.17.7/tinybird_cdk/connector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:00:09.291656 tinybird_cdk-0.17.7/tinybird_cdk/connectors/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 14:00:04.000000 tinybird_cdk-0.17.7/tinybird_cdk/connectors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10438 2024-04-19 14:00:04.000000 tinybird_cdk-0.17.7/tinybird_cdk/connectors/bigquery.py
--rw-r--r--   0 runner    (1001) docker     (127)      320 2024-04-19 14:00:04.000000 tinybird_cdk-0.17.7/tinybird_cdk/connectors/gcs.py
--rw-r--r--   0 runner    (1001) docker     (127)      671 2024-04-19 14:00:04.000000 tinybird_cdk-0.17.7/tinybird_cdk/connectors/kinesis.py
--rw-r--r--   0 runner    (1001) docker     (127)     1657 2024-04-19 14:00:04.000000 tinybird_cdk-0.17.7/tinybird_cdk/connectors/mysql.py
--rw-r--r--   0 runner    (1001) docker     (127)     2152 2024-04-19 14:00:04.000000 tinybird_cdk-0.17.7/tinybird_cdk/connectors/postgresql.py
--rw-r--r--   0 runner    (1001) docker     (127)      318 2024-04-19 14:00:04.000000 tinybird_cdk-0.17.7/tinybird_cdk/connectors/s3.py
--rw-r--r--   0 runner    (1001) docker     (127)    17899 2024-04-19 14:00:04.000000 tinybird_cdk-0.17.7/tinybird_cdk/connectors/snowflake.py
--rw-r--r--   0 runner    (1001) docker     (127)     1595 2024-04-19 14:00:04.000000 tinybird_cdk-0.17.7/tinybird_cdk/connectors/sqlite.py
--rw-r--r--   0 runner    (1001) docker     (127)     2831 2024-04-19 14:00:04.000000 tinybird_cdk-0.17.7/tinybird_cdk/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)      840 2024-04-19 14:00:04.000000 tinybird_cdk-0.17.7/tinybird_cdk/export.py
--rw-r--r--   0 runner    (1001) docker     (127)      514 2024-04-19 14:00:04.000000 tinybird_cdk-0.17.7/tinybird_cdk/formats.py
--rw-r--r--   0 runner    (1001) docker     (127)      515 2024-04-19 14:00:04.000000 tinybird_cdk-0.17.7/tinybird_cdk/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     3694 2024-04-19 14:00:04.000000 tinybird_cdk-0.17.7/tinybird_cdk/migration.py
--rw-r--r--   0 runner    (1001) docker     (127)     5546 2024-04-19 14:00:04.000000 tinybird_cdk-0.17.7/tinybird_cdk/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)    12911 2024-04-19 14:00:04.000000 tinybird_cdk-0.17.7/tinybird_cdk/tinybird.py
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-04-19 14:00:04.000000 tinybird_cdk-0.17.7/tinybird_cdk/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:00:09.291656 tinybird_cdk-0.17.7/tinybird_cdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1031 2024-04-19 14:00:09.000000 tinybird_cdk-0.17.7/tinybird_cdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      993 2024-04-19 14:00:09.000000 tinybird_cdk-0.17.7/tinybird_cdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 14:00:09.000000 tinybird_cdk-0.17.7/tinybird_cdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      343 2024-04-19 14:00:09.000000 tinybird_cdk-0.17.7/tinybird_cdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-19 14:00:09.000000 tinybird_cdk-0.17.7/tinybird_cdk.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:33:50.865026 tinybird_cdk-0.17.9/
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-19 14:33:46.000000 tinybird_cdk-0.17.9/DESCRIPTION.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-04-19 14:33:50.865026 tinybird_cdk-0.17.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    26054 2024-04-19 14:33:46.000000 tinybird_cdk-0.17.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      636 2024-04-19 14:33:46.000000 tinybird_cdk-0.17.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-19 14:33:46.000000 tinybird_cdk-0.17.9/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2024-04-19 14:33:46.000000 tinybird_cdk-0.17.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 14:33:50.865026 tinybird_cdk-0.17.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:33:50.857026 tinybird_cdk-0.17.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1970 2024-04-19 14:33:46.000000 tinybird_cdk-0.17.9/tests/test_gcp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:33:50.857026 tinybird_cdk-0.17.9/tinybird_cdk/
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-04-19 14:33:46.000000 tinybird_cdk-0.17.9/tinybird_cdk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:33:50.861026 tinybird_cdk-0.17.9/tinybird_cdk/cloud/
+-rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-04-19 14:33:46.000000 tinybird_cdk-0.17.9/tinybird_cdk/cloud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2025 2024-04-19 14:33:46.000000 tinybird_cdk-0.17.9/tinybird_cdk/cloud/abstract_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1474 2024-04-19 14:33:46.000000 tinybird_cdk-0.17.9/tinybird_cdk/cloud/gcp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4159 2024-04-19 14:33:46.000000 tinybird_cdk-0.17.9/tinybird_cdk/cloud/gcs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4946 2024-04-19 14:33:46.000000 tinybird_cdk-0.17.9/tinybird_cdk/cloud/s3.py
+-rw-r--r--   0 runner    (1001) docker     (127)      764 2024-04-19 14:33:46.000000 tinybird_cdk-0.17.9/tinybird_cdk/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7729 2024-04-19 14:33:46.000000 tinybird_cdk-0.17.9/tinybird_cdk/connector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:33:50.861026 tinybird_cdk-0.17.9/tinybird_cdk/connectors/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 14:33:46.000000 tinybird_cdk-0.17.9/tinybird_cdk/connectors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10438 2024-04-19 14:33:46.000000 tinybird_cdk-0.17.9/tinybird_cdk/connectors/bigquery.py
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-04-19 14:33:46.000000 tinybird_cdk-0.17.9/tinybird_cdk/connectors/gcs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      671 2024-04-19 14:33:46.000000 tinybird_cdk-0.17.9/tinybird_cdk/connectors/kinesis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1657 2024-04-19 14:33:46.000000 tinybird_cdk-0.17.9/tinybird_cdk/connectors/mysql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2152 2024-04-19 14:33:46.000000 tinybird_cdk-0.17.9/tinybird_cdk/connectors/postgresql.py
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-04-19 14:33:46.000000 tinybird_cdk-0.17.9/tinybird_cdk/connectors/s3.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17899 2024-04-19 14:33:46.000000 tinybird_cdk-0.17.9/tinybird_cdk/connectors/snowflake.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1595 2024-04-19 14:33:46.000000 tinybird_cdk-0.17.9/tinybird_cdk/connectors/sqlite.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2831 2024-04-19 14:33:46.000000 tinybird_cdk-0.17.9/tinybird_cdk/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)      840 2024-04-19 14:33:46.000000 tinybird_cdk-0.17.9/tinybird_cdk/export.py
+-rw-r--r--   0 runner    (1001) docker     (127)      514 2024-04-19 14:33:46.000000 tinybird_cdk-0.17.9/tinybird_cdk/formats.py
+-rw-r--r--   0 runner    (1001) docker     (127)      515 2024-04-19 14:33:46.000000 tinybird_cdk-0.17.9/tinybird_cdk/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3694 2024-04-19 14:33:46.000000 tinybird_cdk-0.17.9/tinybird_cdk/migration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5546 2024-04-19 14:33:46.000000 tinybird_cdk-0.17.9/tinybird_cdk/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12911 2024-04-19 14:33:46.000000 tinybird_cdk-0.17.9/tinybird_cdk/tinybird.py
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-04-19 14:33:46.000000 tinybird_cdk-0.17.9/tinybird_cdk/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:33:50.861026 tinybird_cdk-0.17.9/tinybird_cdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-04-19 14:33:50.000000 tinybird_cdk-0.17.9/tinybird_cdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      993 2024-04-19 14:33:50.000000 tinybird_cdk-0.17.9/tinybird_cdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 14:33:50.000000 tinybird_cdk-0.17.9/tinybird_cdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      343 2024-04-19 14:33:50.000000 tinybird_cdk-0.17.9/tinybird_cdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-19 14:33:50.000000 tinybird_cdk-0.17.9/tinybird_cdk.egg-info/top_level.txt
```

### Comparing `tinybird_cdk-0.17.7/PKG-INFO` & `tinybird_cdk-0.17.9/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: tinybird-cdk
-Version: 0.17.7
+Version: 0.17.9
 Summary: Tinybird's Connector Development Kit.
 Author-email: "tinybird.co" <support@tinybird.co>
 Project-URL: Repository, https://github.com/tinybirdco/cdk.git
-Requires-Python: <3.12,>=3.8
+Requires-Python: <3.12,>=3.11
 Description-Content-Type: text/markdown
 Requires-Dist: boto3==1.26.38
 Requires-Dist: google-cloud-bigquery==3.4.1
 Requires-Dist: google-cloud-storage==2.7.0
 Requires-Dist: humanize==4.2.3
 Requires-Dist: httpx[http2]==0.23.1
 Requires-Dist: kinesis-python==0.2.1
 Requires-Dist: mysql-connector-python==8.0.29
 Requires-Dist: ndjson==0.3.1
-Requires-Dist: psycopg2-binary==2.9.3
+Requires-Dist: psycopg2-binary==2.9.9
 Requires-Dist: python-dateutil==2.8.2
 Requires-Dist: sentry-sdk
 Requires-Dist: snowflake-connector-python==3.8.1
 Provides-Extra: dev
 Requires-Dist: bump2version==1.0.1; extra == "dev"
 Requires-Dist: faker==15.3.4; extra == "dev"
 Requires-Dist: pytest==7.2.0; extra == "dev"
```

### Comparing `tinybird_cdk-0.17.7/README.md` & `tinybird_cdk-0.17.9/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -63,27 +63,27 @@
 ## CDK Development
 
 <a id="markdown-tldr" name="tldr"></a>
 ### TL;DR
 
 Everything is detailed later, but this is the gist of it:
 
-1. Install Python >= 3.8
+1. Install Python >= 3.11
 1. Install Docker Compose
 1. Setup and activate a virtual environment
 1. Set the environment variable `TB_CDK_TEST_SUITE_TOKEN` (ask for its value)
 1. Run `pip install -e .["dev"]`
 1. Run `bin/test`
 
 You should see the test suite passing.
 
 <a id="markdown-python" name="python"></a>
 ### Python
 
-The CDK is tested with Python 3.8 to match Analytics.
+The CDK is tested with Python 3.11 to match Analytics.
 
 However, the CDK uses pretty standard Python, nothing fancy. Upgrading when
 Analytics does should be routine.
 
 <a id="markdown-virtual-environment" name="virtual-environment"></a>
 ### Virtual Environment
```

### Comparing `tinybird_cdk-0.17.7/pyproject.toml` & `tinybird_cdk-0.17.9/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [project]
 dynamic = ["dependencies", "optional-dependencies"]
 name = "tinybird-cdk"
-version = "0.17.7"
+version = "0.17.9"
 description = "Tinybird's Connector Development Kit.\nThis package is under active development and currently meant for internal use only."
 readme = "DESCRIPTION.md"
 authors=[{name = "tinybird.co", email= "support@tinybird.co"}]
-requires-python = ">=3.8, <3.12"
+requires-python = ">=3.11, <3.12"
 
 [tool.setuptools.package-dir]
 tinybird_cdk = "tinybird_cdk/"
 
 [tool.setuptools.dynamic]
 dependencies = {file = ["requirements.txt"]}
 optional-dependencies = { dev = {file = ["requirements-dev.txt"]} }
```

### Comparing `tinybird_cdk-0.17.7/tests/test_gcp.py` & `tinybird_cdk-0.17.9/tests/test_gcp.py`

 * *Files identical despite different names*

### Comparing `tinybird_cdk-0.17.7/tinybird_cdk/cloud/__init__.py` & `tinybird_cdk-0.17.9/tinybird_cdk/cloud/__init__.py`

 * *Files identical despite different names*

### Comparing `tinybird_cdk-0.17.7/tinybird_cdk/cloud/abstract_client.py` & `tinybird_cdk-0.17.9/tinybird_cdk/cloud/abstract_client.py`

 * *Files identical despite different names*

### Comparing `tinybird_cdk-0.17.7/tinybird_cdk/cloud/gcp.py` & `tinybird_cdk-0.17.9/tinybird_cdk/cloud/gcp.py`

 * *Files identical despite different names*

### Comparing `tinybird_cdk-0.17.7/tinybird_cdk/cloud/gcs.py` & `tinybird_cdk-0.17.9/tinybird_cdk/cloud/gcs.py`

 * *Files identical despite different names*

### Comparing `tinybird_cdk-0.17.7/tinybird_cdk/cloud/s3.py` & `tinybird_cdk-0.17.9/tinybird_cdk/cloud/s3.py`

 * *Files identical despite different names*

### Comparing `tinybird_cdk-0.17.7/tinybird_cdk/config.py` & `tinybird_cdk-0.17.9/tinybird_cdk/config.py`

 * *Files identical despite different names*

### Comparing `tinybird_cdk-0.17.7/tinybird_cdk/connector.py` & `tinybird_cdk-0.17.9/tinybird_cdk/connector.py`

 * *Files identical despite different names*

### Comparing `tinybird_cdk-0.17.7/tinybird_cdk/connectors/bigquery.py` & `tinybird_cdk-0.17.9/tinybird_cdk/connectors/bigquery.py`

 * *Files identical despite different names*

### Comparing `tinybird_cdk-0.17.7/tinybird_cdk/connectors/kinesis.py` & `tinybird_cdk-0.17.9/tinybird_cdk/connectors/kinesis.py`

 * *Files identical despite different names*

### Comparing `tinybird_cdk-0.17.7/tinybird_cdk/connectors/mysql.py` & `tinybird_cdk-0.17.9/tinybird_cdk/connectors/mysql.py`

 * *Files identical despite different names*

### Comparing `tinybird_cdk-0.17.7/tinybird_cdk/connectors/postgresql.py` & `tinybird_cdk-0.17.9/tinybird_cdk/connectors/postgresql.py`

 * *Files identical despite different names*

### Comparing `tinybird_cdk-0.17.7/tinybird_cdk/connectors/snowflake.py` & `tinybird_cdk-0.17.9/tinybird_cdk/connectors/snowflake.py`

 * *Files identical despite different names*

### Comparing `tinybird_cdk-0.17.7/tinybird_cdk/connectors/sqlite.py` & `tinybird_cdk-0.17.9/tinybird_cdk/connectors/sqlite.py`

 * *Files identical despite different names*

### Comparing `tinybird_cdk-0.17.7/tinybird_cdk/errors.py` & `tinybird_cdk-0.17.9/tinybird_cdk/errors.py`

 * *Files identical despite different names*

### Comparing `tinybird_cdk-0.17.7/tinybird_cdk/export.py` & `tinybird_cdk-0.17.9/tinybird_cdk/export.py`

 * *Files identical despite different names*

### Comparing `tinybird_cdk-0.17.7/tinybird_cdk/formats.py` & `tinybird_cdk-0.17.9/tinybird_cdk/formats.py`

 * *Files identical despite different names*

### Comparing `tinybird_cdk-0.17.7/tinybird_cdk/logger.py` & `tinybird_cdk-0.17.9/tinybird_cdk/logger.py`

 * *Files identical despite different names*

### Comparing `tinybird_cdk-0.17.7/tinybird_cdk/migration.py` & `tinybird_cdk-0.17.9/tinybird_cdk/migration.py`

 * *Files identical despite different names*

### Comparing `tinybird_cdk-0.17.7/tinybird_cdk/schema.py` & `tinybird_cdk-0.17.9/tinybird_cdk/schema.py`

 * *Files identical despite different names*

### Comparing `tinybird_cdk-0.17.7/tinybird_cdk/tinybird.py` & `tinybird_cdk-0.17.9/tinybird_cdk/tinybird.py`

 * *Files identical despite different names*

### Comparing `tinybird_cdk-0.17.7/tinybird_cdk.egg-info/PKG-INFO` & `tinybird_cdk-0.17.9/tinybird_cdk.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: tinybird-cdk
-Version: 0.17.7
+Version: 0.17.9
 Summary: Tinybird's Connector Development Kit.
 Author-email: "tinybird.co" <support@tinybird.co>
 Project-URL: Repository, https://github.com/tinybirdco/cdk.git
-Requires-Python: <3.12,>=3.8
+Requires-Python: <3.12,>=3.11
 Description-Content-Type: text/markdown
 Requires-Dist: boto3==1.26.38
 Requires-Dist: google-cloud-bigquery==3.4.1
 Requires-Dist: google-cloud-storage==2.7.0
 Requires-Dist: humanize==4.2.3
 Requires-Dist: httpx[http2]==0.23.1
 Requires-Dist: kinesis-python==0.2.1
 Requires-Dist: mysql-connector-python==8.0.29
 Requires-Dist: ndjson==0.3.1
-Requires-Dist: psycopg2-binary==2.9.3
+Requires-Dist: psycopg2-binary==2.9.9
 Requires-Dist: python-dateutil==2.8.2
 Requires-Dist: sentry-sdk
 Requires-Dist: snowflake-connector-python==3.8.1
 Provides-Extra: dev
 Requires-Dist: bump2version==1.0.1; extra == "dev"
 Requires-Dist: faker==15.3.4; extra == "dev"
 Requires-Dist: pytest==7.2.0; extra == "dev"
```

### Comparing `tinybird_cdk-0.17.7/tinybird_cdk.egg-info/SOURCES.txt` & `tinybird_cdk-0.17.9/tinybird_cdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

