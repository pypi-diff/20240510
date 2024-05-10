# Comparing `tmp/dataforge_core-1.0.0.tar.gz` & `tmp/dataforge_core-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dataforge_core-1.0.0.tar", last modified: Tue Apr 30 19:36:51 2024, max compression
+gzip compressed data, was "dataforge_core-1.0.1.tar", last modified: Fri May 10 16:36:07 2024, max compression
```

## Comparing `dataforge_core-1.0.0.tar` & `dataforge_core-1.0.1.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 19:36:51.558631 dataforge_core-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11393 2024-04-30 19:36:46.000000 dataforge_core-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 19:36:46.000000 dataforge_core-1.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5631 2024-04-30 19:36:51.558631 dataforge_core-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5025 2024-04-30 19:36:46.000000 dataforge_core-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 19:36:51.550631 dataforge_core-1.0.0/cli/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 19:36:51.554631 dataforge_core-1.0.0/cli/dataforge/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 19:36:46.000000 dataforge_core-1.0.0/cli/dataforge/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2918 2024-04-30 19:36:46.000000 dataforge_core-1.0.0/cli/dataforge/databricks_sql.py
--rw-r--r--   0 runner    (1001) docker     (127)     6413 2024-04-30 19:36:46.000000 dataforge_core-1.0.0/cli/dataforge/importProject.py
--rw-r--r--   0 runner    (1001) docker     (127)      371 2024-04-30 19:36:46.000000 dataforge_core-1.0.0/cli/dataforge/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     7432 2024-04-30 19:36:46.000000 dataforge_core-1.0.0/cli/dataforge/mainConfig.py
--rw-r--r--   0 runner    (1001) docker     (127)     4046 2024-04-30 19:36:46.000000 dataforge_core-1.0.0/cli/dataforge/miniSparky.py
--rw-r--r--   0 runner    (1001) docker     (127)     1831 2024-04-30 19:36:46.000000 dataforge_core-1.0.0/cli/dataforge/pg.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 19:36:51.554631 dataforge_core-1.0.0/cli/dataforge/resources/
--rw-r--r--   0 runner    (1001) docker     (127)     2630 2024-04-30 19:36:46.000000 dataforge_core-1.0.0/cli/dataforge/resources/log4j2.properties
--rw-r--r--   0 runner    (1001) docker     (127)   253868 2024-04-30 19:36:46.000000 dataforge_core-1.0.0/cli/dataforge/resources/pg_deploy.sql
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 19:36:51.554631 dataforge_core-1.0.0/cli/dataforge/resources/project/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-30 19:36:46.000000 dataforge_core-1.0.0/cli/dataforge/resources/project/meta.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 19:36:51.554631 dataforge_core-1.0.0/cli/dataforge/resources/project/outputs/
--rw-r--r--   0 runner    (1001) docker     (127)      690 2024-04-30 19:36:46.000000 dataforge_core-1.0.0/cli/dataforge/resources/project/outputs/feature_customer.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-04-30 19:36:46.000000 dataforge_core-1.0.0/cli/dataforge/resources/project/relations.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 19:36:51.558631 dataforge_core-1.0.0/cli/dataforge/resources/project/sources/
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-04-30 19:36:46.000000 dataforge_core-1.0.0/cli/dataforge/resources/project/sources/tpch_customer.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1499 2024-04-30 19:36:46.000000 dataforge_core-1.0.0/cli/dataforge/resources/project/sources/tpch_lineitem.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-30 19:36:46.000000 dataforge_core-1.0.0/cli/dataforge/resources/project/sources/tpch_nations.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      296 2024-04-30 19:36:46.000000 dataforge_core-1.0.0/cli/dataforge/resources/project/sources/tpch_orders.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-30 19:36:46.000000 dataforge_core-1.0.0/cli/dataforge/resources/project/sources/tpch_part.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      307 2024-04-30 19:36:46.000000 dataforge_core-1.0.0/cli/dataforge/resources/project/sources/tpch_partsupp.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-04-30 19:36:46.000000 dataforge_core-1.0.0/cli/dataforge/resources/project/sources/tpch_region.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-04-30 19:36:46.000000 dataforge_core-1.0.0/cli/dataforge/resources/project/sources/tpch_supplier.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1769 2024-04-30 19:36:46.000000 dataforge_core-1.0.0/cli/dataforge/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 19:36:51.558631 dataforge_core-1.0.0/cli/dataforge_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5631 2024-04-30 19:36:51.000000 dataforge_core-1.0.0/cli/dataforge_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-04-30 19:36:51.000000 dataforge_core-1.0.0/cli/dataforge_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 19:36:51.000000 dataforge_core-1.0.0/cli/dataforge_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-30 19:36:51.000000 dataforge_core-1.0.0/cli/dataforge_core.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-30 19:36:51.000000 dataforge_core-1.0.0/cli/dataforge_core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-30 19:36:51.000000 dataforge_core-1.0.0/cli/dataforge_core.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      880 2024-04-30 19:36:46.000000 dataforge_core-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 19:36:51.558631 dataforge_core-1.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 16:36:07.656473 dataforge_core-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    11393 2024-05-10 16:35:59.000000 dataforge_core-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 16:35:59.000000 dataforge_core-1.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5767 2024-05-10 16:36:07.656473 dataforge_core-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5161 2024-05-10 16:35:59.000000 dataforge_core-1.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 16:36:07.648473 dataforge_core-1.0.1/cli/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 16:36:07.648473 dataforge_core-1.0.1/cli/dataforge/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 16:35:59.000000 dataforge_core-1.0.1/cli/dataforge/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2918 2024-05-10 16:35:59.000000 dataforge_core-1.0.1/cli/dataforge/databricks_sql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6413 2024-05-10 16:35:59.000000 dataforge_core-1.0.1/cli/dataforge/importProject.py
+-rw-r--r--   0 runner    (1001) docker     (127)      371 2024-05-10 16:35:59.000000 dataforge_core-1.0.1/cli/dataforge/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7432 2024-05-10 16:35:59.000000 dataforge_core-1.0.1/cli/dataforge/mainConfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4046 2024-05-10 16:35:59.000000 dataforge_core-1.0.1/cli/dataforge/miniSparky.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1831 2024-05-10 16:35:59.000000 dataforge_core-1.0.1/cli/dataforge/pg.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 16:36:07.652473 dataforge_core-1.0.1/cli/dataforge/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)     2630 2024-05-10 16:35:59.000000 dataforge_core-1.0.1/cli/dataforge/resources/log4j2.properties
+-rw-r--r--   0 runner    (1001) docker     (127)   254078 2024-05-10 16:35:59.000000 dataforge_core-1.0.1/cli/dataforge/resources/pg_deploy.sql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 16:36:07.652473 dataforge_core-1.0.1/cli/dataforge/resources/project/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-10 16:35:59.000000 dataforge_core-1.0.1/cli/dataforge/resources/project/meta.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 16:36:07.652473 dataforge_core-1.0.1/cli/dataforge/resources/project/outputs/
+-rw-r--r--   0 runner    (1001) docker     (127)      690 2024-05-10 16:35:59.000000 dataforge_core-1.0.1/cli/dataforge/resources/project/outputs/feature_customer.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-05-10 16:35:59.000000 dataforge_core-1.0.1/cli/dataforge/resources/project/relations.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 16:36:07.652473 dataforge_core-1.0.1/cli/dataforge/resources/project/sources/
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-05-10 16:35:59.000000 dataforge_core-1.0.1/cli/dataforge/resources/project/sources/tpch_customer.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1499 2024-05-10 16:35:59.000000 dataforge_core-1.0.1/cli/dataforge/resources/project/sources/tpch_lineitem.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-10 16:35:59.000000 dataforge_core-1.0.1/cli/dataforge/resources/project/sources/tpch_nations.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2024-05-10 16:35:59.000000 dataforge_core-1.0.1/cli/dataforge/resources/project/sources/tpch_orders.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-10 16:35:59.000000 dataforge_core-1.0.1/cli/dataforge/resources/project/sources/tpch_part.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-05-10 16:35:59.000000 dataforge_core-1.0.1/cli/dataforge/resources/project/sources/tpch_partsupp.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-05-10 16:35:59.000000 dataforge_core-1.0.1/cli/dataforge/resources/project/sources/tpch_region.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-10 16:35:59.000000 dataforge_core-1.0.1/cli/dataforge/resources/project/sources/tpch_supplier.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1769 2024-05-10 16:35:59.000000 dataforge_core-1.0.1/cli/dataforge/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 16:36:07.656473 dataforge_core-1.0.1/cli/dataforge_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5767 2024-05-10 16:36:07.000000 dataforge_core-1.0.1/cli/dataforge_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-05-10 16:36:07.000000 dataforge_core-1.0.1/cli/dataforge_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 16:36:07.000000 dataforge_core-1.0.1/cli/dataforge_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-10 16:36:07.000000 dataforge_core-1.0.1/cli/dataforge_core.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-10 16:36:07.000000 dataforge_core-1.0.1/cli/dataforge_core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-10 16:36:07.000000 dataforge_core-1.0.1/cli/dataforge_core.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      880 2024-05-10 16:35:59.000000 dataforge_core-1.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 16:36:07.656473 dataforge_core-1.0.1/setup.cfg
```

### Comparing `dataforge_core-1.0.0/LICENSE` & `dataforge_core-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dataforge_core-1.0.0/PKG-INFO` & `dataforge_core-1.0.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dataforge-core
-Version: 1.0.0
+Version: 1.0.1
 Summary: Command line compiler for dataforge core projects
 Author-email: Vadim Orlov <vorlov@dataforgelabs.com>
 Project-URL: Homepage, https://github.com/dataforgelabs/dataforge-core
 Project-URL: Issues, https://github.com/dataforgelabs/dataforge-core/issues
 Requires-Python: >=3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -15,42 +15,44 @@
 Requires-Dist: databricks-sql-connector
 Requires-Dist: sql-formatter
 Requires-Dist: psutil
 
 ![DataForge Core-Light](etc/DataForge_Core_Flow.svg#gh-light-mode-only)
 ![DataForge Core-Dark](etc/DataForge_Core_Flow_Reverse.svg#gh-dark-mode-only)
 
-[DataForge](https://www.dataforgelabs.com) helps data analysts and engineers build and extend data solutions by leveraging modern software engineering principals.
+[DataForge](https://www.dataforgelabs.com) helps data analysts and engineers build and extend data solutions by leveraging modern software engineering principles.
 
 ## Understanding DataForge
 
 DataForge enables writing of inline functions using single-column SQL expressions rather than CTEs, procedural scripts, or set-based models.
 
 
 Each function:
 - is [pure](https://en.wikipedia.org/wiki/Pure_function), with no [side effects](https://en.wikipedia.org/wiki/Side_effect_(computer_science))
 - returns single column
 - is composable with other functions
 
-DataForge software engineering principals:
+DataForge software engineering principles:
 - [Functional Programming](https://en.wikipedia.org/wiki/Functional_programming)
 - [Inversion of Control](https://en.wikipedia.org/wiki/Inversion_of_control)
 - [Single Responsibility Principal](https://en.wikipedia.org/wiki/Single-responsibility_principle)
 - [DRY](https://en.wikipedia.org/wiki/Don%27t_repeat_yourself)
 
-These principals allow DataForge projects to be easy to modify and extend - even with thousands of integrated pipelines.`
+These principles allow DataForge projects to be easy to modify and extend - even with thousands of integrated pipelines.
+
+Explore the Core CLI or [learn more](https://www.dataforgelabs.com/core-vs-cloud) about how Core powers DataForge Cloud.
 
 ## Requirements
 Dataforge Core is a code framework and command line tool to develop transformation functions and compile them into executable Spark SQL.
 
 To run the CLI you will need:
 - Java 8 or higher
   - [Amazon Corretto](https://docs.aws.amazon.com/corretto/) is a great option
-- A PostgreSQL server with a dedicated empty database
-  - Check out our friends over at https://tembo.io/
+- A PostgreSQL v14+ server with a dedicated empty database
+  - Check out our friends over at [Tembo](https://tembo.io/)
 - Python version 3.12+
   - [Official Link](https://www.python.org/downloads/)
 
 The CLI also includes an integration to run the code in Databricks. To support this you need:
 - [Databricks Workspace](https://docs.databricks.com/en/administration-guide/workspace/index.html)
 - [Databricks SQL Warehouse](https://docs.databricks.com/en/compute/sql-warehouse/index.html)
 - [Developer Personal Access Token](https://docs.databricks.com/en/dev-tools/auth/pat.html)
@@ -76,20 +78,15 @@
   Collecting dataforge-core...
   Installing collected packages: dataforge-core
   Successfully installed dataforge-core...
   ```
 - Validate installation:
   ```
   > dataforge --version
-  dataforge-core 0.1.27
-  ```
-- Navigate to an empty folder and initialize project structure and sample files:
-  ```
-  > dataforge --init
-  Initialized project in C:\Users...
+  dataforge-core 1.0.0
   ```
 - Configure connections and credentials to Postgres and optionally Databricks
   ```
   > dataforge --configure
   Enter postgres connection string: postgresql://postgres:<postgres-server-url>:5432/postgres
   Do you want to configure Databricks SQL Warehouse connection (y/n)? y
   Enter Server hostname: <workspace-url>.cloud.databricks.com
@@ -97,14 +94,21 @@
   Enter access token: <token-guid>
   Enter catalog name: <unity_catalog_name>
   Enter schema name: <schema_in_catalog_name>
   Connecting to Databricks SQL Warehouse <workspace-url>.cloud.databricks.com
   Databricks connection validated successfully
   Profile saved in C:\Users...
   ```
+
+- Navigate to an empty folder and initialize project structure and sample files:
+  ```
+  > dataforge --init
+  Initialized project in C:\Users...
+  ```
+
 - Deploy dataforge structures to Postgres
   ```
   > dataforge --seed
   All objects in schema(s) log,meta in postgres database will be deleted. Do you want to continue (y/n)? y
   Initializing database..
   Database initialized
   ```
```

### Comparing `dataforge_core-1.0.0/README.md` & `dataforge_core-1.0.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,38 +1,40 @@
 ![DataForge Core-Light](etc/DataForge_Core_Flow.svg#gh-light-mode-only)
 ![DataForge Core-Dark](etc/DataForge_Core_Flow_Reverse.svg#gh-dark-mode-only)
 
-[DataForge](https://www.dataforgelabs.com) helps data analysts and engineers build and extend data solutions by leveraging modern software engineering principals.
+[DataForge](https://www.dataforgelabs.com) helps data analysts and engineers build and extend data solutions by leveraging modern software engineering principles.
 
 ## Understanding DataForge
 
 DataForge enables writing of inline functions using single-column SQL expressions rather than CTEs, procedural scripts, or set-based models.
 
 
 Each function:
 - is [pure](https://en.wikipedia.org/wiki/Pure_function), with no [side effects](https://en.wikipedia.org/wiki/Side_effect_(computer_science))
 - returns single column
 - is composable with other functions
 
-DataForge software engineering principals:
+DataForge software engineering principles:
 - [Functional Programming](https://en.wikipedia.org/wiki/Functional_programming)
 - [Inversion of Control](https://en.wikipedia.org/wiki/Inversion_of_control)
 - [Single Responsibility Principal](https://en.wikipedia.org/wiki/Single-responsibility_principle)
 - [DRY](https://en.wikipedia.org/wiki/Don%27t_repeat_yourself)
 
-These principals allow DataForge projects to be easy to modify and extend - even with thousands of integrated pipelines.`
+These principles allow DataForge projects to be easy to modify and extend - even with thousands of integrated pipelines.
+
+Explore the Core CLI or [learn more](https://www.dataforgelabs.com/core-vs-cloud) about how Core powers DataForge Cloud.
 
 ## Requirements
 Dataforge Core is a code framework and command line tool to develop transformation functions and compile them into executable Spark SQL.
 
 To run the CLI you will need:
 - Java 8 or higher
   - [Amazon Corretto](https://docs.aws.amazon.com/corretto/) is a great option
-- A PostgreSQL server with a dedicated empty database
-  - Check out our friends over at https://tembo.io/
+- A PostgreSQL v14+ server with a dedicated empty database
+  - Check out our friends over at [Tembo](https://tembo.io/)
 - Python version 3.12+
   - [Official Link](https://www.python.org/downloads/)
 
 The CLI also includes an integration to run the code in Databricks. To support this you need:
 - [Databricks Workspace](https://docs.databricks.com/en/administration-guide/workspace/index.html)
 - [Databricks SQL Warehouse](https://docs.databricks.com/en/compute/sql-warehouse/index.html)
 - [Developer Personal Access Token](https://docs.databricks.com/en/dev-tools/auth/pat.html)
@@ -58,20 +60,15 @@
   Collecting dataforge-core...
   Installing collected packages: dataforge-core
   Successfully installed dataforge-core...
   ```
 - Validate installation:
   ```
   > dataforge --version
-  dataforge-core 0.1.27
-  ```
-- Navigate to an empty folder and initialize project structure and sample files:
-  ```
-  > dataforge --init
-  Initialized project in C:\Users...
+  dataforge-core 1.0.0
   ```
 - Configure connections and credentials to Postgres and optionally Databricks
   ```
   > dataforge --configure
   Enter postgres connection string: postgresql://postgres:<postgres-server-url>:5432/postgres
   Do you want to configure Databricks SQL Warehouse connection (y/n)? y
   Enter Server hostname: <workspace-url>.cloud.databricks.com
@@ -79,14 +76,21 @@
   Enter access token: <token-guid>
   Enter catalog name: <unity_catalog_name>
   Enter schema name: <schema_in_catalog_name>
   Connecting to Databricks SQL Warehouse <workspace-url>.cloud.databricks.com
   Databricks connection validated successfully
   Profile saved in C:\Users...
   ```
+
+- Navigate to an empty folder and initialize project structure and sample files:
+  ```
+  > dataforge --init
+  Initialized project in C:\Users...
+  ```
+
 - Deploy dataforge structures to Postgres
   ```
   > dataforge --seed
   All objects in schema(s) log,meta in postgres database will be deleted. Do you want to continue (y/n)? y
   Initializing database..
   Database initialized
   ```
```

### Comparing `dataforge_core-1.0.0/cli/dataforge/databricks_sql.py` & `dataforge_core-1.0.1/cli/dataforge/databricks_sql.py`

 * *Files identical despite different names*

### Comparing `dataforge_core-1.0.0/cli/dataforge/importProject.py` & `dataforge_core-1.0.1/cli/dataforge/importProject.py`

 * *Files identical despite different names*

### Comparing `dataforge_core-1.0.0/cli/dataforge/mainConfig.py` & `dataforge_core-1.0.1/cli/dataforge/mainConfig.py`

 * *Files identical despite different names*

### Comparing `dataforge_core-1.0.0/cli/dataforge/miniSparky.py` & `dataforge_core-1.0.1/cli/dataforge/miniSparky.py`

 * *Files identical despite different names*

### Comparing `dataforge_core-1.0.0/cli/dataforge/pg.py` & `dataforge_core-1.0.1/cli/dataforge/pg.py`

 * *Files identical despite different names*

### Comparing `dataforge_core-1.0.0/cli/dataforge/resources/log4j2.properties` & `dataforge_core-1.0.1/cli/dataforge/resources/log4j2.properties`

 * *Files identical despite different names*

### Comparing `dataforge_core-1.0.0/cli/dataforge/resources/pg_deploy.sql` & `dataforge_core-1.0.1/cli/dataforge/resources/pg_deploy.sql`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
---Built: Tue Apr 30 19:36:46 UTC 2024
+--Built: Fri May 10 16:35:59 UTC 2024
 CREATE SCHEMA IF NOT EXISTS meta;
 CREATE SCHEMA IF NOT EXISTS log;
 DO $$
 BEGIN
     IF EXISTS (SELECT 1 FROM pg_type WHERE typname = 'parameter_map') THEN
         DROP TYPE parameter_map CASCADE; 
     END IF;
@@ -216,15 +216,15 @@
     ('avg', 'Returns the mean calculated from values of a group.', TRUE, 'double'),
     ('bit_or', 'Returns the bitwise OR of all non-null input values, or null if none.', FALSE, 'boolean'),
     ('bit_xor', 'Returns the bitwise XOR of all non-null input values, or null if none.', FALSE, 'boolean'),
     ('bool_and', 'Returns true if all values of `expr` are true.', FALSE, 'boolean'),
     ('bool_or', 'Returns true if at least one value of `expr` is true.', FALSE, 'boolean'),
     ('collect_list', 'Collects and returns a list of non-unique elements', FALSE, 'array'),
     ('collect_set', 'Collects and returns a set of unique elements', FALSE, 'array'),
-    ('corr', 'Returns Pearson coefficient of correlation between a set of number pairs.', TRUE, 'numeric'),
+    ('corr', 'Returns Pearson coefficient of correlation between a set of number pairs.', TRUE, 'decimal'),
     ('count', 'Returns the number of rows for which the column expression is non-null.', FALSE, 'long'),
     ('count_if', 'Returns the number of `TRUE` values for the expression.', FALSE, 'long'),
 ('count_min_sketch', 'Returns a count-min sketch of a column with the given esp, confidence and seed. The result is an array of bytes, which can be deserialized to a `CountMinSketch` before usage. Count-min sketch is a probabilistic data structure used for cardinality estimation using sub-linear space.', FALSE, 'string'),
     ('covar_pop', 'Returns the population covariance of a set of number pairs.', TRUE, 'decimal'),
     ('covar_samp', 'Returns the sample covariance of a set of number pairs.', TRUE, 'decimal'),
     ('every', 'Returns true if all values of `expr` are true.', FALSE, 'boolean'),
     ('first', 'Returns the first value of column for a group of rows', FALSE, 'default'),
@@ -726,16 +726,15 @@
     WITH parsed AS (
         SELECT import_object_id, body_text::jsonb body
         FROM meta.import_object WHERE import_id = in_import_id)
     UPDATE meta.import_object io
     SET body = p.body, 
         name =  CASE WHEN object_type IN ('source' ,'output', 'group', 'token') THEN p.body->>(object_type || '_name')
                 WHEN object_type IN ('output_template','source_template') THEN p.body->>'object_name'
-        ELSE p.body->>'name' END,
-        hash = md5(io.body_text)
+        ELSE p.body->>'name' END
     FROM parsed p WHERE p.import_object_id = io.import_object_id;
 
     INSERT INTO log.actor_log (log_id, message, actor_path, severity, insert_datetime)
     VALUES ( v_log_id, 'Import files parsing completed','imp_parse_objects', 'I', clock_timestamp());
 END;
 $function$;CREATE OR REPLACE FUNCTION meta.impc_execute(in_imp meta.import)
     RETURNS jsonb
@@ -1040,32 +1039,35 @@
     v_datatype_schema jsonb;
 BEGIN
 
     IF jsonb_typeof(in_raw) = 'string' THEN -- parse string
         v_parsed := regexp_split_to_array(in_raw->>0, '\s+(AS\s+|)','i');
         v_attribute_name := v_parsed[1];
         v_data_type := lower(v_parsed[2]);
+        IF v_data_type IS NULL THEN
+            RETURN jsonb_build_object('error', format('Unable to parse raw attribute data type from %s', in_raw));
+        END IF;
         v_datatype_schema := meta.u_get_schema_from_type(null, v_data_type);
 
     ELSEIF jsonb_typeof(in_raw) = 'object' THEN -- parse object
         v_attribute_name := in_raw->>'name';
         v_datatype_schema := in_raw->'schema';
         v_data_type := meta.u_get_typename_from_schema(v_datatype_schema);
     ELSE
         RETURN jsonb_build_object('error', format('Invalid raw attribute spec %s', in_raw));
     END IF;
 
 -- validate name and type
 
     IF v_attribute_name IS NULL THEN
-        RETURN jsonb_build_object('error', format('Invalid raw attribute %s', in_raw));
+        RETURN jsonb_build_object('error', format('Unable to parse raw attribute name from %s', in_raw));
     END IF;
 
     IF v_data_type NOT IN (SELECT hive_type from meta.attribute_type) THEN
-        RETURN jsonb_build_object('error', format('Invalid raw attribute datatype %s', in_raw));
+        RETURN jsonb_build_object('error', format('Invalid raw attribute datatype `%s`', v_data_type));
     END IF;
 
     RETURN jsonb_build_object('name', lower(v_attribute_name), 'data_type', v_data_type, 'datatype_schema', v_datatype_schema);
 
 END;
 
 $BODY$;
@@ -4103,18 +4105,20 @@
 
 DECLARE
     v_attribute_name text;
 
 BEGIN
 
     IF osc IS NULL THEN
-        RETURN CASE in_hive_type
-            WHEN 'struct' THEN 'struct()'
-            WHEN 'array' THEN 'array()'
-            ELSE 'CAST(null as ' || COALESCE(osc.datatype,'string') || ')'
+        RETURN 
+            CASE 
+            WHEN in_hive_type = 'struct' THEN 'struct()'
+            WHEN in_hive_type = 'array' THEN 'array()'
+            WHEN in_hive_type IS NOT NULL THEN 'CAST(null as ' || in_hive_type || ')'
+            ELSE 'null'
             END;
     END IF;
 
     SELECT attribute_name INTO v_attribute_name
     FROM meta.u_get_output_parameter_name_id(osc);
 
     PERFORM meta.u_assert(v_attribute_name IS NOT NULL,format('Unable to lookup attribute name for output mapping %s',osc));
@@ -4914,15 +4918,15 @@
 -- We now have now added all parents of enrichment
 -- Inserting the enrichment record
 
     WITH cte AS (
     INSERT INTO elements ( type, expression, alias, attribute_id, parent_ids, data_type)
     VALUES ( 'enrichment', v_expression, in_enr.attribute_name, in_enr.enrichment_id, v_parent_element_ids,
             --Check for explicit casts or numeric/decimal types that need to be cast to 38,12
-    (SELECT CASE WHEN COALESCE(NULLIF(in_enr.cast_datatype,''), in_enr.datatype) IN ('decimal', 'numeric') OR (COALESCE(in_enr.cast_datatype,'') <> '' AND in_enr.cast_datatype <> in_enr.datatype) THEN at.hive_ddl_type END FROM meta.attribute_type at WHERE at.hive_type = COALESCE(NULLIF(in_enr.cast_datatype,''), in_enr.datatype) ))
+    (SELECT CASE WHEN COALESCE(NULLIF(in_enr.cast_datatype,''), in_enr.datatype) = 'decimal' OR (COALESCE(in_enr.cast_datatype,'') <> '' AND in_enr.cast_datatype <> in_enr.datatype) THEN at.hive_ddl_type END FROM meta.attribute_type at WHERE at.hive_type = COALESCE(NULLIF(in_enr.cast_datatype,''), in_enr.datatype) ))
     RETURNING id )
     SELECT id INTO v_ret_element_id
     FROM cte;
 
 RETURN v_ret_element_id;        
 END;
```

### Comparing `dataforge_core-1.0.0/cli/dataforge/resources/project/outputs/feature_customer.yaml` & `dataforge_core-1.0.1/cli/dataforge/resources/project/outputs/feature_customer.yaml`

 * *Files identical despite different names*

### Comparing `dataforge_core-1.0.0/cli/dataforge/resources/project/relations.yaml` & `dataforge_core-1.0.1/cli/dataforge/resources/project/relations.yaml`

 * *Files identical despite different names*

### Comparing `dataforge_core-1.0.0/cli/dataforge/resources/project/sources/tpch_lineitem.yaml` & `dataforge_core-1.0.1/cli/dataforge/resources/project/sources/tpch_lineitem.yaml`

 * *Ordering differences only*

 * *Files 8% similar despite different names*

```diff
@@ -16,29 +16,29 @@
 - l_returnflag string
 - l_shipdate date
 - l_shipinstruct string
 - l_shipmode string
 - l_suppkey long
 - l_tax decimal
 rules:
+#Calculation using raw attributes only
+- name: "net_price_int"
+  expression: "([This].l_extendedprice - [This].l_tax - [This].l_discount)*100"
 #Basic lookup:
 - name: "c_name"
   expression: "[tpch_customer].c_name"
 #Lookup using explicit relation path
 - name: "c_n_name"
   expression: "[tpch_nation].n_name"
   parameters:
   - source_name: tpch_nation
     relations:
     - "[tpch_lineitem]- orderkey -[tpch_orders]"
     - "[tpch_orders]- custkey -[tpch_customer]"
     - "[tpch_customer]- nationkey -[tpch_nation]"
-#Calculation using raw attributes only
-- name: "net_price_int"
-  expression: "([This].l_extendedprice - [This].l_tax - [This].l_discount)*100"
 #Calculation using function results from two sources and a raw attribute
 - name: "gross_margin_per_quantity"
   expression: "([This].net_price_int - [tpch_partsupp].ps_supplycost)/[This].l_quantity"
 #Function result used as a key in a relation (see relations.yaml)
 - name: "partsupp_pkey"
   expression: "CONCAT([This].l_partkey,'|',[This].l_suppkey)"
 #Use spark SQL functions inline (https://spark.apache.org/docs/latest/api/sql/index.html)
```

### Comparing `dataforge_core-1.0.0/cli/dataforge/util.py` & `dataforge_core-1.0.1/cli/dataforge/util.py`

 * *Files identical despite different names*

### Comparing `dataforge_core-1.0.0/cli/dataforge_core.egg-info/PKG-INFO` & `dataforge_core-1.0.1/cli/dataforge_core.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dataforge-core
-Version: 1.0.0
+Version: 1.0.1
 Summary: Command line compiler for dataforge core projects
 Author-email: Vadim Orlov <vorlov@dataforgelabs.com>
 Project-URL: Homepage, https://github.com/dataforgelabs/dataforge-core
 Project-URL: Issues, https://github.com/dataforgelabs/dataforge-core/issues
 Requires-Python: >=3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -15,42 +15,44 @@
 Requires-Dist: databricks-sql-connector
 Requires-Dist: sql-formatter
 Requires-Dist: psutil
 
 ![DataForge Core-Light](etc/DataForge_Core_Flow.svg#gh-light-mode-only)
 ![DataForge Core-Dark](etc/DataForge_Core_Flow_Reverse.svg#gh-dark-mode-only)
 
-[DataForge](https://www.dataforgelabs.com) helps data analysts and engineers build and extend data solutions by leveraging modern software engineering principals.
+[DataForge](https://www.dataforgelabs.com) helps data analysts and engineers build and extend data solutions by leveraging modern software engineering principles.
 
 ## Understanding DataForge
 
 DataForge enables writing of inline functions using single-column SQL expressions rather than CTEs, procedural scripts, or set-based models.
 
 
 Each function:
 - is [pure](https://en.wikipedia.org/wiki/Pure_function), with no [side effects](https://en.wikipedia.org/wiki/Side_effect_(computer_science))
 - returns single column
 - is composable with other functions
 
-DataForge software engineering principals:
+DataForge software engineering principles:
 - [Functional Programming](https://en.wikipedia.org/wiki/Functional_programming)
 - [Inversion of Control](https://en.wikipedia.org/wiki/Inversion_of_control)
 - [Single Responsibility Principal](https://en.wikipedia.org/wiki/Single-responsibility_principle)
 - [DRY](https://en.wikipedia.org/wiki/Don%27t_repeat_yourself)
 
-These principals allow DataForge projects to be easy to modify and extend - even with thousands of integrated pipelines.`
+These principles allow DataForge projects to be easy to modify and extend - even with thousands of integrated pipelines.
+
+Explore the Core CLI or [learn more](https://www.dataforgelabs.com/core-vs-cloud) about how Core powers DataForge Cloud.
 
 ## Requirements
 Dataforge Core is a code framework and command line tool to develop transformation functions and compile them into executable Spark SQL.
 
 To run the CLI you will need:
 - Java 8 or higher
   - [Amazon Corretto](https://docs.aws.amazon.com/corretto/) is a great option
-- A PostgreSQL server with a dedicated empty database
-  - Check out our friends over at https://tembo.io/
+- A PostgreSQL v14+ server with a dedicated empty database
+  - Check out our friends over at [Tembo](https://tembo.io/)
 - Python version 3.12+
   - [Official Link](https://www.python.org/downloads/)
 
 The CLI also includes an integration to run the code in Databricks. To support this you need:
 - [Databricks Workspace](https://docs.databricks.com/en/administration-guide/workspace/index.html)
 - [Databricks SQL Warehouse](https://docs.databricks.com/en/compute/sql-warehouse/index.html)
 - [Developer Personal Access Token](https://docs.databricks.com/en/dev-tools/auth/pat.html)
@@ -76,20 +78,15 @@
   Collecting dataforge-core...
   Installing collected packages: dataforge-core
   Successfully installed dataforge-core...
   ```
 - Validate installation:
   ```
   > dataforge --version
-  dataforge-core 0.1.27
-  ```
-- Navigate to an empty folder and initialize project structure and sample files:
-  ```
-  > dataforge --init
-  Initialized project in C:\Users...
+  dataforge-core 1.0.0
   ```
 - Configure connections and credentials to Postgres and optionally Databricks
   ```
   > dataforge --configure
   Enter postgres connection string: postgresql://postgres:<postgres-server-url>:5432/postgres
   Do you want to configure Databricks SQL Warehouse connection (y/n)? y
   Enter Server hostname: <workspace-url>.cloud.databricks.com
@@ -97,14 +94,21 @@
   Enter access token: <token-guid>
   Enter catalog name: <unity_catalog_name>
   Enter schema name: <schema_in_catalog_name>
   Connecting to Databricks SQL Warehouse <workspace-url>.cloud.databricks.com
   Databricks connection validated successfully
   Profile saved in C:\Users...
   ```
+
+- Navigate to an empty folder and initialize project structure and sample files:
+  ```
+  > dataforge --init
+  Initialized project in C:\Users...
+  ```
+
 - Deploy dataforge structures to Postgres
   ```
   > dataforge --seed
   All objects in schema(s) log,meta in postgres database will be deleted. Do you want to continue (y/n)? y
   Initializing database..
   Database initialized
   ```
```

### Comparing `dataforge_core-1.0.0/cli/dataforge_core.egg-info/SOURCES.txt` & `dataforge_core-1.0.1/cli/dataforge_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dataforge_core-1.0.0/pyproject.toml` & `dataforge_core-1.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "dataforge-core"
-version = "v1.0.0"
+version = "v1.0.1"
 authors = [
     {name="Vadim Orlov", email="vorlov@dataforgelabs.com"}
 ]
 description = "Command line compiler for dataforge core projects"
 readme = "README.md"
 requires-python = ">=3.12"
 dependencies = [
```

