# Comparing `tmp/palje-2.0.0-py3-none-any.whl.zip` & `tmp/palje-2.1.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 23804 bytes, number of entries: 13
+Zip file size: 24548 bytes, number of entries: 13
 -rw-rw-rw-  2.0 fat      131 b- defN 24-Apr-12 06:36 palje/__init__.py
--rw-rw-rw-  2.0 fat    10408 b- defN 24-May-06 13:39 palje/__main__.py
+-rw-rw-rw-  2.0 fat    10422 b- defN 24-May-10 07:11 palje/__main__.py
 -rw-rw-rw-  2.0 fat     7152 b- defN 24-May-06 13:39 palje/confluence_rest.py
 -rw-rw-rw-  2.0 fat    10947 b- defN 24-Apr-16 13:53 palje/mssql_database.py
 -rw-rw-rw-  2.0 fat     4256 b- defN 24-May-06 13:39 palje/storage_format.py
--rw-rw-rw-  2.0 fat      427 b- defN 24-May-07 07:15 palje/version.py
+-rw-rw-rw-  2.0 fat      427 b- defN 24-May-10 09:03 palje/version.py
 -rw-rw-rw-  2.0 fat    10126 b- defN 24-Apr-12 06:36 palje/queries/database_queries.ini
--rw-rw-rw-  2.0 fat    11556 b- defN 24-May-07 07:15 palje-2.0.0.dist-info/LICENSE
--rw-rw-rw-  2.0 fat    21369 b- defN 24-May-07 07:15 palje-2.0.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-May-07 07:15 palje-2.0.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       46 b- defN 24-May-07 07:15 palje-2.0.0.dist-info/entry_points.txt
--rw-rw-rw-  2.0 fat        6 b- defN 24-May-07 07:15 palje-2.0.0.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1024 b- defN 24-May-07 07:15 palje-2.0.0.dist-info/RECORD
-13 files, 77540 bytes uncompressed, 22112 bytes compressed:  71.5%
+-rw-rw-rw-  2.0 fat    11556 b- defN 24-May-10 09:03 palje-2.1.0.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat    23307 b- defN 24-May-10 09:03 palje-2.1.0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-May-10 09:03 palje-2.1.0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       46 b- defN 24-May-10 09:03 palje-2.1.0.dist-info/entry_points.txt
+-rw-rw-rw-  2.0 fat        6 b- defN 24-May-10 09:03 palje-2.1.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1024 b- defN 24-May-10 09:03 palje-2.1.0.dist-info/RECORD
+13 files, 79492 bytes uncompressed, 22856 bytes compressed:  71.2%
```

## zipnote {}

```diff
@@ -15,26 +15,26 @@
 
 Filename: palje/version.py
 Comment: 
 
 Filename: palje/queries/database_queries.ini
 Comment: 
 
-Filename: palje-2.0.0.dist-info/LICENSE
+Filename: palje-2.1.0.dist-info/LICENSE
 Comment: 
 
-Filename: palje-2.0.0.dist-info/METADATA
+Filename: palje-2.1.0.dist-info/METADATA
 Comment: 
 
-Filename: palje-2.0.0.dist-info/WHEEL
+Filename: palje-2.1.0.dist-info/WHEEL
 Comment: 
 
-Filename: palje-2.0.0.dist-info/entry_points.txt
+Filename: palje-2.1.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: palje-2.0.0.dist-info/top_level.txt
+Filename: palje-2.1.0.dist-info/top_level.txt
 Comment: 
 
-Filename: palje-2.0.0.dist-info/RECORD
+Filename: palje-2.1.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## palje/__main__.py

```diff
@@ -2,17 +2,17 @@
 #
 # Copyright 2021 ALM Partners Oy
 # SPDX-License-Identifier: Apache-2.0
 
 import sys
 from argparse import ArgumentParser
 
-from . import storage_format
-from .confluence_rest import ConfluenceREST
-from .mssql_database import MSSQLDatabase, DATABASE_OBJECT_TYPES
+from palje import storage_format
+from palje.confluence_rest import ConfluenceREST
+from palje.mssql_database import MSSQLDatabase, DATABASE_OBJECT_TYPES
 
 
 def main(argv: list[str] | None = None):
     global WIKI, DB, SPACE, space_id
     # TODO: possibility to read params from config?
     (confluence_url, SPACE, parent_page, server, database,
         schema_filter, database_filter, driver, authentication) = parse_arguments(argv)
```

## palje/version.py

```diff
@@ -8,9 +8,9 @@
     VERSION_TUPLE = object
 
 version: str
 __version__: str
 __version_tuple__: VERSION_TUPLE
 version_tuple: VERSION_TUPLE
 
-__version__ = version = '2.0.0'
-__version_tuple__ = version_tuple = (2, 0, 0)
+__version__ = version = '2.1.0'
+__version_tuple__ = version_tuple = (2, 1, 0)
```

## Comparing `palje-2.0.0.dist-info/LICENSE` & `palje-2.1.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `palje-2.0.0.dist-info/METADATA` & `palje-2.1.0.dist-info/METADATA`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: palje
-Version: 2.0.0
+Version: 2.1.0
 Summary: A tool for creating hierarchical documentation of SQL Server databases to Confluence wiki.
 Author: ALM Partners Oy
 Maintainer: ALM Partners Oy
 License: Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
@@ -215,14 +215,16 @@
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: azure-identity ~=1.14
 Requires-Dist: sqlalchemy[mssql] ~=2.0.29
 Requires-Dist: requests ~=2.31.0
+Provides-Extra: msibuild
+Requires-Dist: cx-freeze ~=7.0.0 ; extra == 'msibuild'
 Provides-Extra: test
 Requires-Dist: tox ~=4.15 ; extra == 'test'
 
 Palje
 ====================
 
 # Description
@@ -384,14 +386,52 @@
 
 # without MSSQL tests
 pytest
 ```
 
 Notice that tests have dependencies to packages [ahjo](https://pypi.org/project/ahjo/) and [SQL Alchemy](https://pypi.org/project/SQLAlchemy/). To succesfully run SQL Server tests, you must have permissions to create a new database in instance.
 
+## MSI installers
+
+Palje can be packaged into an MSI installer which can be used to install it into a Windows environment and easily update it later. Installers are self-contained, meaning that the package contains everything that is needed for running Palje (e.g. required parts of Python installation and all the 3rd party libraries and their dependencies are included).
+
+### Types of MSI installers
+
+There two types of installers, `user` and `system`. The `user` installer is suitable for single-user installations e.g. for a user who wants to run palje on their own workstation. For shared use, e.g. Azure Virtual Desktop, the `system` installer may be the better option: once installed, the tools are available for all users on that machine.
+
+**Notice:** using the `system` installer requires administrator priviledges.
+
+### Local MSI builds
+
+**Notice:** using an unsigned installer can end up with Windows Defender blocking Palje as malware. There is an ALM Partners developer signing key available to overcome this problem. Ask team TA3 for help if you need to sign development MSIs for testing purposes.
+
+To set up an environment for MSI builds, create a new venv, activate it, and install build dependencies.
+
+```
+python venv <name-of-venv>
+./<name-of-venv>/Scripts/activate
+pip install .[msibuild]
+```
+
+To build a `user` installer, use commands:
+
+```
+$env:PALJE_MSI_TARGET_TYPE="user"
+python ./msi_build.py bdist_msi
+```
+
+To build a `system` installer, use commands:
+
+```
+$env:PALJE_MSI_TARGET_TYPE="system"
+python ./msi_build.py bdist_msi
+```
+
+**Notice:** if you make changes to the code, you __must re-install the palje__ package (`pip install .` or `pip install .[msibuild]`) into the build venv for the changes to be included in the next MSI build. Editable installs don't work here, so don't use them!
+
 # License
 Copyright 2021 ALM Partners Oy
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
```

## Comparing `palje-2.0.0.dist-info/RECORD` & `palje-2.1.0.dist-info/RECORD`

 * *Files 27% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 palje/__init__.py,sha256=p9MBmsdR1dkfxDNT_vLYuaLIbq6vTLRYuRAJKjWontc,131
-palje/__main__.py,sha256=5GWf6HmWaHDCVIYdigSMkkLxKqsq7cGpoZryk1E0Sko,10408
+palje/__main__.py,sha256=ztpnkCM0ovCXVyvgvSUO6fq18wSPJIlr3figpa5WFUI,10422
 palje/confluence_rest.py,sha256=WvEAxBUpMiGYuAozbqLtxoPLJD-QHRo0KqV5XqRn7Ws,7152
 palje/mssql_database.py,sha256=h4DMmR8aKe6mBbOu4ugL3w_qVOeNruG86dOK1tjLqmA,10947
 palje/storage_format.py,sha256=K3fbZslt-BHmSdsnDKV7C8m0PmQ1HRpW1AxLN7yN8Y4,4256
-palje/version.py,sha256=hje97DjNnjjzdk2AwQsDgJXvORhASGZ-8JywrlJVLIw,427
+palje/version.py,sha256=RNKDW89EC1jx19YzwFi-xpYjE252Ld4fuY3bcovr8-s,427
 palje/queries/database_queries.ini,sha256=oZnh7P02rfiNDQFCcgqG5jNPWbdDhQPa4A-CJ_eRTRk,10126
-palje-2.0.0.dist-info/LICENSE,sha256=WtjCEwlcVzkh1ziO35P2qfVEkLjr87Flro7xlHz3CEY,11556
-palje-2.0.0.dist-info/METADATA,sha256=I4TuQ2fHaZK2J5uZ_W0KJn1LaXfZc8SQ8KIeasmkitU,21369
-palje-2.0.0.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-palje-2.0.0.dist-info/entry_points.txt,sha256=oeN2UDXpBFxr2Irspa8WJO3L-HVeoYQb7OFdYr5z6kg,46
-palje-2.0.0.dist-info/top_level.txt,sha256=n64ANesnvcj7pdU1ifEXOLLWMzNK4jiK4Arx76WooIA,6
-palje-2.0.0.dist-info/RECORD,,
+palje-2.1.0.dist-info/LICENSE,sha256=WtjCEwlcVzkh1ziO35P2qfVEkLjr87Flro7xlHz3CEY,11556
+palje-2.1.0.dist-info/METADATA,sha256=_D1kwmgyunbN8wjeT9y5kqgCmjVQs9HAc14gRajK6BY,23307
+palje-2.1.0.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+palje-2.1.0.dist-info/entry_points.txt,sha256=oeN2UDXpBFxr2Irspa8WJO3L-HVeoYQb7OFdYr5z6kg,46
+palje-2.1.0.dist-info/top_level.txt,sha256=n64ANesnvcj7pdU1ifEXOLLWMzNK4jiK4Arx76WooIA,6
+palje-2.1.0.dist-info/RECORD,,
```

