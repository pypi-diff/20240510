# Comparing `tmp/constellate-0.8.5.tar.gz` & `tmp/constellate-0.8.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "constellate-0.8.5.tar", last modified: Sun May  5 14:12:53 2024, max compression
+gzip compressed data, was "constellate-0.8.7.tar", last modified: Fri May 10 01:38:44 2024, max compression
```

## Comparing `constellate-0.8.5.tar` & `constellate-0.8.7.tar`

### file list

```diff
@@ -1,281 +1,286 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 14:12:53.268925 constellate-0.8.5/
--rw-rw-rw-   0 root         (0) root         (0)       47 2024-05-05 14:11:47.000000 constellate-0.8.5/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       42 2024-05-05 14:11:47.000000 constellate-0.8.5/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     3553 2024-05-05 14:12:53.268925 constellate-0.8.5/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      893 2024-05-05 14:11:47.000000 constellate-0.8.5/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 14:12:53.228923 constellate-0.8.5/constellate/
--rwxrwxrwx   0 root         (0) root         (0)        0 2024-05-05 14:11:47.000000 constellate-0.8.5/constellate/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       23 2024-05-05 14:11:47.000000 constellate-0.8.5/constellate/__version__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 14:12:53.228923 constellate-0.8.5/constellate/cli/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-05 14:11:47.000000 constellate-0.8.5/constellate/cli/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 14:12:53.228923 constellate-0.8.5/constellate/cli/argument/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-05 14:11:47.000000 constellate-0.8.5/constellate/cli/argument/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1410 2024-05-05 14:11:47.000000 constellate-0.8.5/constellate/cli/argument/unparse.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 14:12:53.228923 constellate-0.8.5/constellate/compression/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-05 14:11:47.000000 constellate-0.8.5/constellate/compression/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 14:12:53.232924 constellate-0.8.5/constellate/compression/zip/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-05 14:11:47.000000 constellate-0.8.5/constellate/compression/zip/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2575 2024-05-05 14:11:47.000000 constellate-0.8.5/constellate/compression/zip/zip.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 14:12:53.232924 constellate-0.8.5/constellate/concurrency/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-05 14:11:47.000000 constellate-0.8.5/constellate/concurrency/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 14:12:53.232924 constellate-0.8.5/constellate/concurrency/asyncio/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-05 14:11:47.000000 constellate-0.8.5/constellate/concurrency/asyncio/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3009 2024-05-05 14:11:47.000000 constellate-0.8.5/constellate/concurrency/asyncio/tasks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 14:12:53.232924 constellate-0.8.5/constellate/concurrency/pebble/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-05 14:11:47.000000 constellate-0.8.5/constellate/concurrency/pebble/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2683 2024-05-05 14:11:47.000000 constellate-0.8.5/constellate/concurrency/pebble/pool_cleanup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 14:12:53.232924 constellate-0.8.5/constellate/concurrency/simple/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-05 14:11:47.000000 constellate-0.8.5/constellate/concurrency/simple/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4057 2024-05-05 14:11:47.000000 constellate-0.8.5/constellate/concurrency/simple/simple.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 14:12:53.232924 constellate-0.8.5/constellate/concurrency/std/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-05 14:11:47.000000 constellate-0.8.5/constellate/concurrency/std/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      591 2024-05-05 14:11:47.000000 constellate-0.8.5/constellate/concurrency/std/pool.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 14:12:53.232924 constellate-0.8.5/constellate/constant/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-05 14:11:47.000000 constellate-0.8.5/constellate/constant/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      250 2024-05-05 14:11:47.000000 constellate-0.8.5/constellate/constant/concurrency.py
--rw-rw-rw-   0 root         (0) root         (0)       22 2024-05-05 14:11:47.000000 constellate-0.8.5/constellate/constant/debug.py
--rw-rw-rw-   0 root         (0) root         (0)      102 2024-05-05 14:11:47.000000 constellate-0.8.5/constellate/constant/platform.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 14:12:53.232924 constellate-0.8.5/constellate/container/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-05 14:11:47.000000 constellate-0.8.5/constellate/container/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 14:12:53.232924 constellate-0.8.5/constellate/container/orchestration/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-05 14:11:47.000000 constellate-0.8.5/constellate/container/orchestration/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 14:12:53.232924 constellate-0.8.5/constellate/container/orchestration/k8s/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-05 14:11:47.000000 constellate-0.8.5/constellate/container/orchestration/k8s/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      447 2024-05-05 14:11:47.000000 constellate-0.8.5/constellate/container/orchestration/k8s/probe.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 14:12:53.232924 constellate-0.8.5/constellate/cryptography/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-05 14:11:47.000000 constellate-0.8.5/constellate/cryptography/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 14:12:53.232924 constellate-0.8.5/constellate/cryptography/digest/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-05 14:11:47.000000 constellate-0.8.5/constellate/cryptography/digest/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1793 2024-05-05 14:11:47.000000 constellate-0.8.5/constellate/cryptography/digest/hexadecimal.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 14:12:53.232924 constellate-0.8.5/constellate/database/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-05 14:11:47.000000 constellate-0.8.5/constellate/database/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 14:12:53.236924 constellate-0.8.5/constellate/database/common/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-05 14:11:47.000000 constellate-0.8.5/constellate/database/common/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      121 2024-05-05 14:11:47.000000 constellate-0.8.5/constellate/database/common/databasetype.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 14:12:53.236924 constellate-0.8.5/constellate/database/migration/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-05 14:11:47.000000 constellate-0.8.5/constellate/database/migration/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      697 2024-05-05 14:11:47.000000 constellate-0.8.5/constellate/database/migration/constant.py
--rw-rw-rw-   0 root         (0) root         (0)     2220 2024-05-05 14:11:47.000000 constellate-0.8.5/constellate/database/migration/metadata.py
--rw-rw-rw-   0 root         (0) root         (0)     6720 2024-05-05 14:11:47.000000 constellate-0.8.5/constellate/database/migration/migrate.py
--rw-rw-rw-   0 root         (0) root         (0)     3429 2024-05-05 14:11:47.000000 constellate-0.8.5/constellate/database/migration/migrationcontext.py
--rw-rw-rw-   0 root         (0) root         (0)     9643 2024-05-05 14:11:47.000000 constellate-0.8.5/constellate/database/migration/migrationstep.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 14:12:53.236924 constellate-0.8.5/constellate/database/migration/standard/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-05 14:11:47.000000 constellate-0.8.5/constellate/database/migration/standard/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      445 2024-05-05 14:11:47.000000 constellate-0.8.5/constellate/database/migration/standard/base.py
--rw-rw-rw-   0 root         (0) root         (0)    22342 2024-05-05 14:11:47.000000 constellate-0.8.5/constellate/database/migration/standard/migrate.py
--rw-rw-rw-   0 root         (0) root         (0)     2492 2024-05-05 14:11:47.000000 constellate-0.8.5/constellate/database/migration/standard/table.py
--rw-rw-rw-   0 root         (0) root         (0)      372 2024-05-05 14:11:47.000000 constellate-0.8.5/constellate/database/migration/tablecontext.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 14:12:53.236924 constellate-0.8.5/constellate/database/sparql/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-05 14:11:47.000000 constellate-0.8.5/constellate/database/sparql/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      544 2024-05-05 14:11:47.000000 constellate-0.8.5/constellate/database/sparql/query.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 14:12:53.236924 constellate-0.8.5/constellate/database/sparql/sparqlburger/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-05 14:11:47.000000 constellate-0.8.5/constellate/database/sparql/sparqlburger/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      553 2024-05-05 14:11:47.000000 constellate-0.8.5/constellate/database/sparql/sparqlburger/triple.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 14:12:53.240924 constellate-0.8.5/constellate/database/sqlalchemy/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-05 14:11:47.000000 constellate-0.8.5/constellate/database/sqlalchemy/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 14:12:53.240924 constellate-0.8.5/constellate/database/sqlalchemy/crud/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-05 14:11:47.000000 constellate-0.8.5/constellate/database/sqlalchemy/crud/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6311 2024-05-05 14:11:47.000000 constellate-0.8.5/constellate/database/sqlalchemy/crud/cru.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 14:12:53.240924 constellate-0.8.5/constellate/database/sqlalchemy/exception/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-05 14:11:47.000000 constellate-0.8.5/constellate/database/sqlalchemy/exception/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       46 2024-05-05 14:11:47.000000 constellate-0.8.5/constellate/database/sqlalchemy/exception/migrationexception.py
--rw-rw-rw-   0 root         (0) root         (0)       42 2024-05-05 14:11:47.000000 constellate-0.8.5/constellate/database/sqlalchemy/exception/vacumexception.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 14:12:53.240924 constellate-0.8.5/constellate/database/sqlalchemy/execution/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-05 14:11:47.000000 constellate-0.8.5/constellate/database/sqlalchemy/execution/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7472 2024-05-05 14:11:47.000000 constellate-0.8.5/constellate/database/sqlalchemy/execution/execute.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 14:12:53.240924 constellate-0.8.5/constellate/database/sqlalchemy/expression/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-05 14:11:47.000000 constellate-0.8.5/constellate/database/sqlalchemy/expression/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 14:12:53.240924 constellate-0.8.5/constellate/database/sqlalchemy/expression/schema/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-05 14:11:47.000000 constellate-0.8.5/constellate/database/sqlalchemy/expression/schema/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1510 2024-05-05 14:11:47.000000 constellate-0.8.5/constellate/database/sqlalchemy/expression/schema/create.py
--rw-rw-rw-   0 root         (0) root         (0)     1230 2024-05-05 14:11:47.000000 constellate-0.8.5/constellate/database/sqlalchemy/expression/schema/drop.py
--rw-rw-rw-   0 root         (0) root         (0)     1690 2024-05-05 14:11:47.000000 constellate-0.8.5/constellate/database/sqlalchemy/expression/schema/setsearchpath.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 14:12:53.240924 constellate-0.8.5/constellate/database/sqlalchemy/expression/table/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-05 14:11:47.000000 constellate-0.8.5/constellate/database/sqlalchemy/expression/table/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2344 2024-05-05 14:11:47.000000 constellate-0.8.5/constellate/database/sqlalchemy/expression/table/drop.py
--rw-rw-rw-   0 root         (0) root         (0)     1641 2024-05-05 14:11:47.000000 constellate-0.8.5/constellate/database/sqlalchemy/expression/table/lock.py
--rw-rw-rw-   0 root         (0) root         (0)     3546 2024-05-05 14:11:47.000000 constellate-0.8.5/constellate/database/sqlalchemy/expression/table/presence.py
--rw-rw-rw-   0 root         (0) root         (0)     1105 2024-05-05 14:11:47.000000 constellate-0.8.5/constellate/database/sqlalchemy/expression/table/truncate.py
--rw-rw-rw-   0 root         (0) root         (0)      180 2024-05-05 14:11:47.000000 constellate-0.8.5/constellate/database/sqlalchemy/relationshiptype.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 14:12:53.244924 constellate-0.8.5/constellate/database/sqlalchemy/session/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-05 14:11:47.000000 constellate-0.8.5/constellate/database/sqlalchemy/session/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 14:12:53.244924 constellate-0.8.5/constellate/database/sqlalchemy/session/binder/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-05 14:11:47.000000 constellate-0.8.5/constellate/database/sqlalchemy/session/binder/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1813 2024-05-05 14:11:47.000000 constellate-0.8.5/constellate/database/sqlalchemy/session/binder/binderresolver.py
--rw-rw-rw-   0 root         (0) root         (0)     6094 2024-05-05 14:11:47.000000 constellate-0.8.5/constellate/database/sqlalchemy/session/multienginesession.py
--rw-rw-rw-   0 root         (0) root         (0)     3781 2024-05-05 14:11:47.000000 constellate-0.8.5/constellate/database/sqlalchemy/session/syncmultienginesession.py
--rw-rw-rw-   0 root         (0) root         (0)     3097 2024-05-05 14:11:47.000000 constellate-0.8.5/constellate/database/sqlalchemy/session/syncmultiengineshardsession.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 14:12:53.244924 constellate-0.8.5/constellate/database/sqlalchemy/sharding/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-05 14:11:47.000000 constellate-0.8.5/constellate/database/sqlalchemy/sharding/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7054 2024-05-05 14:11:47.000000 constellate-0.8.5/constellate/database/sqlalchemy/sharding/sharder.py
--rw-rw-rw-   0 root         (0) root         (0)      529 2024-05-05 14:11:47.000000 constellate-0.8.5/constellate/database/sqlalchemy/sharding/shardoption.py
--rw-rw-rw-   0 root         (0) root         (0)     2468 2024-05-05 14:11:47.000000 constellate-0.8.5/constellate/database/sqlalchemy/sharding/simplesession.py
--rw-rw-rw-   0 root         (0) root         (0)     2104 2024-05-05 14:11:47.000000 constellate-0.8.5/constellate/database/sqlalchemy/sharding/unittoshardmixin.py
--rw-rw-rw-   0 root         (0) root         (0)    32171 2024-05-05 14:11:47.000000 constellate-0.8.5/constellate/database/sqlalchemy/sqlalchemy.py
--rw-rw-rw-   0 root         (0) root         (0)      810 2024-05-05 14:11:47.000000 constellate-0.8.5/constellate/database/sqlalchemy/sqlalchemydbconfig.py
--rw-rw-rw-   0 root         (0) root         (0)     1477 2024-05-05 14:11:47.000000 constellate-0.8.5/constellate/database/sqlalchemy/sqlalchemydbconfigmanager.py
--rw-rw-rw-   0 root         (0) root         (0)     1004 2024-05-05 14:11:47.000000 constellate-0.8.5/constellate/database/sqlalchemy/sqlalchemyengineconfig.py
--rw-rw-rw-   0 root         (0) root         (0)      215 2024-05-05 14:11:47.000000 constellate-0.8.5/constellate/database/sqlalchemy/sqlalchemymigrationconfig.py
--rw-rw-rw-   0 root         (0) root         (0)    13143 2024-05-05 14:11:47.000000 constellate-0.8.5/constellate/database/sqlalchemy/sqlalchemypostgresql.py
--rw-rw-rw-   0 root         (0) root         (0)     9929 2024-05-05 14:11:47.000000 constellate-0.8.5/constellate/database/sqlalchemy/sqlalchemysqlite3.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 14:12:53.244924 constellate-0.8.5/constellate/database/sqlalchemy/typedecorator/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-05 14:11:47.000000 constellate-0.8.5/constellate/database/sqlalchemy/typedecorator/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      756 2024-05-05 14:11:47.000000 constellate-0.8.5/constellate/database/sqlalchemy/typedecorator/enuminteger.py
--rw-rw-rw-   0 root         (0) root         (0)      755 2024-05-05 14:11:47.000000 constellate-0.8.5/constellate/database/sqlalchemy/typedecorator/enumstring.py
--rw-rw-rw-   0 root         (0) root         (0)     2097 2024-05-05 14:11:47.000000 constellate-0.8.5/constellate/database/sqlalchemy/typedecorator/enumvalue.py
--rw-rw-rw-   0 root         (0) root         (0)      576 2024-05-05 14:11:47.000000 constellate-0.8.5/constellate/database/sqlalchemy/typedecorator/timestamptz.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 14:12:53.244924 constellate-0.8.5/constellate/database/sqlalchemy/types/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-05 14:11:47.000000 constellate-0.8.5/constellate/database/sqlalchemy/types/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    16098 2024-05-05 14:11:47.000000 constellate-0.8.5/constellate/database/sqlalchemy/types/composite.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 14:12:53.244924 constellate-0.8.5/constellate/database/sqlalchemy/utils/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-05 14:11:47.000000 constellate-0.8.5/constellate/database/sqlalchemy/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      479 2024-05-05 14:11:47.000000 constellate-0.8.5/constellate/database/sqlalchemy/utils/sessioncommit.py
--rw-rw-rw-   0 root         (0) root         (0)     1681 2024-05-05 14:11:47.000000 constellate-0.8.5/constellate/database/sqlalchemy/utils/sql_query.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 14:12:53.244924 constellate-0.8.5/constellate/database/sqlite3/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-05 14:11:47.000000 constellate-0.8.5/constellate/database/sqlite3/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1932 2024-05-05 14:11:47.000000 constellate-0.8.5/constellate/database/sqlite3/sqlite3.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 14:12:53.244924 constellate-0.8.5/constellate/datatype/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-05 14:11:47.000000 constellate-0.8.5/constellate/datatype/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 14:12:53.244924 constellate-0.8.5/constellate/datatype/dictionary/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-05 14:11:47.000000 constellate-0.8.5/constellate/datatype/dictionary/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      383 2024-05-05 14:11:47.000000 constellate-0.8.5/constellate/datatype/dictionary/pop.py
--rw-rw-rw-   0 root         (0) root         (0)      663 2024-05-05 14:11:47.000000 constellate-0.8.5/constellate/datatype/dictionary/update.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 14:12:53.248924 constellate-0.8.5/constellate/datatype/enum/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-05 14:11:47.000000 constellate-0.8.5/constellate/datatype/enum/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      350 2024-05-05 14:11:47.000000 constellate-0.8.5/constellate/datatype/enum/enum.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 14:12:53.248924 constellate-0.8.5/constellate/datetime/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-05 14:11:47.000000 constellate-0.8.5/constellate/datetime/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 14:12:53.248924 constellate-0.8.5/constellate/datetime/timeinterval/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-05 14:11:47.000000 constellate-0.8.5/constellate/datetime/timeinterval/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    10941 2024-05-05 14:11:47.000000 constellate-0.8.5/constellate/datetime/timeinterval/timeinterval.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 14:12:53.248924 constellate-0.8.5/constellate/debug/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-05 14:11:47.000000 constellate-0.8.5/constellate/debug/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 14:12:53.248924 constellate-0.8.5/constellate/debug/packages/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-05 14:11:47.000000 constellate-0.8.5/constellate/debug/packages/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       88 2024-05-05 14:11:47.000000 constellate-0.8.5/constellate/debug/packages/package.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 14:12:53.248924 constellate-0.8.5/constellate/debugger/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-05 14:11:47.000000 constellate-0.8.5/constellate/debugger/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1374 2024-05-05 14:11:47.000000 constellate-0.8.5/constellate/debugger/debugger.py
--rw-rw-rw-   0 root         (0) root         (0)      737 2024-05-05 14:11:47.000000 constellate-0.8.5/constellate/debugger/simple.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 14:12:53.248924 constellate-0.8.5/constellate/logger/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-05 14:11:47.000000 constellate-0.8.5/constellate/logger/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 14:12:53.248924 constellate-0.8.5/constellate/logger/formatter/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-05 14:11:47.000000 constellate-0.8.5/constellate/logger/formatter/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      785 2024-05-05 14:11:47.000000 constellate-0.8.5/constellate/logger/formatter/formatterfactory.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 14:12:53.252924 constellate-0.8.5/constellate/logger/handler/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-05 14:11:47.000000 constellate-0.8.5/constellate/logger/handler/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      562 2024-05-05 14:11:47.000000 constellate-0.8.5/constellate/logger/handler/forwarderhandler.py
--rw-rw-rw-   0 root         (0) root         (0)      569 2024-05-05 14:11:47.000000 constellate-0.8.5/constellate/logger/handler/stringhandler.py
--rw-rw-rw-   0 root         (0) root         (0)    20086 2024-05-05 14:11:47.000000 constellate-0.8.5/constellate/logger/log.py
--rw-rw-rw-   0 root         (0) root         (0)     3980 2024-05-05 14:11:47.000000 constellate-0.8.5/constellate/logger/loggers.py
--rw-rw-rw-   0 root         (0) root         (0)      652 2024-05-05 14:11:47.000000 constellate-0.8.5/constellate/logger/logmode.py
--rw-rw-rw-   0 root         (0) root         (0)     3050 2024-05-05 14:11:47.000000 constellate-0.8.5/constellate/logger/simple.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 14:12:53.252924 constellate-0.8.5/constellate/network/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-05 14:11:47.000000 constellate-0.8.5/constellate/network/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 14:12:53.252924 constellate-0.8.5/constellate/network/download/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-05 14:11:47.000000 constellate-0.8.5/constellate/network/download/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 14:12:53.252924 constellate-0.8.5/constellate/network/url/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-05 14:11:47.000000 constellate-0.8.5/constellate/network/url/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      248 2024-05-05 14:11:47.000000 constellate-0.8.5/constellate/network/url/unshortener.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 14:12:53.252924 constellate-0.8.5/constellate/package/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-05 14:11:47.000000 constellate-0.8.5/constellate/package/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      173 2024-05-05 14:11:47.000000 constellate-0.8.5/constellate/package/package.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 14:12:53.252924 constellate-0.8.5/constellate/pretty/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-05 14:11:47.000000 constellate-0.8.5/constellate/pretty/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 14:12:53.252924 constellate-0.8.5/constellate/pretty/log/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-05 14:11:47.000000 constellate-0.8.5/constellate/pretty/log/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      350 2024-05-05 14:11:47.000000 constellate-0.8.5/constellate/pretty/log/line.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 14:12:53.252924 constellate-0.8.5/constellate/progression/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-05 14:11:47.000000 constellate-0.8.5/constellate/progression/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1013 2024-05-05 14:11:47.000000 constellate-0.8.5/constellate/progression/progres.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 14:12:53.252924 constellate-0.8.5/constellate/project/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-05 14:11:47.000000 constellate-0.8.5/constellate/project/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      202 2024-05-05 14:11:47.000000 constellate-0.8.5/constellate/project/version.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-05 14:11:47.000000 constellate-0.8.5/constellate/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 14:12:53.252924 constellate-0.8.5/constellate/resource/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-05 14:11:47.000000 constellate-0.8.5/constellate/resource/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2206 2024-05-05 14:11:47.000000 constellate-0.8.5/constellate/resource/resource.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 14:12:53.252924 constellate-0.8.5/constellate/storage/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-05 14:11:47.000000 constellate-0.8.5/constellate/storage/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 14:12:53.252924 constellate-0.8.5/constellate/storage/filesystem/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-05 14:11:47.000000 constellate-0.8.5/constellate/storage/filesystem/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 14:12:53.256924 constellate-0.8.5/constellate/storage/filesystem/anyfs/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-05 14:11:47.000000 constellate-0.8.5/constellate/storage/filesystem/anyfs/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      127 2024-05-05 14:11:47.000000 constellate-0.8.5/constellate/storage/filesystem/anyfs/availability.py
--rw-rw-rw-   0 root         (0) root         (0)     3808 2024-05-05 14:11:47.000000 constellate-0.8.5/constellate/storage/filesystem/anyfs/path.py
--rw-rw-rw-   0 root         (0) root         (0)      264 2024-05-05 14:11:47.000000 constellate-0.8.5/constellate/storage/filesystem/anyfs/size.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 14:12:53.256924 constellate-0.8.5/constellate/storage/filesystem/tmpfs/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-05 14:11:47.000000 constellate-0.8.5/constellate/storage/filesystem/tmpfs/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6635 2024-05-05 14:11:47.000000 constellate-0.8.5/constellate/storage/filesystem/tmpfs/memory_tempfile.py
--rw-rw-rw-   0 root         (0) root         (0)     2631 2024-05-05 14:11:47.000000 constellate-0.8.5/constellate/storage/filesystem/tmpfs/rambacked.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 14:12:53.256924 constellate-0.8.5/constellate/testing/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-05 14:11:47.000000 constellate-0.8.5/constellate/testing/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 14:12:53.256924 constellate-0.8.5/constellate/testing/mock/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-05 14:11:47.000000 constellate-0.8.5/constellate/testing/mock/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      374 2024-05-05 14:11:47.000000 constellate-0.8.5/constellate/testing/mock/argv.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 14:12:53.256924 constellate-0.8.5/constellate/thirdparty/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-05 14:11:47.000000 constellate-0.8.5/constellate/thirdparty/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 14:12:53.256924 constellate-0.8.5/constellate/thirdparty/numba/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-05 14:11:47.000000 constellate-0.8.5/constellate/thirdparty/numba/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 14:12:53.256924 constellate-0.8.5/constellate/thirdparty/numba/progress/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-05 14:11:47.000000 constellate-0.8.5/constellate/thirdparty/numba/progress/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1040 2024-05-05 14:11:47.000000 constellate-0.8.5/constellate/thirdparty/numba/progress/progress.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 14:12:53.256924 constellate-0.8.5/constellate/thirdparty/pandas/
--rw-rw-rw-   0 root         (0) root         (0)      763 2024-05-05 14:11:47.000000 constellate-0.8.5/constellate/thirdparty/pandas/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 14:12:53.256924 constellate-0.8.5/constellate/thirdparty/pandas/accessor/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-05 14:11:47.000000 constellate-0.8.5/constellate/thirdparty/pandas/accessor/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3173 2024-05-05 14:11:47.000000 constellate-0.8.5/constellate/thirdparty/pandas/accessor/attribute_accessor.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 14:12:53.256924 constellate-0.8.5/constellate/thirdparty/pandas/extra/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-05 14:11:47.000000 constellate-0.8.5/constellate/thirdparty/pandas/extra/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 14:12:53.256924 constellate-0.8.5/constellate/thirdparty/pandas/extra/sanitize/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-05 14:11:47.000000 constellate-0.8.5/constellate/thirdparty/pandas/extra/sanitize/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    11079 2024-05-05 14:11:47.000000 constellate-0.8.5/constellate/thirdparty/pandas/extra/sanitize/sanitize.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 14:12:53.256924 constellate-0.8.5/constellate/thirdparty/pandas/io/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-05 14:11:47.000000 constellate-0.8.5/constellate/thirdparty/pandas/io/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 14:12:53.260924 constellate-0.8.5/constellate/thirdparty/pandas/io/sql/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-05 14:11:47.000000 constellate-0.8.5/constellate/thirdparty/pandas/io/sql/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2552 2024-05-05 14:11:47.000000 constellate-0.8.5/constellate/thirdparty/pandas/io/sql/sqlalchemy.py
--rw-rw-rw-   0 root         (0) root         (0)      565 2024-05-05 14:11:47.000000 constellate-0.8.5/constellate/thirdparty/pandas/io/sql/sqlalchemy_engine.py
--rw-rw-rw-   0 root         (0) root         (0)     1127 2024-05-05 14:11:47.000000 constellate-0.8.5/constellate/thirdparty/pandas/io/sql/sqlalchemy_execution_option.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 14:12:53.260924 constellate-0.8.5/constellate/thirdparty/pandas/operation/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-05 14:11:47.000000 constellate-0.8.5/constellate/thirdparty/pandas/operation/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 14:12:53.260924 constellate-0.8.5/constellate/thirdparty/pandas/operation/introspection/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-05 14:11:47.000000 constellate-0.8.5/constellate/thirdparty/pandas/operation/introspection/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      336 2024-05-05 14:11:47.000000 constellate-0.8.5/constellate/thirdparty/pandas/operation/introspection/introspection.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 14:12:53.260924 constellate-0.8.5/constellate/thirdparty/pandas/validation/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-05 14:11:47.000000 constellate-0.8.5/constellate/thirdparty/pandas/validation/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      624 2024-05-05 14:11:47.000000 constellate-0.8.5/constellate/thirdparty/pandas/validation/pandera.py
--rw-rw-rw-   0 root         (0) root         (0)     6050 2024-05-05 14:11:47.000000 constellate-0.8.5/constellate/thirdparty/pandas/validation/validation.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 14:12:53.260924 constellate-0.8.5/constellate/thirdparty/pandera/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-05 14:11:47.000000 constellate-0.8.5/constellate/thirdparty/pandera/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1623 2024-05-05 14:11:47.000000 constellate-0.8.5/constellate/thirdparty/pandera/inspector.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 14:12:53.260924 constellate-0.8.5/constellate/virtualization/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-05 14:11:47.000000 constellate-0.8.5/constellate/virtualization/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 14:12:53.260924 constellate-0.8.5/constellate/virtualization/common/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-05 14:11:47.000000 constellate-0.8.5/constellate/virtualization/common/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      214 2024-05-05 14:11:47.000000 constellate-0.8.5/constellate/virtualization/common/common.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 14:12:53.260924 constellate-0.8.5/constellate/virtualization/docker/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-05 14:11:47.000000 constellate-0.8.5/constellate/virtualization/docker/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 14:12:53.264924 constellate-0.8.5/constellate.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3553 2024-05-05 14:12:53.000000 constellate-0.8.5/constellate.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     8588 2024-05-05 14:12:53.000000 constellate-0.8.5/constellate.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-05 14:12:53.000000 constellate-0.8.5/constellate.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      737 2024-05-05 14:12:53.000000 constellate-0.8.5/constellate.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2024-05-05 14:12:53.000000 constellate-0.8.5/constellate.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)     2790 2024-05-05 14:11:47.000000 constellate-0.8.5/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)      162 2024-05-05 14:12:53.268925 constellate-0.8.5/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 14:12:53.264924 constellate-0.8.5/tests/
--rw-rw-rw-   0 root         (0) root         (0)     1074 2024-05-05 14:11:47.000000 constellate-0.8.5/tests/test_cli_argument.py
--rw-rw-rw-   0 root         (0) root         (0)      751 2024-05-05 14:11:47.000000 constellate-0.8.5/tests/test_compression.py
--rw-rw-rw-   0 root         (0) root         (0)     1021 2024-05-05 14:11:47.000000 constellate-0.8.5/tests/test_concurrency.py
--rw-rw-rw-   0 root         (0) root         (0)      863 2024-05-05 14:11:47.000000 constellate-0.8.5/tests/test_cryptography.py
--rw-rw-rw-   0 root         (0) root         (0)     1373 2024-05-05 14:11:47.000000 constellate-0.8.5/tests/test_enum.py
--rw-rw-rw-   0 root         (0) root         (0)     9696 2024-05-05 14:11:47.000000 constellate-0.8.5/tests/test_logger.py
--rw-rw-rw-   0 root         (0) root         (0)    19319 2024-05-05 14:11:47.000000 constellate-0.8.5/tests/test_migration.py
--rw-rw-rw-   0 root         (0) root         (0)     8652 2024-05-05 14:11:47.000000 constellate-0.8.5/tests/test_pandas.py
--rw-rw-rw-   0 root         (0) root         (0)      942 2024-05-05 14:11:47.000000 constellate-0.8.5/tests/test_pandera.py
--rw-rw-rw-   0 root         (0) root         (0)      846 2024-05-05 14:11:47.000000 constellate-0.8.5/tests/test_progression.py
--rw-rw-rw-   0 root         (0) root         (0)      465 2024-05-05 14:11:47.000000 constellate-0.8.5/tests/test_resource.py
--rw-rw-rw-   0 root         (0) root         (0)     1988 2024-05-05 14:11:47.000000 constellate-0.8.5/tests/test_sparql.py
--rw-rw-rw-   0 root         (0) root         (0)    11500 2024-05-05 14:11:47.000000 constellate-0.8.5/tests/test_sqlalchemy.py
--rw-rw-rw-   0 root         (0) root         (0)     1738 2024-05-05 14:11:47.000000 constellate-0.8.5/tests/test_storage_filesystem_tmpfs_rambacked.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 01:38:44.295883 constellate-0.8.7/
+-rw-rw-rw-   0 root         (0) root         (0)       47 2024-05-10 01:37:42.000000 constellate-0.8.7/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       42 2024-05-10 01:37:42.000000 constellate-0.8.7/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     3919 2024-05-10 01:38:44.295883 constellate-0.8.7/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      893 2024-05-10 01:37:42.000000 constellate-0.8.7/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 01:38:44.263882 constellate-0.8.7/constellate/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2024-05-10 01:37:42.000000 constellate-0.8.7/constellate/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       23 2024-05-10 01:37:42.000000 constellate-0.8.7/constellate/__version__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 01:38:44.263882 constellate-0.8.7/constellate/cli/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-10 01:37:42.000000 constellate-0.8.7/constellate/cli/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 01:38:44.263882 constellate-0.8.7/constellate/cli/argument/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-10 01:37:42.000000 constellate-0.8.7/constellate/cli/argument/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1406 2024-05-10 01:37:42.000000 constellate-0.8.7/constellate/cli/argument/unparse.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 01:38:44.263882 constellate-0.8.7/constellate/compression/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-10 01:37:42.000000 constellate-0.8.7/constellate/compression/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 01:38:44.263882 constellate-0.8.7/constellate/compression/zip/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-10 01:37:42.000000 constellate-0.8.7/constellate/compression/zip/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2576 2024-05-10 01:37:42.000000 constellate-0.8.7/constellate/compression/zip/zip.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 01:38:44.263882 constellate-0.8.7/constellate/compression/zstd/
+-rw-rw-rw-   0 root         (0) root         (0)      606 2024-05-10 01:37:42.000000 constellate-0.8.7/constellate/compression/zstd/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1630 2024-05-10 01:37:42.000000 constellate-0.8.7/constellate/compression/zstd/common.py
+-rw-rw-rw-   0 root         (0) root         (0)     2102 2024-05-10 01:37:42.000000 constellate-0.8.7/constellate/compression/zstd/pyzstd.py
+-rw-rw-rw-   0 root         (0) root         (0)     1798 2024-05-10 01:37:42.000000 constellate-0.8.7/constellate/compression/zstd/zstandard.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 01:38:44.263882 constellate-0.8.7/constellate/concurrency/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-10 01:37:42.000000 constellate-0.8.7/constellate/concurrency/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 01:38:44.263882 constellate-0.8.7/constellate/concurrency/asyncio/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-10 01:37:42.000000 constellate-0.8.7/constellate/concurrency/asyncio/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3031 2024-05-10 01:37:42.000000 constellate-0.8.7/constellate/concurrency/asyncio/tasks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 01:38:44.263882 constellate-0.8.7/constellate/concurrency/pebble/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-10 01:37:42.000000 constellate-0.8.7/constellate/concurrency/pebble/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2792 2024-05-10 01:37:42.000000 constellate-0.8.7/constellate/concurrency/pebble/pool_cleanup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 01:38:44.267882 constellate-0.8.7/constellate/concurrency/simple/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-10 01:37:42.000000 constellate-0.8.7/constellate/concurrency/simple/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4057 2024-05-10 01:37:42.000000 constellate-0.8.7/constellate/concurrency/simple/simple.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 01:38:44.267882 constellate-0.8.7/constellate/concurrency/std/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-10 01:37:42.000000 constellate-0.8.7/constellate/concurrency/std/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      591 2024-05-10 01:37:42.000000 constellate-0.8.7/constellate/concurrency/std/pool.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 01:38:44.267882 constellate-0.8.7/constellate/constant/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-10 01:37:42.000000 constellate-0.8.7/constellate/constant/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      250 2024-05-10 01:37:42.000000 constellate-0.8.7/constellate/constant/concurrency.py
+-rw-rw-rw-   0 root         (0) root         (0)       22 2024-05-10 01:37:42.000000 constellate-0.8.7/constellate/constant/debug.py
+-rw-rw-rw-   0 root         (0) root         (0)      102 2024-05-10 01:37:42.000000 constellate-0.8.7/constellate/constant/platform.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 01:38:44.267882 constellate-0.8.7/constellate/container/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-10 01:37:42.000000 constellate-0.8.7/constellate/container/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 01:38:44.267882 constellate-0.8.7/constellate/container/orchestration/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-10 01:37:42.000000 constellate-0.8.7/constellate/container/orchestration/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 01:38:44.267882 constellate-0.8.7/constellate/container/orchestration/k8s/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-10 01:37:42.000000 constellate-0.8.7/constellate/container/orchestration/k8s/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      447 2024-05-10 01:37:42.000000 constellate-0.8.7/constellate/container/orchestration/k8s/probe.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 01:38:44.267882 constellate-0.8.7/constellate/cryptography/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-10 01:37:42.000000 constellate-0.8.7/constellate/cryptography/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 01:38:44.267882 constellate-0.8.7/constellate/cryptography/digest/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-10 01:37:42.000000 constellate-0.8.7/constellate/cryptography/digest/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1780 2024-05-10 01:37:42.000000 constellate-0.8.7/constellate/cryptography/digest/hexadecimal.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 01:38:44.267882 constellate-0.8.7/constellate/database/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-10 01:37:42.000000 constellate-0.8.7/constellate/database/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 01:38:44.267882 constellate-0.8.7/constellate/database/common/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-10 01:37:42.000000 constellate-0.8.7/constellate/database/common/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      121 2024-05-10 01:37:42.000000 constellate-0.8.7/constellate/database/common/databasetype.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 01:38:44.267882 constellate-0.8.7/constellate/database/migration/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-10 01:37:42.000000 constellate-0.8.7/constellate/database/migration/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      697 2024-05-10 01:37:42.000000 constellate-0.8.7/constellate/database/migration/constant.py
+-rw-rw-rw-   0 root         (0) root         (0)     2220 2024-05-10 01:37:42.000000 constellate-0.8.7/constellate/database/migration/metadata.py
+-rw-rw-rw-   0 root         (0) root         (0)     6720 2024-05-10 01:37:42.000000 constellate-0.8.7/constellate/database/migration/migrate.py
+-rw-rw-rw-   0 root         (0) root         (0)     3429 2024-05-10 01:37:42.000000 constellate-0.8.7/constellate/database/migration/migrationcontext.py
+-rw-rw-rw-   0 root         (0) root         (0)     9700 2024-05-10 01:37:42.000000 constellate-0.8.7/constellate/database/migration/migrationstep.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 01:38:44.267882 constellate-0.8.7/constellate/database/migration/standard/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-10 01:37:42.000000 constellate-0.8.7/constellate/database/migration/standard/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      445 2024-05-10 01:37:42.000000 constellate-0.8.7/constellate/database/migration/standard/base.py
+-rw-rw-rw-   0 root         (0) root         (0)    22342 2024-05-10 01:37:42.000000 constellate-0.8.7/constellate/database/migration/standard/migrate.py
+-rw-rw-rw-   0 root         (0) root         (0)     2492 2024-05-10 01:37:42.000000 constellate-0.8.7/constellate/database/migration/standard/table.py
+-rw-rw-rw-   0 root         (0) root         (0)      372 2024-05-10 01:37:42.000000 constellate-0.8.7/constellate/database/migration/tablecontext.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 01:38:44.267882 constellate-0.8.7/constellate/database/sparql/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-10 01:37:42.000000 constellate-0.8.7/constellate/database/sparql/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      633 2024-05-10 01:37:42.000000 constellate-0.8.7/constellate/database/sparql/query.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 01:38:44.271882 constellate-0.8.7/constellate/database/sparql/sparqlburger/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-10 01:37:42.000000 constellate-0.8.7/constellate/database/sparql/sparqlburger/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      553 2024-05-10 01:37:42.000000 constellate-0.8.7/constellate/database/sparql/sparqlburger/triple.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 01:38:44.271882 constellate-0.8.7/constellate/database/sqlalchemy/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-10 01:37:42.000000 constellate-0.8.7/constellate/database/sqlalchemy/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 01:38:44.271882 constellate-0.8.7/constellate/database/sqlalchemy/crud/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-10 01:37:42.000000 constellate-0.8.7/constellate/database/sqlalchemy/crud/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6311 2024-05-10 01:37:42.000000 constellate-0.8.7/constellate/database/sqlalchemy/crud/cru.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 01:38:44.271882 constellate-0.8.7/constellate/database/sqlalchemy/exception/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-10 01:37:42.000000 constellate-0.8.7/constellate/database/sqlalchemy/exception/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       46 2024-05-10 01:37:42.000000 constellate-0.8.7/constellate/database/sqlalchemy/exception/migrationexception.py
+-rw-rw-rw-   0 root         (0) root         (0)       42 2024-05-10 01:37:42.000000 constellate-0.8.7/constellate/database/sqlalchemy/exception/vacumexception.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 01:38:44.271882 constellate-0.8.7/constellate/database/sqlalchemy/execution/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-10 01:37:42.000000 constellate-0.8.7/constellate/database/sqlalchemy/execution/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7472 2024-05-10 01:37:42.000000 constellate-0.8.7/constellate/database/sqlalchemy/execution/execute.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 01:38:44.271882 constellate-0.8.7/constellate/database/sqlalchemy/expression/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-10 01:37:42.000000 constellate-0.8.7/constellate/database/sqlalchemy/expression/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 01:38:44.271882 constellate-0.8.7/constellate/database/sqlalchemy/expression/schema/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-10 01:37:42.000000 constellate-0.8.7/constellate/database/sqlalchemy/expression/schema/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1510 2024-05-10 01:37:42.000000 constellate-0.8.7/constellate/database/sqlalchemy/expression/schema/create.py
+-rw-rw-rw-   0 root         (0) root         (0)     1230 2024-05-10 01:37:42.000000 constellate-0.8.7/constellate/database/sqlalchemy/expression/schema/drop.py
+-rw-rw-rw-   0 root         (0) root         (0)     1690 2024-05-10 01:37:42.000000 constellate-0.8.7/constellate/database/sqlalchemy/expression/schema/setsearchpath.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 01:38:44.271882 constellate-0.8.7/constellate/database/sqlalchemy/expression/table/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-10 01:37:42.000000 constellate-0.8.7/constellate/database/sqlalchemy/expression/table/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2344 2024-05-10 01:37:42.000000 constellate-0.8.7/constellate/database/sqlalchemy/expression/table/drop.py
+-rw-rw-rw-   0 root         (0) root         (0)     1641 2024-05-10 01:37:42.000000 constellate-0.8.7/constellate/database/sqlalchemy/expression/table/lock.py
+-rw-rw-rw-   0 root         (0) root         (0)     3546 2024-05-10 01:37:42.000000 constellate-0.8.7/constellate/database/sqlalchemy/expression/table/presence.py
+-rw-rw-rw-   0 root         (0) root         (0)     1105 2024-05-10 01:37:42.000000 constellate-0.8.7/constellate/database/sqlalchemy/expression/table/truncate.py
+-rw-rw-rw-   0 root         (0) root         (0)      180 2024-05-10 01:37:42.000000 constellate-0.8.7/constellate/database/sqlalchemy/relationshiptype.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 01:38:44.275882 constellate-0.8.7/constellate/database/sqlalchemy/session/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-10 01:37:42.000000 constellate-0.8.7/constellate/database/sqlalchemy/session/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 01:38:44.275882 constellate-0.8.7/constellate/database/sqlalchemy/session/binder/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-10 01:37:42.000000 constellate-0.8.7/constellate/database/sqlalchemy/session/binder/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1813 2024-05-10 01:37:42.000000 constellate-0.8.7/constellate/database/sqlalchemy/session/binder/binderresolver.py
+-rw-rw-rw-   0 root         (0) root         (0)     6094 2024-05-10 01:37:42.000000 constellate-0.8.7/constellate/database/sqlalchemy/session/multienginesession.py
+-rw-rw-rw-   0 root         (0) root         (0)     3781 2024-05-10 01:37:42.000000 constellate-0.8.7/constellate/database/sqlalchemy/session/syncmultienginesession.py
+-rw-rw-rw-   0 root         (0) root         (0)     3097 2024-05-10 01:37:42.000000 constellate-0.8.7/constellate/database/sqlalchemy/session/syncmultiengineshardsession.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 01:38:44.275882 constellate-0.8.7/constellate/database/sqlalchemy/sharding/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-10 01:37:42.000000 constellate-0.8.7/constellate/database/sqlalchemy/sharding/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7054 2024-05-10 01:37:42.000000 constellate-0.8.7/constellate/database/sqlalchemy/sharding/sharder.py
+-rw-rw-rw-   0 root         (0) root         (0)      529 2024-05-10 01:37:42.000000 constellate-0.8.7/constellate/database/sqlalchemy/sharding/shardoption.py
+-rw-rw-rw-   0 root         (0) root         (0)     2468 2024-05-10 01:37:42.000000 constellate-0.8.7/constellate/database/sqlalchemy/sharding/simplesession.py
+-rw-rw-rw-   0 root         (0) root         (0)     2104 2024-05-10 01:37:42.000000 constellate-0.8.7/constellate/database/sqlalchemy/sharding/unittoshardmixin.py
+-rw-rw-rw-   0 root         (0) root         (0)    32171 2024-05-10 01:37:42.000000 constellate-0.8.7/constellate/database/sqlalchemy/sqlalchemy.py
+-rw-rw-rw-   0 root         (0) root         (0)      810 2024-05-10 01:37:42.000000 constellate-0.8.7/constellate/database/sqlalchemy/sqlalchemydbconfig.py
+-rw-rw-rw-   0 root         (0) root         (0)     1477 2024-05-10 01:37:42.000000 constellate-0.8.7/constellate/database/sqlalchemy/sqlalchemydbconfigmanager.py
+-rw-rw-rw-   0 root         (0) root         (0)     1004 2024-05-10 01:37:42.000000 constellate-0.8.7/constellate/database/sqlalchemy/sqlalchemyengineconfig.py
+-rw-rw-rw-   0 root         (0) root         (0)      215 2024-05-10 01:37:42.000000 constellate-0.8.7/constellate/database/sqlalchemy/sqlalchemymigrationconfig.py
+-rw-rw-rw-   0 root         (0) root         (0)    13143 2024-05-10 01:37:42.000000 constellate-0.8.7/constellate/database/sqlalchemy/sqlalchemypostgresql.py
+-rw-rw-rw-   0 root         (0) root         (0)     9929 2024-05-10 01:37:42.000000 constellate-0.8.7/constellate/database/sqlalchemy/sqlalchemysqlite3.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 01:38:44.275882 constellate-0.8.7/constellate/database/sqlalchemy/typedecorator/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-10 01:37:42.000000 constellate-0.8.7/constellate/database/sqlalchemy/typedecorator/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      756 2024-05-10 01:37:42.000000 constellate-0.8.7/constellate/database/sqlalchemy/typedecorator/enuminteger.py
+-rw-rw-rw-   0 root         (0) root         (0)      755 2024-05-10 01:37:42.000000 constellate-0.8.7/constellate/database/sqlalchemy/typedecorator/enumstring.py
+-rw-rw-rw-   0 root         (0) root         (0)     2097 2024-05-10 01:37:42.000000 constellate-0.8.7/constellate/database/sqlalchemy/typedecorator/enumvalue.py
+-rw-rw-rw-   0 root         (0) root         (0)      576 2024-05-10 01:37:42.000000 constellate-0.8.7/constellate/database/sqlalchemy/typedecorator/timestamptz.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 01:38:44.275882 constellate-0.8.7/constellate/database/sqlalchemy/types/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-10 01:37:42.000000 constellate-0.8.7/constellate/database/sqlalchemy/types/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    16098 2024-05-10 01:37:42.000000 constellate-0.8.7/constellate/database/sqlalchemy/types/composite.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 01:38:44.275882 constellate-0.8.7/constellate/database/sqlalchemy/utils/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-10 01:37:42.000000 constellate-0.8.7/constellate/database/sqlalchemy/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      479 2024-05-10 01:37:42.000000 constellate-0.8.7/constellate/database/sqlalchemy/utils/sessioncommit.py
+-rw-rw-rw-   0 root         (0) root         (0)     1681 2024-05-10 01:37:42.000000 constellate-0.8.7/constellate/database/sqlalchemy/utils/sql_query.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 01:38:44.275882 constellate-0.8.7/constellate/database/sqlite3/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-10 01:37:42.000000 constellate-0.8.7/constellate/database/sqlite3/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2000 2024-05-10 01:37:42.000000 constellate-0.8.7/constellate/database/sqlite3/sqlite3.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 01:38:44.275882 constellate-0.8.7/constellate/datatype/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-10 01:37:42.000000 constellate-0.8.7/constellate/datatype/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 01:38:44.279882 constellate-0.8.7/constellate/datatype/dictionary/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-10 01:37:42.000000 constellate-0.8.7/constellate/datatype/dictionary/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      383 2024-05-10 01:37:42.000000 constellate-0.8.7/constellate/datatype/dictionary/pop.py
+-rw-rw-rw-   0 root         (0) root         (0)      663 2024-05-10 01:37:42.000000 constellate-0.8.7/constellate/datatype/dictionary/update.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 01:38:44.279882 constellate-0.8.7/constellate/datatype/enum/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-10 01:37:42.000000 constellate-0.8.7/constellate/datatype/enum/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      350 2024-05-10 01:37:42.000000 constellate-0.8.7/constellate/datatype/enum/enum.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 01:38:44.279882 constellate-0.8.7/constellate/datetime/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-10 01:37:42.000000 constellate-0.8.7/constellate/datetime/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 01:38:44.279882 constellate-0.8.7/constellate/datetime/timeinterval/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-10 01:37:42.000000 constellate-0.8.7/constellate/datetime/timeinterval/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    10689 2024-05-10 01:37:42.000000 constellate-0.8.7/constellate/datetime/timeinterval/timeinterval.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 01:38:44.279882 constellate-0.8.7/constellate/debug/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-10 01:37:42.000000 constellate-0.8.7/constellate/debug/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 01:38:44.279882 constellate-0.8.7/constellate/debug/packages/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-10 01:37:42.000000 constellate-0.8.7/constellate/debug/packages/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       88 2024-05-10 01:37:42.000000 constellate-0.8.7/constellate/debug/packages/package.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 01:38:44.279882 constellate-0.8.7/constellate/debugger/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-10 01:37:42.000000 constellate-0.8.7/constellate/debugger/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1376 2024-05-10 01:37:42.000000 constellate-0.8.7/constellate/debugger/debugger.py
+-rw-rw-rw-   0 root         (0) root         (0)      737 2024-05-10 01:37:42.000000 constellate-0.8.7/constellate/debugger/simple.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 01:38:44.279882 constellate-0.8.7/constellate/logger/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-10 01:37:42.000000 constellate-0.8.7/constellate/logger/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 01:38:44.279882 constellate-0.8.7/constellate/logger/formatter/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-10 01:37:42.000000 constellate-0.8.7/constellate/logger/formatter/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      770 2024-05-10 01:37:42.000000 constellate-0.8.7/constellate/logger/formatter/formatterfactory.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 01:38:44.283882 constellate-0.8.7/constellate/logger/handler/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-10 01:37:42.000000 constellate-0.8.7/constellate/logger/handler/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      562 2024-05-10 01:37:42.000000 constellate-0.8.7/constellate/logger/handler/forwarderhandler.py
+-rw-rw-rw-   0 root         (0) root         (0)      572 2024-05-10 01:37:42.000000 constellate-0.8.7/constellate/logger/handler/stringhandler.py
+-rw-rw-rw-   0 root         (0) root         (0)    20171 2024-05-10 01:37:42.000000 constellate-0.8.7/constellate/logger/log.py
+-rw-rw-rw-   0 root         (0) root         (0)     3980 2024-05-10 01:37:42.000000 constellate-0.8.7/constellate/logger/loggers.py
+-rw-rw-rw-   0 root         (0) root         (0)      652 2024-05-10 01:37:42.000000 constellate-0.8.7/constellate/logger/logmode.py
+-rw-rw-rw-   0 root         (0) root         (0)     3048 2024-05-10 01:37:42.000000 constellate-0.8.7/constellate/logger/simple.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 01:38:44.283882 constellate-0.8.7/constellate/network/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-10 01:37:42.000000 constellate-0.8.7/constellate/network/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 01:38:44.283882 constellate-0.8.7/constellate/network/download/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-10 01:37:42.000000 constellate-0.8.7/constellate/network/download/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 01:38:44.283882 constellate-0.8.7/constellate/network/url/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-10 01:37:42.000000 constellate-0.8.7/constellate/network/url/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      248 2024-05-10 01:37:42.000000 constellate-0.8.7/constellate/network/url/unshortener.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 01:38:44.283882 constellate-0.8.7/constellate/package/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-10 01:37:42.000000 constellate-0.8.7/constellate/package/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      173 2024-05-10 01:37:42.000000 constellate-0.8.7/constellate/package/package.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 01:38:44.283882 constellate-0.8.7/constellate/pretty/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-10 01:37:42.000000 constellate-0.8.7/constellate/pretty/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 01:38:44.283882 constellate-0.8.7/constellate/pretty/log/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-10 01:37:42.000000 constellate-0.8.7/constellate/pretty/log/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      350 2024-05-10 01:37:42.000000 constellate-0.8.7/constellate/pretty/log/line.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 01:38:44.283882 constellate-0.8.7/constellate/progression/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-10 01:37:42.000000 constellate-0.8.7/constellate/progression/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1016 2024-05-10 01:37:42.000000 constellate-0.8.7/constellate/progression/progres.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 01:38:44.283882 constellate-0.8.7/constellate/project/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-10 01:37:42.000000 constellate-0.8.7/constellate/project/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      202 2024-05-10 01:37:42.000000 constellate-0.8.7/constellate/project/version.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-10 01:37:42.000000 constellate-0.8.7/constellate/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 01:38:44.283882 constellate-0.8.7/constellate/resource/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-10 01:37:42.000000 constellate-0.8.7/constellate/resource/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2171 2024-05-10 01:37:42.000000 constellate-0.8.7/constellate/resource/resource.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 01:38:44.283882 constellate-0.8.7/constellate/storage/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-10 01:37:42.000000 constellate-0.8.7/constellate/storage/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 01:38:44.283882 constellate-0.8.7/constellate/storage/filesystem/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-10 01:37:42.000000 constellate-0.8.7/constellate/storage/filesystem/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 01:38:44.283882 constellate-0.8.7/constellate/storage/filesystem/anyfs/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-10 01:37:42.000000 constellate-0.8.7/constellate/storage/filesystem/anyfs/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      127 2024-05-10 01:37:42.000000 constellate-0.8.7/constellate/storage/filesystem/anyfs/availability.py
+-rw-rw-rw-   0 root         (0) root         (0)     3804 2024-05-10 01:37:42.000000 constellate-0.8.7/constellate/storage/filesystem/anyfs/path.py
+-rw-rw-rw-   0 root         (0) root         (0)      264 2024-05-10 01:37:42.000000 constellate-0.8.7/constellate/storage/filesystem/anyfs/size.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 01:38:44.283882 constellate-0.8.7/constellate/storage/filesystem/tmpfs/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-10 01:37:42.000000 constellate-0.8.7/constellate/storage/filesystem/tmpfs/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6635 2024-05-10 01:37:42.000000 constellate-0.8.7/constellate/storage/filesystem/tmpfs/memory_tempfile.py
+-rw-rw-rw-   0 root         (0) root         (0)     2692 2024-05-10 01:37:42.000000 constellate-0.8.7/constellate/storage/filesystem/tmpfs/rambacked.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 01:38:44.283882 constellate-0.8.7/constellate/testing/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-10 01:37:42.000000 constellate-0.8.7/constellate/testing/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 01:38:44.283882 constellate-0.8.7/constellate/testing/mock/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-10 01:37:42.000000 constellate-0.8.7/constellate/testing/mock/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      374 2024-05-10 01:37:42.000000 constellate-0.8.7/constellate/testing/mock/argv.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 01:38:44.283882 constellate-0.8.7/constellate/thirdparty/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-10 01:37:42.000000 constellate-0.8.7/constellate/thirdparty/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 01:38:44.283882 constellate-0.8.7/constellate/thirdparty/numba/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-10 01:37:42.000000 constellate-0.8.7/constellate/thirdparty/numba/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 01:38:44.283882 constellate-0.8.7/constellate/thirdparty/numba/progress/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-10 01:37:42.000000 constellate-0.8.7/constellate/thirdparty/numba/progress/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1040 2024-05-10 01:37:42.000000 constellate-0.8.7/constellate/thirdparty/numba/progress/progress.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 01:38:44.287882 constellate-0.8.7/constellate/thirdparty/pandas/
+-rw-rw-rw-   0 root         (0) root         (0)      763 2024-05-10 01:37:42.000000 constellate-0.8.7/constellate/thirdparty/pandas/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 01:38:44.287882 constellate-0.8.7/constellate/thirdparty/pandas/accessor/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-10 01:37:42.000000 constellate-0.8.7/constellate/thirdparty/pandas/accessor/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3173 2024-05-10 01:37:42.000000 constellate-0.8.7/constellate/thirdparty/pandas/accessor/attribute_accessor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 01:38:44.287882 constellate-0.8.7/constellate/thirdparty/pandas/extra/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-10 01:37:42.000000 constellate-0.8.7/constellate/thirdparty/pandas/extra/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 01:38:44.287882 constellate-0.8.7/constellate/thirdparty/pandas/extra/sanitize/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-10 01:37:42.000000 constellate-0.8.7/constellate/thirdparty/pandas/extra/sanitize/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11051 2024-05-10 01:37:42.000000 constellate-0.8.7/constellate/thirdparty/pandas/extra/sanitize/sanitize.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 01:38:44.287882 constellate-0.8.7/constellate/thirdparty/pandas/io/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-10 01:37:42.000000 constellate-0.8.7/constellate/thirdparty/pandas/io/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 01:38:44.287882 constellate-0.8.7/constellate/thirdparty/pandas/io/sql/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-10 01:37:42.000000 constellate-0.8.7/constellate/thirdparty/pandas/io/sql/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2553 2024-05-10 01:37:42.000000 constellate-0.8.7/constellate/thirdparty/pandas/io/sql/sqlalchemy.py
+-rw-rw-rw-   0 root         (0) root         (0)      565 2024-05-10 01:37:42.000000 constellate-0.8.7/constellate/thirdparty/pandas/io/sql/sqlalchemy_engine.py
+-rw-rw-rw-   0 root         (0) root         (0)     1124 2024-05-10 01:37:42.000000 constellate-0.8.7/constellate/thirdparty/pandas/io/sql/sqlalchemy_execution_option.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 01:38:44.287882 constellate-0.8.7/constellate/thirdparty/pandas/operation/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-10 01:37:42.000000 constellate-0.8.7/constellate/thirdparty/pandas/operation/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 01:38:44.287882 constellate-0.8.7/constellate/thirdparty/pandas/operation/introspection/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-10 01:37:42.000000 constellate-0.8.7/constellate/thirdparty/pandas/operation/introspection/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      336 2024-05-10 01:37:42.000000 constellate-0.8.7/constellate/thirdparty/pandas/operation/introspection/introspection.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 01:38:44.287882 constellate-0.8.7/constellate/thirdparty/pandas/validation/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-10 01:37:42.000000 constellate-0.8.7/constellate/thirdparty/pandas/validation/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      696 2024-05-10 01:37:42.000000 constellate-0.8.7/constellate/thirdparty/pandas/validation/pandera.py
+-rw-rw-rw-   0 root         (0) root         (0)     7088 2024-05-10 01:37:42.000000 constellate-0.8.7/constellate/thirdparty/pandas/validation/validation.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 01:38:44.287882 constellate-0.8.7/constellate/thirdparty/pandera/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-10 01:37:42.000000 constellate-0.8.7/constellate/thirdparty/pandera/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1802 2024-05-10 01:37:42.000000 constellate-0.8.7/constellate/thirdparty/pandera/inspector.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 01:38:44.287882 constellate-0.8.7/constellate/virtualization/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-10 01:37:42.000000 constellate-0.8.7/constellate/virtualization/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 01:38:44.287882 constellate-0.8.7/constellate/virtualization/common/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-10 01:37:42.000000 constellate-0.8.7/constellate/virtualization/common/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      214 2024-05-10 01:37:42.000000 constellate-0.8.7/constellate/virtualization/common/common.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 01:38:44.287882 constellate-0.8.7/constellate/virtualization/docker/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-10 01:37:42.000000 constellate-0.8.7/constellate/virtualization/docker/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 01:38:44.291883 constellate-0.8.7/constellate.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3919 2024-05-10 01:38:44.000000 constellate-0.8.7/constellate.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     8749 2024-05-10 01:38:44.000000 constellate-0.8.7/constellate.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-10 01:38:44.000000 constellate-0.8.7/constellate.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      904 2024-05-10 01:38:44.000000 constellate-0.8.7/constellate.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2024-05-10 01:38:44.000000 constellate-0.8.7/constellate.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)     3085 2024-05-10 01:37:42.000000 constellate-0.8.7/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)      162 2024-05-10 01:38:44.295883 constellate-0.8.7/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 01:38:44.291883 constellate-0.8.7/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     1074 2024-05-10 01:37:42.000000 constellate-0.8.7/tests/test_cli_argument.py
+-rw-rw-rw-   0 root         (0) root         (0)     1385 2024-05-10 01:37:42.000000 constellate-0.8.7/tests/test_compression.py
+-rw-rw-rw-   0 root         (0) root         (0)      941 2024-05-10 01:37:42.000000 constellate-0.8.7/tests/test_concurrency.py
+-rw-rw-rw-   0 root         (0) root         (0)      863 2024-05-10 01:37:42.000000 constellate-0.8.7/tests/test_cryptography.py
+-rw-rw-rw-   0 root         (0) root         (0)     1373 2024-05-10 01:37:42.000000 constellate-0.8.7/tests/test_enum.py
+-rw-rw-rw-   0 root         (0) root         (0)     9700 2024-05-10 01:37:42.000000 constellate-0.8.7/tests/test_logger.py
+-rw-rw-rw-   0 root         (0) root         (0)    19319 2024-05-10 01:37:42.000000 constellate-0.8.7/tests/test_migration.py
+-rw-rw-rw-   0 root         (0) root         (0)     8679 2024-05-10 01:37:42.000000 constellate-0.8.7/tests/test_pandas.py
+-rw-rw-rw-   0 root         (0) root         (0)      942 2024-05-10 01:37:42.000000 constellate-0.8.7/tests/test_pandera.py
+-rw-rw-rw-   0 root         (0) root         (0)      846 2024-05-10 01:37:42.000000 constellate-0.8.7/tests/test_progression.py
+-rw-rw-rw-   0 root         (0) root         (0)      465 2024-05-10 01:37:42.000000 constellate-0.8.7/tests/test_resource.py
+-rw-rw-rw-   0 root         (0) root         (0)     1988 2024-05-10 01:37:42.000000 constellate-0.8.7/tests/test_sparql.py
+-rw-rw-rw-   0 root         (0) root         (0)    11500 2024-05-10 01:37:42.000000 constellate-0.8.7/tests/test_sqlalchemy.py
+-rw-rw-rw-   0 root         (0) root         (0)     1738 2024-05-10 01:37:42.000000 constellate-0.8.7/tests/test_storage_filesystem_tmpfs_rambacked.py
```

### Comparing `constellate-0.8.5/PKG-INFO` & `constellate-0.8.7/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: constellate
-Version: 0.8.5
+Version: 0.8.7
 Summary: A bunch of utilities aggregated over time
 Author-email: David Andreoletti <none@provided.yet>
 Project-URL: repository, https://github.com/davidandreoletti/constellate
 Keywords: constellate
 Classifier: License :: Other/Proprietary License
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -17,57 +17,64 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: <3.13,>=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
-Requires-Dist: Pebble>=4.6.3
 Requires-Dist: decorator>=5.1.0
 Requires-Dist: aioitertools>=0.8.0
 Requires-Dist: psutil>=5.7.0
 Requires-Dist: pendulum>=2.1.2
 Requires-Dist: requests>=2.25.0
 Requires-Dist: memory-tempfile>=2.2.3
-Requires-Dist: narration>=0.2.16
 Requires-Dist: bidict>=0.21.4
 Requires-Dist: attrs>=20.3.0
 Requires-Dist: portion>=2.2.0
 Requires-Dist: jsonmerge>=1.8.0
 Requires-Dist: jsonschema>=4.7.2
 Requires-Dist: Deprecated>=1.2.12
 Requires-Dist: importlib-resources>=5.1.4
 Requires-Dist: typing-extensions>=4.3.0
 Requires-Dist: tqdm>=4.62.3
 Requires-Dist: regex>=2021.11.10
 Requires-Dist: blake3>=0.3.1
 Requires-Dist: sqlparse>=0.4.2
 Requires-Dist: stackeddag>=0.3.3
-Provides-Extra: cli-args
-Requires-Dist: argunparse>=0.1.3; extra == "cli-args"
+Provides-Extra: cliargs
+Requires-Dist: argunparse>=0.1.3; extra == "cliargs"
 Provides-Extra: sqlalchemy
 Requires-Dist: SQLAlchemy>=2.0.11; extra == "sqlalchemy"
 Requires-Dist: sqlalchemy-utils>=0.37.9; extra == "sqlalchemy"
 Requires-Dist: sqlalchemy-json>=0.4.0; extra == "sqlalchemy"
 Requires-Dist: sqlalchemy_mixins>=2.0; extra == "sqlalchemy"
 Requires-Dist: aiosqlite>=0.17.0; extra == "sqlalchemy"
 Requires-Dist: asyncpg>=0.23.0; extra == "sqlalchemy"
 Requires-Dist: networkx>=2.8.5; extra == "sqlalchemy"
 Provides-Extra: pandas
-Requires-Dist: pandas>=1.3.4; extra == "pandas"
+Requires-Dist: pandas>=2.0.0; extra == "pandas"
 Requires-Dist: pandas-log>=0.1.7; extra == "pandas"
-Requires-Dist: pandera!=0.13.4,>=0.14.5; extra == "pandas"
+Requires-Dist: pandera!=0.13.4,>=0.19.0; extra == "pandas"
 Requires-Dist: hypothesis>=6.54.4; extra == "pandas"
 Provides-Extra: numpy
 Requires-Dist: numpy>=1.21.4; extra == "numpy"
 Provides-Extra: numba
 Requires-Dist: numba-progress>=0.0.3; extra == "numba"
 Provides-Extra: sparql
 Requires-Dist: rdflib>=6.3.0; extra == "sparql"
 Requires-Dist: SPARQL-Burger>=1.0.2; extra == "sparql"
+Provides-Extra: zstd
+Requires-Dist: pyzstd>=0.15.10; extra == "zstd"
+Provides-Extra: logging
+Requires-Dist: narration>=0.2.17; extra == "logging"
+Requires-Dist: colorlog>=6.8.2; extra == "logging"
+Provides-Extra: concurrencypebble
+Requires-Dist: Pebble>=4.6.3; extra == "concurrencypebble"
+Provides-Extra: all
+Requires-Dist: constellate[cliargs,concurrencypebble,logging,numba,numpy,pandas,sparql,sqlalchemy,zstd]; extra == "all"
 
 .. image:: https://img.shields.io/pypi/v/constellate.svg
 .. image:: https://img.shields.io/pypi/pyversions/constellate.svg
 .. image:: https://img.shields.io/pypi/status/constellate.svg
 .. image:: https://img.shields.io/pypi/l/constellate.svg
 
 constellate
```

### Comparing `constellate-0.8.5/README.rst` & `constellate-0.8.7/README.rst`

 * *Files identical despite different names*

### Comparing `constellate-0.8.5/constellate/cli/argument/unparse.py` & `constellate-0.8.7/constellate/cli/argument/unparse.py`

 * *Files 22% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
     to_arg_unparse(command="cmd", sub_command="sub", options=['foo', True, 'bar', 'baz', 'bar', 'baz'], args=['file.txt'])
     > cmd sub --foo --bar=baz --bar=baz2 file.txt
 
     """
     unparser = argunparse.ArgumentUnparser(**(argunparser_kwargs or {}))
 
-    data = list()
+    data = []
     if isinstance(options, Dict):
         data = unparser.unparse_options_and_args(options, arguments, to_list=True)
     elif isinstance(options, List):
         # Convert options in list of tuple
         it = iter(options)
         for k, v in list(zip(it, it)):
             if k is None:
```

### Comparing `constellate-0.8.5/constellate/compression/zip/zip.py` & `constellate-0.8.7/constellate/compression/zip/zip.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
 def create_ram_zip(compression: int = ZIP_STORED, allowZip64: bool = True) -> RAMZipConfig:
     buffer = BytesIO()
     mode = "a"
 
     config = RAMZipConfig(buffer=buffer, mode=mode, compression=compression, allowZip64=allowZip64)
 
-    with _zip_file_from_ram_zip_config(config=config) as zip_file:
+    with _zip_file_from_ram_zip_config(config=config) as _zip_file:
         #  file is created with mode 'w', 'x' or 'a' and then closed without adding any files to the archive,
         #  the appropriate ZIP structures for an empty archive will be written to the file.
         # src: https://docs.python.org/3/library/zipfile.html#zipfile.ZipFile
         return config
 
 
 @attr.s(kw_only=True, auto_attribs=True)
```

### Comparing `constellate-0.8.5/constellate/concurrency/asyncio/tasks.py` & `constellate-0.8.7/constellate/concurrency/asyncio/tasks.py`

 * *Files 7% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     TimeoutError when the timeout occurs before all Futures are done.
 
     Note: The futures 'f' are not necessarily members of fs.
     """
     if futures.isfuture(fs) or coroutines.iscoroutine(fs):
         raise TypeError(f"expect a list of futures, not {type(fs).__name__}")
 
-    SENTINEL = object()
+    sentinel_value = object()
     done = Queue()
 
     _priority = -1
     todo = {}
     for f in fs:
         _priority += 1
         todo[_priority] = ensure_future(f)
@@ -54,45 +54,45 @@
             return  # _on_timeout() was here first.
         priority = todo.inverse.pop(f, None)
         done.put_nowait((priority, f))
         if not todo and timeout_handle is not None:
             timeout_handle.cancel()
 
     async def _wait_for_one(expected_priority):
-        r = ready.pop(expected_priority, SENTINEL)
-        if r is not SENTINEL:
+        r = ready.pop(expected_priority, sentinel_value)
+        if r is not sentinel_value:
             return r
 
         priority, f = await done.get()
         if priority is None and f is None:
             # Dummy value from _on_timeout().
             raise asyncio.exceptions.TimeoutError
 
         try:
             r = f.result()  # May raise f.exception().
             ready[priority] = r
 
-            r = ready.pop(expected_priority, SENTINEL)
+            r = ready.pop(expected_priority, sentinel_value)
             return r
         except BaseException as e:
             if return_exception:
                 ready[priority] = e
                 return e
-            else:
-                # Propagate
-                raise e
+
+            # Propagate
+            raise e
 
     for priority, f in list(todo.items()):
         f.add_done_callback(_on_completion)
     if todo and timeout is not None:
-        timeout_handle = asyncio.call_later(timeout, _on_timeout)
+        loop = asyncio.get_running_loop()
+        timeout_handle = loop.call_later(timeout, _on_timeout)
 
     priority = -1
-    exhausted = False
     while len(list(todo.keys())) > 0:
         priority += 1
         result = await _wait_for_one(priority)
-        if result is not SENTINEL:
+        if result is not sentinel_value:
             yield result
         else:
             priority -= 1
         await asyncio.sleep(0)
```

### Comparing `constellate-0.8.5/constellate/concurrency/pebble/pool_cleanup.py` & `constellate-0.8.7/constellate/concurrency/pebble/pool_cleanup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 import logging
 import signal
 import threading
 from typing import Dict, List, Protocol
 
-import pebble as pebble
+import pebble
 
-"""
-Clean up pebble process pool on signals
-"""
+#
+# Clean up pebble process pool on signals
+#
 
 
 class PostPebblePoolCleanup(Protocol):
     def __call__(self, forced_shutdown: bool = False) -> None: ...
 
 
 def _pebble_cleanup_pool(
     force_shutdown: bool = False,
     pool: pebble.ProcessPool = None,
-    futures: List[pebble.ProcessFuture] = [],
+    futures: List[pebble.ProcessFuture] = None,
     post_cleanup: PostPebblePoolCleanup = None,
     logger: logging.Logger = None,
 ):
+    futures = futures or []
     # Cancel remaining tasks
     logger.debug("Cancelling tasks pool ...")
     for future in futures:
         if not future.done():
             future.cancel()
 
     if force_shutdown:
@@ -42,44 +43,47 @@
     if post_cleanup is not None:
         post_cleanup(force_shutdown=force_shutdown)
 
 
 def pebble_cleanup_pool(
     logger=None,
     pool: pebble.ProcessPool = None,
-    futures: List[pebble.ProcessFuture] = [],
+    futures: List[pebble.ProcessFuture] = None,
     post_cleanup: PostPebblePoolCleanup = None,
 ):
+    futures = futures or []
     _pebble_cleanup_pool(
         force_shutdown=False, logger=logger, pool=pool, futures=futures, post_cleanup=post_cleanup
     )
 
 
 def pebble_cleanup_pool_on_signal(
     force_shutdown: bool = False,
     logger=None,
     pool: pebble.ProcessPool = None,
-    futures: List[pebble.ProcessFuture] = [],
-    signals: Dict[int, str] = {signal.SIGINT: "SIGINT", signal.SIGTERM: "SIGTERM"},
+    futures: List[pebble.ProcessFuture] = None,
+    signals: Dict[int, str] = None,
     post_cleanup: PostPebblePoolCleanup = None,
 ):
     """Clean up pebble process pool on signals
 
     :param force_shutdown: bool:  (Default value = False)
     :param logger:  (Default value = None)
     :param pool: pebble.ProcessPool:  (Default value = None)
     :param futures: List[pebble.ProcessFuture]:  (Default value = [])
     :param signals: Dict[int:
     :param str]:  (Default value = {signal.SIGINT: "SIGINT")
     :param signal.SIGTERM: "SIGTERM"}:
     :param post_cleanup: PostPebblePoolCleanup:  (Default value = None)
 
     """
+    futures = futures or []
+    signals = signals or {signal.SIGINT: "SIGINT", signal.SIGTERM: "SIGTERM"}
 
-    def _handler(signum, _frame):
+    def _handler(_signum, _frame):
         # logger.critical(f"Received {signals.get(signum, signum)} signal ...")
         _pebble_cleanup_pool(
             force_shutdown=force_shutdown,
             logger=logger,
             pool=pool,
             futures=futures,
             post_cleanup=post_cleanup,
```

### Comparing `constellate-0.8.5/constellate/concurrency/simple/simple.py` & `constellate-0.8.7/constellate/concurrency/simple/simple.py`

 * *Files identical despite different names*

### Comparing `constellate-0.8.5/constellate/concurrency/std/pool.py` & `constellate-0.8.7/constellate/concurrency/std/pool.py`

 * *Files identical despite different names*

### Comparing `constellate-0.8.5/constellate/cryptography/digest/hexadecimal.py` & `constellate-0.8.7/constellate/cryptography/digest/hexadecimal.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,16 +21,16 @@
     """
     if family in hashlib.algorithms_available:
         return hashlib.new(family)
 
     family = family.lower()
     if family == "blake3":
         return blake3(**kwargs)
-    else:
-        raise NotImplementedError()
+
+    raise NotImplementedError()
 
 
 _hasher_fn = hasher
 
 
 def hexadecimal(
     family: str = None, hasher: Hasher = None, value: Union[str, bytes, Path] = None
```

### Comparing `constellate-0.8.5/constellate/database/migration/constant.py` & `constellate-0.8.7/constellate/database/migration/constant.py`

 * *Files identical despite different names*

### Comparing `constellate-0.8.5/constellate/database/migration/metadata.py` & `constellate-0.8.7/constellate/database/migration/metadata.py`

 * *Files identical despite different names*

### Comparing `constellate-0.8.5/constellate/database/migration/migrate.py` & `constellate-0.8.7/constellate/database/migration/migrate.py`

 * *Files identical despite different names*

### Comparing `constellate-0.8.5/constellate/database/migration/migrationcontext.py` & `constellate-0.8.7/constellate/database/migration/migrationcontext.py`

 * *Files identical despite different names*

### Comparing `constellate-0.8.5/constellate/database/migration/migrationstep.py` & `constellate-0.8.7/constellate/database/migration/migrationstep.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,19 +22,21 @@
     MigrationStepFile,
 )
 from constellate.resource.resource import get_folder
 
 
 def _collect_migration_files(
     migration_dir: Path = None,
-    suffixes: List[str] = ["*.sql", "*.py"],
+    suffixes: List[str] = None,
     invalid_files_names: List[str] = None,
     post_apply_files_names: List[str] = None,
     action: MigrationAction = None,
 ) -> List[Path]:
+    suffixes = suffixes or ["*.sql", "*.py"]
+
     def sort_alphabetically(files: List[Path] = None) -> List[Path]:
         return sorted(files, key=lambda f: str(f))
 
     def _keep_migration_file(infix: str, whitelist_files_names: List[str], file: Path) -> bool:
         def discard_non_migration_file(name):
             return str(name).endswith(file.name)
 
@@ -105,21 +107,21 @@
             )
 
         step_context = _load_module(file=step_context_file)
         kind = _read_property(step_context, "kind", (MigrationKind,), migration_context.kind)
         schema = _read_property(
             step_context, "schema", (str, type(List[str])), migration_context.schema
         )
-        dir = _read_property(step_context, "migration_dir", (Path,), step_directory)
+        migration_dir2 = _read_property(step_context, "migration_dir", (Path,), step_directory)
 
         invalid_files_names = list(
             set(INVALID_MIGRATION_SCRIPT_FILE_NAMES + [step_context_file.name])
         )
         migration_files = _collect_migration_files(
-            migration_dir=dir,
+            migration_dir=migration_dir2,
             invalid_files_names=invalid_files_names,
             post_apply_files_names=DEFAULT_POST_APPLY_FILE_NAMES,
             action=migration_context.action,
         )
 
         def _read_file_metadata(file: Path) -> Tuple[Any, Dict]:
             metadata = {
@@ -131,15 +133,15 @@
 
             directive_names = list(metadata.keys())
             if file.name.endswith(".py"):
                 pymodule = _load_module(file=file)
                 directives = {d: getattr(pymodule, d, None) for d in directive_names}
             elif file.name.endswith(".sql"):
                 pymodule = None
-                directives, leading_comment, statements = read_sql_migration_metadata(
+                directives, _leading_comment, _statements = read_sql_migration_metadata(
                     file=file, directive_names=directive_names
                 )
             else:
                 raise NotImplementedError()
 
             provided_metadata = {k: v for k, v in directives.items() if v is not None}
             return pymodule, dict(ChainMap(metadata, provided_metadata))
```

### Comparing `constellate-0.8.5/constellate/database/migration/standard/migrate.py` & `constellate-0.8.7/constellate/database/migration/standard/migrate.py`

 * *Files identical despite different names*

### Comparing `constellate-0.8.5/constellate/database/migration/standard/table.py` & `constellate-0.8.7/constellate/database/migration/standard/table.py`

 * *Files identical despite different names*

### Comparing `constellate-0.8.5/constellate/database/sparql/query.py` & `constellate-0.8.7/constellate/database/sparql/query.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,17 +4,20 @@
 from rdflib.store import Store
 
 
 def query(
     raw_query: str,
     graph: Graph = None,
     store: Store = None,
-    init_namespaces: Dict = {},
-    init_bindings: Dict = {},
+    init_namespaces: Dict = None,
+    init_bindings: Dict = None,
 ) -> Result:
     """
     Query a store, with provided query builder and bindings applied
 
     Usage: See unit tests
     """
+    init_namespaces = init_namespaces or {}
+    init_bindings = init_bindings or {}
+
     graph = Graph(store=store) if graph is None and store is None else graph
     return graph.query(raw_query, initNs=init_namespaces, initBindings=init_bindings)
```

### Comparing `constellate-0.8.5/constellate/database/sparql/sparqlburger/triple.py` & `constellate-0.8.7/constellate/database/sparql/sparqlburger/triple.py`

 * *Files identical despite different names*

### Comparing `constellate-0.8.5/constellate/database/sqlalchemy/crud/cru.py` & `constellate-0.8.7/constellate/database/sqlalchemy/crud/cru.py`

 * *Files identical despite different names*

### Comparing `constellate-0.8.5/constellate/database/sqlalchemy/execution/execute.py` & `constellate-0.8.7/constellate/database/sqlalchemy/execution/execute.py`

 * *Files identical despite different names*

### Comparing `constellate-0.8.5/constellate/database/sqlalchemy/expression/schema/create.py` & `constellate-0.8.7/constellate/database/sqlalchemy/expression/schema/create.py`

 * *Files identical despite different names*

### Comparing `constellate-0.8.5/constellate/database/sqlalchemy/expression/schema/drop.py` & `constellate-0.8.7/constellate/database/sqlalchemy/expression/schema/drop.py`

 * *Files identical despite different names*

### Comparing `constellate-0.8.5/constellate/database/sqlalchemy/expression/schema/setsearchpath.py` & `constellate-0.8.7/constellate/database/sqlalchemy/expression/schema/setsearchpath.py`

 * *Files identical despite different names*

### Comparing `constellate-0.8.5/constellate/database/sqlalchemy/expression/table/drop.py` & `constellate-0.8.7/constellate/database/sqlalchemy/expression/table/drop.py`

 * *Files identical despite different names*

### Comparing `constellate-0.8.5/constellate/database/sqlalchemy/expression/table/lock.py` & `constellate-0.8.7/constellate/database/sqlalchemy/expression/table/lock.py`

 * *Files identical despite different names*

### Comparing `constellate-0.8.5/constellate/database/sqlalchemy/expression/table/presence.py` & `constellate-0.8.7/constellate/database/sqlalchemy/expression/table/presence.py`

 * *Files identical despite different names*

### Comparing `constellate-0.8.5/constellate/database/sqlalchemy/expression/table/truncate.py` & `constellate-0.8.7/constellate/database/sqlalchemy/expression/table/truncate.py`

 * *Files identical despite different names*

### Comparing `constellate-0.8.5/constellate/database/sqlalchemy/session/binder/binderresolver.py` & `constellate-0.8.7/constellate/database/sqlalchemy/session/binder/binderresolver.py`

 * *Files identical despite different names*

### Comparing `constellate-0.8.5/constellate/database/sqlalchemy/session/multienginesession.py` & `constellate-0.8.7/constellate/database/sqlalchemy/session/multienginesession.py`

 * *Files identical despite different names*

### Comparing `constellate-0.8.5/constellate/database/sqlalchemy/session/syncmultienginesession.py` & `constellate-0.8.7/constellate/database/sqlalchemy/session/syncmultienginesession.py`

 * *Files identical despite different names*

### Comparing `constellate-0.8.5/constellate/database/sqlalchemy/session/syncmultiengineshardsession.py` & `constellate-0.8.7/constellate/database/sqlalchemy/session/syncmultiengineshardsession.py`

 * *Files identical despite different names*

### Comparing `constellate-0.8.5/constellate/database/sqlalchemy/sharding/sharder.py` & `constellate-0.8.7/constellate/database/sqlalchemy/sharding/sharder.py`

 * *Files identical despite different names*

### Comparing `constellate-0.8.5/constellate/database/sqlalchemy/sharding/shardoption.py` & `constellate-0.8.7/constellate/database/sqlalchemy/sharding/shardoption.py`

 * *Files identical despite different names*

### Comparing `constellate-0.8.5/constellate/database/sqlalchemy/sharding/simplesession.py` & `constellate-0.8.7/constellate/database/sqlalchemy/sharding/simplesession.py`

 * *Files identical despite different names*

### Comparing `constellate-0.8.5/constellate/database/sqlalchemy/sharding/unittoshardmixin.py` & `constellate-0.8.7/constellate/database/sqlalchemy/sharding/unittoshardmixin.py`

 * *Files identical despite different names*

### Comparing `constellate-0.8.5/constellate/database/sqlalchemy/sqlalchemy.py` & `constellate-0.8.7/constellate/database/sqlalchemy/sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `constellate-0.8.5/constellate/database/sqlalchemy/sqlalchemydbconfig.py` & `constellate-0.8.7/constellate/database/sqlalchemy/sqlalchemydbconfig.py`

 * *Files identical despite different names*

### Comparing `constellate-0.8.5/constellate/database/sqlalchemy/sqlalchemydbconfigmanager.py` & `constellate-0.8.7/constellate/database/sqlalchemy/sqlalchemydbconfigmanager.py`

 * *Files identical despite different names*

### Comparing `constellate-0.8.5/constellate/database/sqlalchemy/sqlalchemyengineconfig.py` & `constellate-0.8.7/constellate/database/sqlalchemy/sqlalchemyengineconfig.py`

 * *Files identical despite different names*

### Comparing `constellate-0.8.5/constellate/database/sqlalchemy/sqlalchemypostgresql.py` & `constellate-0.8.7/constellate/database/sqlalchemy/sqlalchemypostgresql.py`

 * *Files identical despite different names*

### Comparing `constellate-0.8.5/constellate/database/sqlalchemy/sqlalchemysqlite3.py` & `constellate-0.8.7/constellate/database/sqlalchemy/sqlalchemysqlite3.py`

 * *Files identical despite different names*

### Comparing `constellate-0.8.5/constellate/database/sqlalchemy/typedecorator/enuminteger.py` & `constellate-0.8.7/constellate/database/sqlalchemy/typedecorator/enuminteger.py`

 * *Files identical despite different names*

### Comparing `constellate-0.8.5/constellate/database/sqlalchemy/typedecorator/enumstring.py` & `constellate-0.8.7/constellate/database/sqlalchemy/typedecorator/enumstring.py`

 * *Files identical despite different names*

### Comparing `constellate-0.8.5/constellate/database/sqlalchemy/typedecorator/enumvalue.py` & `constellate-0.8.7/constellate/database/sqlalchemy/typedecorator/enumvalue.py`

 * *Files identical despite different names*

### Comparing `constellate-0.8.5/constellate/database/sqlalchemy/typedecorator/timestamptz.py` & `constellate-0.8.7/constellate/database/sqlalchemy/typedecorator/timestamptz.py`

 * *Files identical despite different names*

### Comparing `constellate-0.8.5/constellate/database/sqlalchemy/types/composite.py` & `constellate-0.8.7/constellate/database/sqlalchemy/types/composite.py`

 * *Files identical despite different names*

### Comparing `constellate-0.8.5/constellate/database/sqlalchemy/utils/sql_query.py` & `constellate-0.8.7/constellate/database/sqlalchemy/utils/sql_query.py`

 * *Files identical despite different names*

### Comparing `constellate-0.8.5/constellate/database/sqlite3/sqlite3.py` & `constellate-0.8.7/constellate/database/sqlite3/sqlite3.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 from typing import Dict, Tuple, Callable
 from sqlalchemy.pool.base import _ConnectionFairy
 
 
 def register_functions(
-    connection: _ConnectionFairy, functions: Dict[str, Tuple[int, Callable]] = {}
+    connection: _ConnectionFairy, functions: Dict[str, Tuple[int, Callable]] = None
 ) -> None:
     """Register custom functions
 
     :param connection: _ConnectionFairy:
     :param functions: Dict[str:
     :param Tuple[int:
     :param Callable]]:  (Default value = {})
 
     """
+    functions = functions or {}
 
     def _register(
         connection, function_name: str = "my_func", num_params: int = 0, function: Callable = None
     ):
         connection.create_function(function_name, num_params, function)
 
     for function_name, value in functions.items():
@@ -30,15 +31,15 @@
 
 # str: function name
 # int: number of parameters in the function
 # Callable: Function implementation
 Functions = Dict[str, Tuple[int, Callable]]
 
 
-def patch_sqlite3_connect(original_connect, enable: bool = True, functions: Functions = {}):
+def patch_sqlite3_connect(original_connect, enable: bool = True, functions: Functions = None):
     """Monkey patch sqlite.connect before any other library uses it with goal to register custom sql function.
     This monkey matching provides that
     :functions:
     - Key: Function name (like it would be called in a sql script)
     - Value: Tuple(Function Parameters Count, Method implementation)
 
     :enable: True to enable monkey patching
@@ -51,14 +52,15 @@
     sqlite3.connect = ...monkeypatch_sqlite3_connect_enable(_sqlite3.connect)
 
     :param original_connect:
     :param enable: bool:  (Default value = True)
     :param functions: Functions:  (Default value = {})
 
     """
+    functions = functions or {}
 
     def connect_decorator(*args, **kwargs):
         connection = original_connect(*args, **kwargs)
         register_functions(connection=connection, functions=functions)
         return connection
 
     return connect_decorator
```

### Comparing `constellate-0.8.5/constellate/datatype/dictionary/update.py` & `constellate-0.8.7/constellate/datatype/dictionary/update.py`

 * *Files identical despite different names*

### Comparing `constellate-0.8.5/constellate/datetime/timeinterval/timeinterval.py` & `constellate-0.8.7/constellate/datetime/timeinterval/timeinterval.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,19 +14,19 @@
 
 UTCTimestampMilliSec = int
 
 
 def __utctimestamp_millisec_converter(
     in_value: Union[int, int64, pendulum.DateTime, pendulum.Date, pandas.Timestamp],
 ):
-    if isinstance(in_value, int) or isinstance(in_value, int64):
+    if isinstance(in_value, (int, int64)):
         return in_value
-    elif isinstance(in_value, pendulum.DateTime) or isinstance(in_value, pendulum.Date):
+    if isinstance(in_value, (pendulum.DateTime, pendulum.Date)):
         return int(in_value.float_timestamp * 1000)
-    elif isinstance(in_value, pandas.Timestamp):
+    if isinstance(in_value, pandas.Timestamp):
         return pendulum.instance(in_value.to_pydatetime()).int_timestamp * 1000
     raise Exception(f"{in_value} not convertible to {type(UTCTimestampMilliSec)}")
 
 
 class TimeInterval(Interval):
     def __init__(
         self,
@@ -129,32 +129,14 @@
 
     def union(self, other):
         return self | other
 
     def difference(self, other):
         return self - other
 
-    def overlaps(self, other):
-        return super().overlaps(other)
-
-    def __eq__(self, other):
-        return super().__eq__(other)
-
-    def __lt__(self, other):
-        return super().__lt__(other)
-
-    def __gt__(self, other):
-        return super().__gt__(other)
-
-    def __le__(self, other):
-        return super().__le__(other)
-
-    def __ge__(self, other):
-        return super().__ge__(other)
-
     def __str__(self):
         def to_str(i):
             if i.empty:
                 return "Period []"
             return str(TimeInterval(i).to_pendulum_period())
 
         value = ",".join([to_str(i) for i in self])
@@ -190,16 +172,17 @@
 
 
 def time_interval_empty() -> TimeInterval:
     return TimeInterval(empty())
 
 
 def to_time_interval_simplified(
-    intervals: Iterator[Union[Interval, TimeInterval]] = [],
+    intervals: Iterator[Union[Interval, TimeInterval]] = None,
 ) -> Union[Interval, TimeInterval]:
+    intervals = intervals or []
     atomic_intervals = itertools.chain.from_iterable(
         [list(non_atomic_interval) for non_atomic_interval in intervals]
     )
     atomic_intervals = list(atomic_intervals)
     return reduce(operator.__or__, atomic_intervals) if len(atomic_intervals) > 0 else empty()
 
 
@@ -271,16 +254,17 @@
 
 
 def to_sorted_atomic_intervals(intervals: Iterator[Interval] = []) -> List[Interval]:
     return [i for i in to_time_interval_simplified(intervals)]
 
 
 def to_sorted_time_intervals_from_intervals(
-    intervals: Iterator[Interval] = [],
+    intervals: Iterator[Interval] = None,
 ) -> List[TimeInterval]:
+    intervals = intervals or []
     intervals = to_sorted_atomic_intervals(intervals)
     return [TimeInterval(interval) for interval in intervals]
 
 
 def discretize_atomic_interval(i: Interval, incr=1):
     # Turn [0,1] | [2,3] into [0,3]
     # src: https://github.com/AlexandreDecan/portion/issues/24#issuecomment-604456362
@@ -309,37 +293,40 @@
     def discretize(interval: Interval):
         return interval.apply(first_step).apply(second_step)
 
     t = Interval(i)
     return discretize(i) if not discretize(t).empty else i
 
 
-def flatten_intervals(intervals: List[Interval] = []) -> Iterator[Interval]:
+def flatten_intervals(intervals: List[Interval] = None) -> Iterator[Interval]:
+    intervals = intervals or []
     atomic_intervals = itertools.chain.from_iterable(
         [list(non_atomic_interval) for non_atomic_interval in intervals]
     )
     return atomic_intervals
 
 
-def sort_intervals(intervals: List[Interval] = []) -> List[Interval]:
+def sort_intervals(intervals: List[Interval] = None) -> List[Interval]:
     """Sorted from earliest to latest
 
     :param intervals: List[Interval]:  (Default value = [])
 
     """
+    intervals = intervals or []
     sequence = enumerate(range(-sys.maxsize, sys.maxsize, 1), start=0)
 
     def to_tuple(interval: Interval):
         assert interval.atomic
         # sequence value must be unique for each interval, otherwise the intervals
         # are merged together
         return (interval, next(sequence))
 
     mapped = IntervalDict(map(to_tuple, intervals))
     return list(mapped.keys())
 
 
 def to_sorted_atomic_intervals_from_time_intervals(
-    instrument_time_intervals: List[TimeInterval] = [],
+    instrument_time_intervals: List[TimeInterval] = None,
 ) -> List[Interval]:
+    instrument_time_intervals = instrument_time_intervals or []
     intervals = [time_interval for time_interval in instrument_time_intervals]
     return to_sorted_atomic_intervals(intervals)
```

### Comparing `constellate-0.8.5/constellate/debugger/debugger.py` & `constellate-0.8.7/constellate/debugger/debugger.py`

 * *Files 7% similar despite different names*

```diff
@@ -25,15 +25,15 @@
             )
         except BaseException as e:
             if not skip_on_missing_debug_server:
                 raise e
 
 
 def debugger_setup_stage(
-    stage: str = None, enabled_stages: List[str] = [], skip_on_missing_debug_server: bool = False
+    stage: str = None, enabled_stages: List[str] = None, skip_on_missing_debug_server: bool = False
 ):
     """Enable remote debugger if the current stage is one of the enabled stages
 
     :param stage: str:  (Default value = None)
     :param enabled_stages: List[str]:  (Default value = [])
     :param skip_on_missing_debug_server: bool:  (Default value = False)
```

### Comparing `constellate-0.8.5/constellate/debugger/simple.py` & `constellate-0.8.7/constellate/debugger/simple.py`

 * *Files identical despite different names*

### Comparing `constellate-0.8.5/constellate/logger/formatter/formatterfactory.py` & `constellate-0.8.7/constellate/logger/formatter/formatterfactory.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,17 +12,17 @@
         kwargs = {
             "fmt": format,
             "datefmt": date_fmt,
         }
         if sys.version_info >= (3, 10, 0):
             kwargs["defaults"] = defaults
         return logging.Formatter(**kwargs)
-    elif class_name == "colorlog.ColoredFormatter":
+    if class_name == "colorlog.ColoredFormatter":
         kwargs = {
             "fmt": format,
             "datefmt": date_fmt,
         }
         if sys.version_info >= (3, 10, 0):
             kwargs["defaults"] = defaults
         return colorlog.ColoredFormatter(**kwargs)
-    else:
-        raise NotImplementedError(f"class_name={class_name}")
+
+    raise NotImplementedError(f"class_name={class_name}")
```

### Comparing `constellate-0.8.5/constellate/logger/handler/forwarderhandler.py` & `constellate-0.8.7/constellate/logger/handler/forwarderhandler.py`

 * *Files identical despite different names*

### Comparing `constellate-0.8.5/constellate/logger/handler/stringhandler.py` & `constellate-0.8.7/constellate/logger/handler/stringhandler.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 from logging import StreamHandler
 from logging.handlers import MemoryHandler
 
 
 class StringHandler(MemoryHandler):
     def __init__(self, capacity):
         logging.handlers.MemoryHandler.__init__(self, capacity, flushLevel=logging.CRITICAL + 1)
-        self.streamBuffer = StringIO()
-        self.handler = StreamHandler(stream=self.streamBuffer)
+        self.stream_buffer = StringIO()
+        self.handler = StreamHandler(stream=self.stream_buffer)
         self.setTarget(self.handler)
 
     def shouldFlush(self, record):
         return False
 
     def output(self):
         self.flush()
-        return self.streamBuffer.getvalue()
+        return self.stream_buffer.getvalue()
```

### Comparing `constellate-0.8.5/constellate/logger/log.py` & `constellate-0.8.7/constellate/logger/log.py`

 * *Files 0% similar despite different names*

```diff
@@ -290,15 +290,16 @@
         return (
             PurePath(Log._LOGS_DIRECTORY, fileName)
             if Log._LOGS_DIRECTORY is not None
             else PurePath(fileName)
         )
 
     @staticmethod
-    def teardown_loggers(loggers: List[logging.Logger] = []):
+    def teardown_loggers(loggers: List[logging.Logger] = None):
+        loggers = loggers or []
         names = [logger.name for logger in loggers]
         for name in names:
             if name in Log._FQDN_LOGGER_NAMES_EXTERNAL:
                 Log._FQDN_LOGGER_NAMES_EXTERNAL.remove(name)
             Log._LOGGER_NAMES_RETRIEVED.pop(name, None)
 
     @staticmethod
@@ -314,24 +315,26 @@
             Log._LOGGER_NAMES_RETRIEVED[name] = True
         return exist, logging.getLogger(name)
 
     @staticmethod
     def get_hierarchical_logger(
         name: str = None,
         mode: LogMode = LogMode.OPERATE_SERVER,
-        mode_settings: Dict = {},
+        mode_settings: Dict = None,
     ):
         """name_parts: List of a logger's split into parts. Eg: foo.bar.zoo => ['foo','bar','zoo']
 
         :param name: str:  (Default value = None)
         :param mode: LogMode:  (Default value = LogMode.OPERATE_SERVER)
         :param mode_settings: Dict:  (Default value = {})
         :returns: A logger instance
 
         """
+        mode_settings = mode_settings or {}
+
         # Construct Fully Qualified Logger Name
         existed, logger = Log.get_native_logger(name=name)
         if not existed:
             # Client mode logger should not have any handlers set by default, as it will create as many handlers as
             # the original "server" logger had
             if has_flag(mode, LogMode.OPERATE_CLIENT):
                 for handler in list(logger.handlers):
@@ -416,22 +419,22 @@
         :param level:  (Default value = logging.DEBUG)
         :param capacity:  (Default value = sys.maxsize)
         :param console:  (Default value = False)
         :returns: Create or get a free Job logger instance
 
         """
         with Log._JOB_LOGGER_NAMES_LOCK:
-            defaultHandlers = [Log._CONSOLE_HANDLER] if console else []
+            default_handlers = [Log._CONSOLE_HANDLER] if console else []
 
             handler = Log.create_job_handler(capacity=capacity)
             logger = logging.getLogger(name=str(uuid.uuid4()))
             logger.setLevel(level)
 
-            for defaultHandler in [handler] + defaultHandlers:
-                logger.addHandler(defaultHandler)
+            for default_handler in [handler] + default_handlers:
+                logger.addHandler(default_handler)
             return logger
 
     @staticmethod
     def free_job_logger(logger=None):
         """
 
         :param logger:  (Default value = None)
```

### Comparing `constellate-0.8.5/constellate/logger/loggers.py` & `constellate-0.8.7/constellate/logger/loggers.py`

 * *Files identical despite different names*

### Comparing `constellate-0.8.5/constellate/logger/logmode.py` & `constellate-0.8.7/constellate/logger/logmode.py`

 * *Files identical despite different names*

### Comparing `constellate-0.8.5/constellate/logger/simple.py` & `constellate-0.8.7/constellate/logger/simple.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     if mode is not None:
         kwargs.update(mode=mode)
 
     if config_dict is not None and template_dict is not None:
         raise ValueError(
             "config_dict and template_dict cannot be set together. It is one of them only, or none"
         )
-    elif config_dict is not None:
+    if config_dict is not None:
         kwargs.update(config_dict=config_dict)
     elif template_dict is not None:
         kwargs.update(template_config_dict=template_dict)
 
     Log.setup(**kwargs)
```

### Comparing `constellate-0.8.5/constellate/progression/progres.py` & `constellate-0.8.7/constellate/progression/progres.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 class Progress:
     def __init__(self, log: Callable = None, **kwargs):
         self._log = log
         self._kwargs = kwargs
 
     def __call__(self, iterator: Iterable[_T] = None) -> tqdm_asyncio:
-        def _discard_log(msg, *args, **kwargs):
+        def _discard_log(_msg, *_args, **_kwargs):
             pass
 
         _log = self._log or _discard_log
         file = _TextIOWrapperLogger(
             buffer=BytesIO(), log=_log, write_through=True, errors="strict", newline=""
         )
         return tqdm_asyncio(iterator, file=file, **self._kwargs)
```

### Comparing `constellate-0.8.5/constellate/resource/resource.py` & `constellate-0.8.7/constellate/resource/resource.py`

 * *Files 3% similar despite different names*

```diff
@@ -45,17 +45,15 @@
     :param s: root_pk_name: Typically my_module.__package__
     :param root_pkg_name: str:  (Default value = __package__)
     :param directory: str:  (Default value = "data")
     :param ignore_init_file: bool:  (Default value = True)
     :returns: s: List of absolute paths
 
     """
-    paths = [
-        filename for filename in importlib_resources.files(f"{root_pkg_name}.{directory}").iterdir()
-    ]
+    paths = list(importlib_resources.files(f"{root_pkg_name}.{directory}").iterdir())
 
     paths = [
         p
         for p in paths
         if (ignore_init_file and not str(p).endswith("__init__.py"))
         and not str(p).endswith("__pycache__")
     ]
```

### Comparing `constellate-0.8.5/constellate/storage/filesystem/anyfs/path.py` & `constellate-0.8.7/constellate/storage/filesystem/anyfs/path.py`

 * *Files 4% similar despite different names*

```diff
@@ -80,15 +80,15 @@
     :param source: String to escape
     :param escape_string: String to escape the first string with
     :returns: Escaped string
 
     """
     assert isinstance(source, str), "source must be a str"
 
-    escaped_string = list()
+    escaped_string = []
     for c in source:
         escaped_string.append(escape_string)
         escaped_string.append(c)
 
     return "".join(escaped_string)
```

### Comparing `constellate-0.8.5/constellate/storage/filesystem/tmpfs/memory_tempfile.py` & `constellate-0.8.7/constellate/storage/filesystem/tmpfs/memory_tempfile.py`

 * *Files identical despite different names*

### Comparing `constellate-0.8.5/constellate/storage/filesystem/tmpfs/rambacked.py` & `constellate-0.8.7/constellate/storage/filesystem/tmpfs/rambacked.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,29 +9,31 @@
 
 
 def mkd_tmpfs(
     prefix: Optional[str] = None,
     suffix: Optional[str] = None,
     dir: str = None,
     env_tmpfs_dir: str = "TMPFS_DIR",
-    env_tmpfs_dir_fs_types: Optional[List[str]] = ["ext4", "overlay", "tmpfs"],
+    env_tmpfs_dir_fs_types: Optional[List[str]] = None,
 ) -> tempfile.TemporaryDirectory:
     """Create a temporary directory, preferably RAM backed, for speed
 
     (dir) and (env_tmpfs_dir + env_tmpfs_dir_fs_types) are MUTUALLY EXCLUSIVE
 
     :param prefix: Prefix
     :param suffix: Suffix
     :param dir: Directory must exist
     :param env_tmpfs_dir: TMPFS_DIR: Env var name indicating the absolute path to a memory backed tmpfs dir. Directory must exist
     :param env_tmpfs_dir_fs_types:  Filesystem type associated to env_tmpfs_dir.
                                     Note: "overlay" mainly used by k8s container with EmptyDir backed by Memory
     :returns: tempfile.TemporaryDirectory
 
     """
+    env_tmpfs_dir_fs_types = env_tmpfs_dir_fs_types or ["ext4", "overlay", "tmpfs"]
+
     tmpfs = None
     tmpfs_dir = None
     fs_types = None
 
     if env_tmpfs_dir in os.environ:
         tmpfs_dir = os.environ[env_tmpfs_dir]
         fs_types = env_tmpfs_dir_fs_types
```

### Comparing `constellate-0.8.5/constellate/thirdparty/numba/progress/progress.py` & `constellate-0.8.7/constellate/thirdparty/numba/progress/progress.py`

 * *Files identical despite different names*

### Comparing `constellate-0.8.5/constellate/thirdparty/pandas/__init__.py` & `constellate-0.8.7/constellate/thirdparty/pandas/__init__.py`

 * *Files identical despite different names*

### Comparing `constellate-0.8.5/constellate/thirdparty/pandas/accessor/attribute_accessor.py` & `constellate-0.8.7/constellate/thirdparty/pandas/accessor/attribute_accessor.py`

 * *Files identical despite different names*

### Comparing `constellate-0.8.5/constellate/thirdparty/pandas/extra/sanitize/sanitize.py` & `constellate-0.8.7/constellate/thirdparty/pandas/extra/sanitize/sanitize.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from typing import List, Union, Dict
 
 import inspect
 import itertools
 import pandas
 import pandas as pd
 import pandera.dtypes
-from pandera.api.pandas.components import MultiIndex
 from pandas import DataFrame, Series
+from pandera.api.pandas.components import MultiIndex
 from typing import Any
 from typing_extensions import TypeAlias
 from typing import get_origin
 from constellate.thirdparty.pandas.validation.validation import (
     PanderaSchema,
     pandera_schema_from_pydantic_schema,
 )
@@ -53,15 +53,15 @@
 
     #
     # Get index name / dtype pair
     #
     index = pandera_schema.index
     multi_indexed = isinstance(index, MultiIndex)
 
-    indexes = dict()
+    indexes = {}
     has_index = index is not None
     if has_index:
         if multi_indexed:
             indexes = index.columns
         else:
             indexes = _get_index_name_and_dtypes(schema=schema)
 
@@ -129,20 +129,20 @@
         return data
 
     def _apply_dtype(
         data: PandasData = None, col_name: str = None, col_type: Any = None
     ) -> PandasData:
         if isinstance(data, pd.DataFrame):
             return _apply_dtype_dataframe(data=data, col_name=col_name, col_type=col_type)
-        elif isinstance(data, pd.Series):
+        if isinstance(data, pd.Series):
             return _apply_dtype_series(data=data, col_name=col_name, col_type=col_type)
-        elif isinstance(data, pd.Index) and not isinstance(data, pd.MultiIndex):
+        if isinstance(data, pd.Index) and not isinstance(data, pd.MultiIndex):
             return _apply_dtype_series(data=data, col_name=col_name, col_type=col_type)
-        else:
-            raise NotImplementedError()
+
+        raise NotImplementedError()
 
     def _to_numeric(data: PandasData = None, col_name: str = None) -> PandasData:
         if isinstance(data, pd.DataFrame):
             data[col_name] = pandas.to_numeric(data[col_name], errors="coerce", downcast=None)
             return data
         elif isinstance(data, pd.Series):
             data = pandas.to_numeric(data, errors="coerce", downcast=None)
@@ -253,29 +253,30 @@
         data[col_name] = data[col_name].apply(_enum_value)
 
 
 def get_index_columns(schema: PanderaSchema = None) -> List[str]:
     schema2 = pandera_schema_from_pydantic_schema(schema=schema)
     if isinstance(schema2.index, pandera.api.pandas.components.MultiIndex):
         return list(schema2.index.columns.keys())
-    elif isinstance(schema2.index, pandera.api.pandas.components.Index):
+    if isinstance(schema2.index, pandera.api.pandas.components.Index):
         annotations = next(
             iter(filter(lambda m: m[0] == "__annotations__", inspect.getmembers(schema))),
             ("__annotations__", {}),
         )[1]
         index_name = next(
             iter(
                 [k for k, v in annotations.items() if get_origin(v) == pandera.typing.pandas.Index]
             ),
             None,
         )
         return [index_name]
-    elif schema2.index is None:
+    if schema2.index is None:
         # Case: No index defined in the schema
         return []
+
     raise NotImplementedError()
 
 
 def _get_index_name_and_dtypes(schema: PanderaSchema = None) -> Dict[str, Any]:
     schema2 = pandera_schema_from_pydantic_schema(schema=schema)
     if isinstance(schema2.index, pandera.api.pandas.components.MultiIndex):
         raise NotImplementedError("not implemented yet")
```

### Comparing `constellate-0.8.5/constellate/thirdparty/pandas/io/sql/sqlalchemy.py` & `constellate-0.8.7/constellate/thirdparty/pandas/io/sql/sqlalchemy.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 from typing import Union, Callable, Dict, Optional
 
-import pandas as pd
 import regex
+import pandas as pd
 from pandas._typing import DtypeArg
+from pandas import DataFrame
 
 from constellate.database.sqlalchemy.session.multienginesession import MultiEngineSession
 from constellate.database.sqlalchemy.utils.sql_query import resolve_engine_from_query
-from pandas import DataFrame
+
 from sqlalchemy.ext.asyncio import AsyncEngine
 from sqlalchemy.future import Engine, Connection
 from sqlalchemy.sql import Select
 
 
 def _driverless_engine_url(engine: AsyncEngine = None):
     url = str(engine.url)
```

### Comparing `constellate-0.8.5/constellate/thirdparty/pandas/io/sql/sqlalchemy_engine.py` & `constellate-0.8.7/constellate/thirdparty/pandas/io/sql/sqlalchemy_engine.py`

 * *Files identical despite different names*

### Comparing `constellate-0.8.5/constellate/thirdparty/pandas/io/sql/sqlalchemy_execution_option.py` & `constellate-0.8.7/constellate/thirdparty/pandas/io/sql/sqlalchemy_execution_option.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,16 +12,17 @@
     default_value: Dict = None,
 ) -> Optional[Dict]:
     async_connectable = isinstance(connectable, (AsyncSession, AsyncEngine, AsyncConnection))
 
     def get_sync_connectable(connectable):
         if isinstance(connectable, AsyncConnection):
             return connectable.sync_connection
-        elif isinstance(connectable, AsyncEngine):
+        if isinstance(connectable, AsyncEngine):
             return connectable.sync_engine
-        elif isinstance(connectable, AsyncSession):
+        if isinstance(connectable, AsyncSession):
             return connectable.sync_session
+
         raise NotImplementedError()
 
     sync_connectable = connectable if not async_connectable else get_sync_connectable(connectable)
     execution_options = getattr(sync_connectable, "_execution_options", None)
     return execution_options if execution_options is not None else default_value
```

### Comparing `constellate-0.8.5/constellate/thirdparty/pandas/validation/pandera.py` & `constellate-0.8.7/constellate/thirdparty/pandas/validation/pandera.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 import pandera.typing
 import pandera
 import enum
 from typing_extensions import TypeAlias
 
+from pandera.api.base.types import StrictType
+
+
 PDAIndex: TypeAlias = pandera.typing.Index
 PDASeries: TypeAlias = pandera.typing.Series
 PDADataFrame: TypeAlias = pandera.typing.DataFrame
 
 
 def Field(*args, **kwargs):
     isin = kwargs.pop("isin", None)
@@ -16,11 +19,11 @@
     return pandera.Field(*args, **kwargs)
 
 
 PDAField: TypeAlias = Field
 
 
 class BaseConfig(pandera.api.pandas.model_config.BaseConfig):
-    strict = True
-    coerce = True
-    ordered = True
+    strict: StrictType = True
+    coerce: bool = True
+    ordered: bool = True
     unique_column_names = True
```

### Comparing `constellate-0.8.5/constellate/thirdparty/pandas/validation/validation.py` & `constellate-0.8.7/constellate/thirdparty/pandas/validation/validation.py`

 * *Files 24% similar despite different names*

```diff
@@ -4,17 +4,18 @@
 from collections import ChainMap
 from typing import Awaitable
 from typing import Union, Any, Dict, Callable
 
 import pandas
 import pandera
 from decorator import decorator
-from pandera.api.pandas.model import _extract_config_options_and_extras
 from typing_extensions import TypeAlias
 
+from constellate.thirdparty.pandas.validation.pandera import BaseConfig as PandaBaseConfig
+
 PanderaSchema: TypeAlias = Union[pandera.DataFrameSchema, pandera.SeriesSchema]
 PandasType: TypeAlias = Union[pandas.DataFrame, pandas.Series]
 
 LibrarySchema: TypeAlias = Union[PanderaSchema]
 
 AsyncOrSyncCallable: TypeAlias = Union[Callable[..., Any], Callable[..., Awaitable]]
 
@@ -42,30 +43,46 @@
 
 def pandera_schema_from_pydantic_schema(schema: LibrarySchema):
     if isinstance(schema, (pandera.DataFrameSchema, pandera.SeriesSchema)):
         return schema
     return schema.to_schema()
 
 
-def _pydantic_schema_fix_config_inheritance(schema: Any = None):
-    # src: _collect_config_and_extras from pandera.api.pandas.model.SchemaModel
-    config = getattr(schema, pandera.api.pandas.model._CONFIG_KEY, {})
-
-    bases = inspect.getmro(config)[:-1]
-    bases = tuple(base for base in bases if issubclass(base, pandera.api.pandas.model.BaseConfig))
-
-    options = []
-    for index, config in enumerate(bases):
-        model_options, _ = _extract_config_options_and_extras(config)
-        options.append(model_options)
+def _pydantic_schema_fix_config_inheritance(
+    schema: Union[pandera.api.dataframe.model.DataFrameModel] = None,
+):
+    # src: https://github.com/unionai-oss/pandera/blob/63140c9af17314541a21f6629801fe09e90202a3/pandera/api/dataframe/model.py#L384
+
+    def _get_schema_config_class(schema_class):
+        return getattr(schema_class, pandera.api.dataframe.model._CONFIG_KEY, {})
+
+    # Extract Config from pandera.api.*.model.DataFrameModel
+    pandera_model_config_cls, _ = schema._collect_config_and_extras()
+    options, _ = schema._extract_config_options_and_extras(pandera_model_config_cls)
+
+    # Extract Config from hierarchy of schema.Config up to pandera.api.*.model.DataFrameModel.Config
+    # (ie the missing Config not retrieved from  _collect_config_and_extras())
+    schema_classes = [
+        c for c in inspect.getmro(schema) if issubclass(c, pandera.api.pandas.model.DataFrameModel)
+    ][:-1]
+    for schema_class in reversed(schema_classes):
+        schema_config_class = _get_schema_config_class(schema_class)
+        config_classes = [
+            config_class
+            for config_class in inspect.getmro(schema_config_class)
+            if issubclass(config_class, PandaBaseConfig)
+        ]
+        for config_class in reversed(config_classes):
+            options2, _ = schema._extract_config_options_and_extras(config_class)
+            options.update(options2)
 
     return type(
         f"{str(schema.__module__)}.Config",
-        (pandera.api.pandas.model.BaseConfig,),
-        dict(ChainMap(*options)),
+        (pandera_model_config_cls,),
+        dict(ChainMap(options)),
     )
 
 
 def _pandera_checks(
     data: PandasType = None,
     schema: LibrarySchema = None,
     schema_validation_options: Dict[str, Any] = None,
@@ -84,14 +101,16 @@
     }
     if schema is None:
         raise ValueError("Missing schema")
 
     try:
         pandera_schema = schema
         if not isinstance(schema, (pandera.DataFrameSchema, pandera.SeriesSchema)):
+            # Convert Pandera's DataFrame Model (ie Pandera's DataFrame Model using pydantic like notation)
+            # into a Pandera native's DataFrame Schema
             schema.__config__ = _pydantic_schema_fix_config_inheritance(schema=schema)
             pandera_schema = pandera_schema_from_pydantic_schema(schema=schema)
 
         # For list of checks carried out:
         # https://pandera.readthedocs.io/en/stable/lazy_validation.html
         return pandera_schema.validate(data, **schema_validation_options)
     except pandera.errors.SchemaError as e:
```

### Comparing `constellate-0.8.5/constellate/thirdparty/pandera/inspector.py` & `constellate-0.8.7/constellate/thirdparty/pandera/inspector.py`

 * *Files 26% similar despite different names*

```diff
@@ -6,26 +6,30 @@
 
 def schema_columns(schema: SchemaModel = None) -> List[str]:
     return [k for k, v in dict(schema.__dict__) if isinstance(v, Field)]
 
 
 def dataframe_from_schema(
     schema: SchemaModel = None,
-    reset_index_kwargs: Dict = {"inplace": True},
-    rename_kwargs: Dict = {},
-    extra_columns: Dict = {},
+    reset_index_kwargs: Dict = None,
+    rename_kwargs: Dict = None,
+    extra_columns: Dict = None,
 ) -> pd.DataFrame:
     """Create an empty dataframe based on a schema
 
     :param schema: SchemaModel:  (Default value = None)
     :param reset_index_kwargs: Dict:  (Default value = {"inplace": True})
     :param rename_kwargs: Dict:  (Default value = {})
     :param extra_columns: Dict:  (Default value = {})
 
     """
+    reset_index_kwargs = reset_index_kwargs or {"inplace": True}
+    rename_kwargs = rename_kwargs or {}
+    extra_columns = extra_columns or {}
+
     # Requires: hypothesis package
     df = schema.to_schema().example(size=0)
 
     # Move / Rename / Add columns
     if len(reset_index_kwargs):
         df.reset_index(**reset_index_kwargs)
     if len(rename_kwargs) > 0:
@@ -34,22 +38,23 @@
         df.insert(0, col_name, [], allow_duplicates=False)
         df = df.astype({col_name: dtype}, copy=False, errors="ignore")
     return df
 
 
 def series_from_schema(
     schema: SchemaModel = None,
-    rename_kwargs: Dict = {},
+    rename_kwargs: Dict = None,
 ) -> pd.Series:
     """Create an empty series based on a schema
 
     :param schema: SchemaModel:  (Default value = None)
     :param rename_kwargs: Dict:  (Default value = {})
 
     """
+    rename_kwargs = rename_kwargs or {}
     # Requires: hypothesis package
     df = schema.to_schema().example(size=0)
 
     if len(rename_kwargs) > 0:
         df.rename(**rename_kwargs)
 
     return df.squeeze(axis="columns")
```

### Comparing `constellate-0.8.5/constellate.egg-info/PKG-INFO` & `constellate-0.8.7/constellate.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: constellate
-Version: 0.8.5
+Version: 0.8.7
 Summary: A bunch of utilities aggregated over time
 Author-email: David Andreoletti <none@provided.yet>
 Project-URL: repository, https://github.com/davidandreoletti/constellate
 Keywords: constellate
 Classifier: License :: Other/Proprietary License
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -17,57 +17,64 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: <3.13,>=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
-Requires-Dist: Pebble>=4.6.3
 Requires-Dist: decorator>=5.1.0
 Requires-Dist: aioitertools>=0.8.0
 Requires-Dist: psutil>=5.7.0
 Requires-Dist: pendulum>=2.1.2
 Requires-Dist: requests>=2.25.0
 Requires-Dist: memory-tempfile>=2.2.3
-Requires-Dist: narration>=0.2.16
 Requires-Dist: bidict>=0.21.4
 Requires-Dist: attrs>=20.3.0
 Requires-Dist: portion>=2.2.0
 Requires-Dist: jsonmerge>=1.8.0
 Requires-Dist: jsonschema>=4.7.2
 Requires-Dist: Deprecated>=1.2.12
 Requires-Dist: importlib-resources>=5.1.4
 Requires-Dist: typing-extensions>=4.3.0
 Requires-Dist: tqdm>=4.62.3
 Requires-Dist: regex>=2021.11.10
 Requires-Dist: blake3>=0.3.1
 Requires-Dist: sqlparse>=0.4.2
 Requires-Dist: stackeddag>=0.3.3
-Provides-Extra: cli-args
-Requires-Dist: argunparse>=0.1.3; extra == "cli-args"
+Provides-Extra: cliargs
+Requires-Dist: argunparse>=0.1.3; extra == "cliargs"
 Provides-Extra: sqlalchemy
 Requires-Dist: SQLAlchemy>=2.0.11; extra == "sqlalchemy"
 Requires-Dist: sqlalchemy-utils>=0.37.9; extra == "sqlalchemy"
 Requires-Dist: sqlalchemy-json>=0.4.0; extra == "sqlalchemy"
 Requires-Dist: sqlalchemy_mixins>=2.0; extra == "sqlalchemy"
 Requires-Dist: aiosqlite>=0.17.0; extra == "sqlalchemy"
 Requires-Dist: asyncpg>=0.23.0; extra == "sqlalchemy"
 Requires-Dist: networkx>=2.8.5; extra == "sqlalchemy"
 Provides-Extra: pandas
-Requires-Dist: pandas>=1.3.4; extra == "pandas"
+Requires-Dist: pandas>=2.0.0; extra == "pandas"
 Requires-Dist: pandas-log>=0.1.7; extra == "pandas"
-Requires-Dist: pandera!=0.13.4,>=0.14.5; extra == "pandas"
+Requires-Dist: pandera!=0.13.4,>=0.19.0; extra == "pandas"
 Requires-Dist: hypothesis>=6.54.4; extra == "pandas"
 Provides-Extra: numpy
 Requires-Dist: numpy>=1.21.4; extra == "numpy"
 Provides-Extra: numba
 Requires-Dist: numba-progress>=0.0.3; extra == "numba"
 Provides-Extra: sparql
 Requires-Dist: rdflib>=6.3.0; extra == "sparql"
 Requires-Dist: SPARQL-Burger>=1.0.2; extra == "sparql"
+Provides-Extra: zstd
+Requires-Dist: pyzstd>=0.15.10; extra == "zstd"
+Provides-Extra: logging
+Requires-Dist: narration>=0.2.17; extra == "logging"
+Requires-Dist: colorlog>=6.8.2; extra == "logging"
+Provides-Extra: concurrencypebble
+Requires-Dist: Pebble>=4.6.3; extra == "concurrencypebble"
+Provides-Extra: all
+Requires-Dist: constellate[cliargs,concurrencypebble,logging,numba,numpy,pandas,sparql,sqlalchemy,zstd]; extra == "all"
 
 .. image:: https://img.shields.io/pypi/v/constellate.svg
 .. image:: https://img.shields.io/pypi/pyversions/constellate.svg
 .. image:: https://img.shields.io/pypi/status/constellate.svg
 .. image:: https://img.shields.io/pypi/l/constellate.svg
 
 constellate
```

### Comparing `constellate-0.8.5/constellate.egg-info/SOURCES.txt` & `constellate-0.8.7/constellate.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,18 @@
 constellate.egg-info/top_level.txt
 constellate/cli/__init__.py
 constellate/cli/argument/__init__.py
 constellate/cli/argument/unparse.py
 constellate/compression/__init__.py
 constellate/compression/zip/__init__.py
 constellate/compression/zip/zip.py
+constellate/compression/zstd/__init__.py
+constellate/compression/zstd/common.py
+constellate/compression/zstd/pyzstd.py
+constellate/compression/zstd/zstandard.py
 constellate/concurrency/__init__.py
 constellate/concurrency/asyncio/__init__.py
 constellate/concurrency/asyncio/tasks.py
 constellate/concurrency/pebble/__init__.py
 constellate/concurrency/pebble/pool_cleanup.py
 constellate/concurrency/simple/__init__.py
 constellate/concurrency/simple/simple.py
```

### Comparing `constellate-0.8.5/pyproject.toml` & `constellate-0.8.7/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -23,22 +23,20 @@
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
 ]
 
 dependencies = [
-    "Pebble>=4.6.3",
     "decorator>=5.1.0",
     "aioitertools>=0.8.0",
     "psutil>=5.7.0",
     "pendulum>=2.1.2",
     "requests>=2.25.0",
     "memory-tempfile>=2.2.3",
-    "narration>=0.2.16",
     "bidict>=0.21.4",
     "attrs>=20.3.0",
     "portion>=2.2.0",
     "jsonmerge>=1.8.0",
     "jsonschema>=4.7.2",
     "Deprecated>=1.2.12",
     "importlib-resources>=5.1.4",
@@ -49,15 +47,15 @@
     "sqlparse>=0.4.2",
     "stackeddag>=0.3.3",
 ]
 
 [project.optional-dependencies]
 # Required by
 # - constellate.cli.arg package
-cli_args = [
+cliargs = [
     "argunparse>=0.1.3",
 ]
 # Required by
 # - constellate.database.migration package
 # - constellate.database.sqlalchemy package
 sqlalchemy = [
     "SQLAlchemy>=2.0.11",
@@ -68,25 +66,37 @@
     "asyncpg>=0.23.0",
     "networkx>=2.8.5",
 ]
 # Required by
 # - constellate.thirdparty.pandas package
 # - constellate.datetime.timeinterval package
 pandas = [
-    "pandas>=1.3.4",
+    "pandas>=2.0.0",
     "pandas-log>=0.1.7",
-    "pandera>=0.14.5,!=0.13.4",
+    "pandera>=0.19.0,!=0.13.4",
     "hypothesis>=6.54.4",
 ]
 # - constellate.datetime.timeinterval package
 numpy = ["numpy>=1.21.4"]
 # - constellate.thirdparty.numba package
 "numba"= ["numba-progress>=0.0.3"]
 # - constellate.database.sparql package
 sparql = ["rdflib>=6.3.0", "SPARQL-Burger>=1.0.2"]
+# - constellate.compression.zstd package
+zstd = ["pyzstd>=0.15.10"]
+# - constellate.logger package
+logging = [
+     "narration>=0.2.17",
+     "colorlog>=6.8.2"
+ ]
+# - constellate.concurrency.pebble
+concurrencypebble = [
+     "Pebble>=4.6.3"
+]
+all = ["constellate[cliargs,sqlalchemy,pandas,numpy,numba,sparql,zstd,logging,concurrencypebble]"]
 
 [project.urls]
 repository = "https://github.com/davidandreoletti/constellate"
 
 [tool.setuptools]
 include-package-data = true
```

### Comparing `constellate-0.8.5/tests/test_cli_argument.py` & `constellate-0.8.7/tests/test_cli_argument.py`

 * *Files identical despite different names*

### Comparing `constellate-0.8.5/tests/test_concurrency.py` & `constellate-0.8.7/tests/test_concurrency.py`

 * *Files 8% similar despite different names*

```diff
@@ -27,9 +27,7 @@
 
 
 @pytest.mark.asyncio
 @pytest.mark.parametrize("pool", [None, pebble.ProcessPool()])
 async def test_concurrency_simple_process(pool) -> None:
     compute = functools.partial(process, __compute_via_process, pool=pool)
     expect(await compute(b=1, c=1)).to_be(2)
-    # This does not wark
-    # expect(await _compute2(1, 1, b=1, c=1)).to_be(4)
```

### Comparing `constellate-0.8.5/tests/test_cryptography.py` & `constellate-0.8.7/tests/test_cryptography.py`

 * *Files identical despite different names*

### Comparing `constellate-0.8.5/tests/test_enum.py` & `constellate-0.8.7/tests/test_enum.py`

 * *Files identical despite different names*

### Comparing `constellate-0.8.5/tests/test_logger.py` & `constellate-0.8.7/tests/test_logger.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,15 +65,15 @@
 
 
 def test_logger_standalone_default(root_logger_name: str) -> None:
     with mkd_tmpfs(prefix="test_logger_default") as tmp_dir:
         setup_any_process_loggers(root_logger_name=root_logger_name, log_dir_path=str(tmp_dir))
         loggers = setup_standalone_process_loggers()
 
-        for logger, name in [
+        for _logger, name in [
             (loggers.app, "app"),
             (loggers.network, "network"),
             (loggers.database, "database"),
             (loggers.media, "media"),
         ]:
             stream = StringIO()
             loggers.app.addHandler(StreamHandler(stream=stream))
@@ -116,15 +116,15 @@
         vectors = {
             1: {"logger": loggers.app.foo.bar, "name": "app.foo.bar", "stream": StringIO()},
             2: {"logger": loggers.app.foo, "name": "app.foo", "stream": StringIO()},
             3: {"logger": loggers.app, "name": "app", "stream": StringIO()},
         }
 
         # Setup handler per logger
-        for index, obj in vectors.items():
+        for _index, obj in vectors.items():
             stream = obj.get("stream", None)
             logger = obj.get("logger", None)
             logger.addHandler(StreamHandler(stream=stream))
 
         propagated_messages = []
         for index, obj in vectors.items():
             stream = obj.get("stream", None)
@@ -237,15 +237,15 @@
 
 
 def test_logger_print_exception_str(root_logger_name: str) -> None:
     with mkd_tmpfs(prefix="test_logger_default") as tmp_dir:
         setup_any_process_loggers(root_logger_name=root_logger_name, log_dir_path=str(tmp_dir))
         loggers = setup_standalone_process_loggers()
 
-        for logger, name in [
+        for _logger, name in [
             (loggers.app, "app"),
         ]:
             stream = StringIO()
             loggers.app.addHandler(StreamHandler(stream=stream))
 
             try:
                 raise TestExceptionString(tag="found")
@@ -264,15 +264,15 @@
 
 
 def test_logger_print_no_exception_str(root_logger_name: str) -> None:
     with mkd_tmpfs(prefix="test_logger_default") as tmp_dir:
         setup_any_process_loggers(root_logger_name=root_logger_name, log_dir_path=str(tmp_dir))
         loggers = setup_standalone_process_loggers()
 
-        for logger, name in [
+        for _logger, name in [
             (loggers.app, "app"),
         ]:
             stream = StringIO()
             loggers.app.addHandler(StreamHandler(stream=stream))
 
             msg = f"{name}-record"
             loggers.app.info(msg)
```

### Comparing `constellate-0.8.5/tests/test_migration.py` & `constellate-0.8.7/tests/test_migration.py`

 * *Files identical despite different names*

### Comparing `constellate-0.8.5/tests/test_pandas.py` & `constellate-0.8.7/tests/test_pandas.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     DataValidationError,
 )
 
 
 @pytest.mark.parametrize("asynced", [False, True])
 @pytest.mark.asyncio
 async def test_pandas_data_coerce_and_validate(asynced) -> None:
-    class _PandaDataChecksDFSchema(pa.SchemaModel):
+    class _PandaDataChecksDFSchema(pa.DataFrameModel):
         name: PDASeries[pandas.StringDtype] = PDAField()
         age: PDASeries[pandas.Int64Dtype] = PDAField()
         country: PDASeries[pandas.StringDtype] = PDAField()
 
         class Config(BaseConfig):
             pass
 
@@ -107,47 +107,47 @@
 
 @pytest.mark.parametrize("typed", [pandas.DataFrame, pandas.Series])
 def test_pandas_fill_missing_from_schema(typed) -> None:
     if typed == pandas.DataFrame:
         #
         # Fill column name
         #
-        class _FillMissingColumnFromSchemaDFSchema(pa.SchemaModel):
+        class _FillMissingColumnFromSchemaDFSchema(pa.DataFrameModel):
             time: PDAIndex[pandas.StringDtype] = PDAField()
             age: PDASeries[pandas.Int64Dtype] = PDAField()
             name: PDASeries[pandas.StringDtype] = PDAField()
 
         df = pandas.DataFrame()
         df = fill_missing_from_schema(schema=_FillMissingColumnFromSchemaDFSchema, data=df)
         expect(isinstance(df.index, pandas.Index)).to_equal(True)
         expect(type(df.index.dtype)).to_equal(pandas.StringDtype)
         expect(type(df.age.dtype)).to_equal(pandas.Int64Dtype)
         expect(type(df.name.dtype)).to_equal(pandas.StringDtype)
 
-        class _FillMissingColumnFromSchemaDFSchemaMultiIndex(pa.SchemaModel):
+        class _FillMissingColumnFromSchemaDFSchemaMultiIndex(pa.DataFrameModel):
             time: PDAIndex[pandas.StringDtype] = PDAField()
             uid: PDAIndex[pandas.Int64Dtype] = PDAField()
             age: PDASeries[pandas.Int64Dtype] = PDAField()
             name: PDASeries[pandas.StringDtype] = PDAField()
 
         #
         # Fill column dtype
         #
-        class _FillNanFromSchemaDFSchemaNoIndex(pa.SchemaModel):
+        class _FillNanFromSchemaDFSchemaNoIndex(pa.DataFrameModel):
             age: PDASeries[pandas.Int64Dtype] = PDAField()
             name: PDASeries[pandas.StringDtype] = PDAField()
 
         df = pandas.DataFrame(data={"age": [None, None], "name": [None, None]})
         df = fill_missing_from_schema(schema=_FillNanFromSchemaDFSchemaNoIndex, data=df)
         expect(type(df.age.dtype)).to_equal(pandas.Int64Dtype)
         expect(type(df.name.dtype)).to_equal(pandas.StringDtype)
         expect(type(df["age"][0])).to_equal(type(pandas.NA))
         expect(type(df["name"][0])).to_equal(type(pandas.NA))
 
-        class _FillNanFromSchemaDFSchemaMonoIndex(pa.SchemaModel):
+        class _FillNanFromSchemaDFSchemaMonoIndex(pa.DataFrameModel):
             time: PDAIndex[pandas.StringDtype] = PDAField()
             age: PDASeries[pandas.Int64Dtype] = PDAField()
             name: PDASeries[pandas.StringDtype] = PDAField()
 
         df = pandas.DataFrame(
             index=["20/10/2022", "21/10/2022"], data={"age": [None, None], "name": [None, None]}
         )
@@ -156,15 +156,15 @@
         expect(type(df.index.dtype)).to_equal(pandas.StringDtype)
         expect(type(df.age.dtype)).to_equal(pandas.Int64Dtype)
         expect(type(df.name.dtype)).to_equal(pandas.StringDtype)
         expect(df.index[0]).to_equal("20/10/2022")
         expect(type(df["age"][0])).to_equal(type(pandas.NA))
         expect(type(df["name"][0])).to_equal(type(pandas.NA))
 
-        class _FillNanFromSchemaDFSchemaMultiIndex(pa.SchemaModel):
+        class _FillNanFromSchemaDFSchemaMultiIndex(pa.DataFrameModel):
             time: PDAIndex[pandas.StringDtype] = PDAField()
             uid: PDAIndex[pandas.Int64Dtype] = PDAField()
             age: PDASeries[pandas.Int64Dtype] = PDAField()
             name: PDASeries[pandas.StringDtype] = PDAField()
 
         multi_index = pandas.MultiIndex.from_tuples(
             [("20/10/2022", 0), ("21/10/2022", 1)], names=["time", "uid"]
@@ -176,34 +176,34 @@
         expect(type(df.name.dtype)).to_equal(pandas.StringDtype)
         expect(df.index[0]).to_equal(("20/10/2022", 0))
         expect(type(df["age"][0])).to_equal(type(pandas.NA))
         expect(type(df["name"][0])).to_equal(type(pandas.NA))
 
     elif typed == pandas.Series:
 
-        class _FillNanFromSchemaSRSchemaNoIndex(pa.SchemaModel):
+        class _FillNanFromSchemaSRSchemaNoIndex(pa.DataFrameModel):
             age: PDASeries[pandas.Int64Dtype] = PDAField()
 
         sr = pandas.Series(data={0: None})
         sr = fill_missing_from_schema(schema=_FillNanFromSchemaSRSchemaNoIndex, data=sr)
         expect(type(sr[0])).to_equal(type(pandas.NA))
 
-        class _FillNanFromSchemaSRSchemaMonoIndex(pa.SchemaModel):
+        class _FillNanFromSchemaSRSchemaMonoIndex(pa.DataFrameModel):
             time: PDAIndex[pandas.StringDtype] = PDAField()
             age: PDASeries[pandas.Int64Dtype] = PDAField()
 
         sr = pandas.Series(
             data={"20/10/2022": None, "21/10/2022": 20}, index=["20/10/2022", "21/10/2022"]
         )
         sr = fill_missing_from_schema(schema=_FillNanFromSchemaSRSchemaMonoIndex, data=sr)
         expect(isinstance(sr.index, pandas.Index)).to_equal(True)
         expect(type(sr.index.dtype)).to_equal(pandas.StringDtype)
         expect(type(sr["20/10/2022"])).to_equal(type(pandas.NA))
 
-        class _FillNanFromSchemaSRSchemaMultiIndex(pa.SchemaModel):
+        class _FillNanFromSchemaSRSchemaMultiIndex(pa.DataFrameModel):
             time: PDAIndex[pandas.StringDtype] = PDAField()
             uid: PDAIndex[pandas.Int64Dtype] = PDAField()
             age: PDASeries[pandas.Int64Dtype] = PDAField()
 
         multi_index = pandas.MultiIndex.from_tuples(
             [("20/10/2022", 0), ("21/10/2022", 1)], names=["time", "uid"]
         )
```

### Comparing `constellate-0.8.5/tests/test_pandera.py` & `constellate-0.8.7/tests/test_pandera.py`

 * *Files identical despite different names*

### Comparing `constellate-0.8.5/tests/test_progression.py` & `constellate-0.8.7/tests/test_progression.py`

 * *Files identical despite different names*

### Comparing `constellate-0.8.5/tests/test_sparql.py` & `constellate-0.8.7/tests/test_sparql.py`

 * *Files identical despite different names*

### Comparing `constellate-0.8.5/tests/test_sqlalchemy.py` & `constellate-0.8.7/tests/test_sqlalchemy.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import List, Iterable, AsyncGenerator
 
 import pytest
+from pyexpect import expect
 import sqlalchemy
 from sqlalchemy.ext.asyncio import AsyncSession
 from sqlalchemy.exc import NoResultFound
-from pyexpect import expect
 from sqlalchemy import Column, Integer, String, select, func
 from sqlalchemy.orm import declarative_base
 
 from constellate.database.common.databasetype import DatabaseType
 from constellate.database.sqlalchemy.execution.execute import (
     execute_scalars_one_or_none,
     execute_scalars_one,
```

### Comparing `constellate-0.8.5/tests/test_storage_filesystem_tmpfs_rambacked.py` & `constellate-0.8.7/tests/test_storage_filesystem_tmpfs_rambacked.py`

 * *Files identical despite different names*

