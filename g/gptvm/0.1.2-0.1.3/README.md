# Comparing `tmp/gptvm-0.1.2-py3-none-any.whl.zip` & `tmp/gptvm-0.1.3-py37-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,72 +1,78 @@
-Zip file size: 60230 bytes, number of entries: 70
--rw-r--r--  2.0 unx       40 b- defN 24-May-06 03:13 gptvm/__init__.py
--rw-r--r--  2.0 unx      127 b- defN 24-May-06 03:13 gptvm/__main__.py
--rw-r--r--  2.0 unx      406 b- defN 24-May-07 07:49 gptvm/api.py
--rw-r--r--  2.0 unx     7637 b- defN 24-May-08 03:28 gptvm/app.py
--rw-r--r--  2.0 unx     1347 b- defN 24-May-06 03:24 gptvm/cls.py
--rw-r--r--  2.0 unx      814 b- defN 24-May-07 16:32 gptvm/config.py
--rw-r--r--  2.0 unx        0 b- defN 24-May-06 03:13 gptvm/function.py
--rw-r--r--  2.0 unx      303 b- defN 24-May-06 03:24 gptvm/log.py
--rw-r--r--  2.0 unx     1227 b- defN 24-May-06 03:13 gptvm/vmcfg.py
--rw-r--r--  2.0 unx       26 b- defN 24-May-06 03:13 gptvm/cli/__init__.py
--rw-r--r--  2.0 unx     4990 b- defN 24-May-07 07:49 gptvm/cli/app.py
--rw-r--r--  2.0 unx      837 b- defN 24-May-07 07:49 gptvm/cli/auth.py
--rw-r--r--  2.0 unx     1526 b- defN 24-May-08 03:27 gptvm/cli/cli.py
--rw-r--r--  2.0 unx     1124 b- defN 24-May-07 07:49 gptvm/cli/env.py
--rw-r--r--  2.0 unx     3217 b- defN 24-May-07 07:49 gptvm/cli/import_vm.py
--rw-r--r--  2.0 unx     1278 b- defN 24-May-08 03:27 gptvm/cli/run.py
--rw-r--r--  2.0 unx     5358 b- defN 24-May-08 17:38 gptvm/cli/runtime.py
--rw-r--r--  2.0 unx     2043 b- defN 24-May-06 03:24 gptvm/cli/serve.py
--rw-r--r--  2.0 unx        0 b- defN 24-May-06 03:13 gptvm/proto/__init__.py
--rw-r--r--  2.0 unx     1610 b- defN 24-May-07 07:57 gptvm/proto/account_pb2.py
--rw-r--r--  2.0 unx     1134 b- defN 24-May-07 07:57 gptvm/proto/account_pb2.pyi
--rw-r--r--  2.0 unx     1136 b- defN 24-May-07 07:57 gptvm/proto/account_pb2_grpc.py
--rw-r--r--  2.0 unx     5469 b- defN 24-May-07 07:57 gptvm/proto/api_pb2.py
--rw-r--r--  2.0 unx      629 b- defN 24-May-07 07:57 gptvm/proto/api_pb2.pyi
--rw-r--r--  2.0 unx    63510 b- defN 24-May-07 07:57 gptvm/proto/api_pb2_grpc.py
--rw-r--r--  2.0 unx    12974 b- defN 24-May-07 07:57 gptvm/proto/app_pb2.py
--rw-r--r--  2.0 unx    18085 b- defN 24-May-07 07:57 gptvm/proto/app_pb2.pyi
--rw-r--r--  2.0 unx     1132 b- defN 24-May-07 07:57 gptvm/proto/app_pb2_grpc.py
--rw-r--r--  2.0 unx     1444 b- defN 24-May-07 07:57 gptvm/proto/app_version_pb2.py
--rw-r--r--  2.0 unx     1002 b- defN 24-May-07 07:57 gptvm/proto/app_version_pb2.pyi
--rw-r--r--  2.0 unx     1140 b- defN 24-May-07 07:57 gptvm/proto/app_version_pb2_grpc.py
--rw-r--r--  2.0 unx     2293 b- defN 24-May-07 07:57 gptvm/proto/common_pb2.py
--rw-r--r--  2.0 unx     2256 b- defN 24-May-07 07:57 gptvm/proto/common_pb2.pyi
--rw-r--r--  2.0 unx     1135 b- defN 24-May-07 07:57 gptvm/proto/common_pb2_grpc.py
--rw-r--r--  2.0 unx     1238 b- defN 24-May-07 07:57 gptvm/proto/device_pb2.py
--rw-r--r--  2.0 unx      626 b- defN 24-May-07 07:57 gptvm/proto/device_pb2.pyi
--rw-r--r--  2.0 unx     1135 b- defN 24-May-07 07:57 gptvm/proto/device_pb2_grpc.py
--rw-r--r--  2.0 unx     3389 b- defN 24-May-07 07:57 gptvm/proto/env_pb2.py
--rw-r--r--  2.0 unx     4204 b- defN 24-May-07 07:57 gptvm/proto/env_pb2.pyi
--rw-r--r--  2.0 unx     1132 b- defN 24-May-07 07:57 gptvm/proto/env_pb2_grpc.py
--rw-r--r--  2.0 unx     1568 b- defN 24-May-07 07:57 gptvm/proto/hello_pb2.py
--rw-r--r--  2.0 unx      856 b- defN 24-May-07 07:57 gptvm/proto/hello_pb2.pyi
--rw-r--r--  2.0 unx     3647 b- defN 24-May-07 07:57 gptvm/proto/hello_pb2_grpc.py
--rw-r--r--  2.0 unx     2449 b- defN 24-May-07 07:57 gptvm/proto/image_pb2.py
--rw-r--r--  2.0 unx     2591 b- defN 24-May-07 07:57 gptvm/proto/image_pb2.pyi
--rw-r--r--  2.0 unx     1134 b- defN 24-May-07 07:57 gptvm/proto/image_pb2_grpc.py
--rw-r--r--  2.0 unx     3259 b- defN 24-May-07 07:57 gptvm/proto/storage_pb2.py
--rw-r--r--  2.0 unx     4278 b- defN 24-May-07 07:57 gptvm/proto/storage_pb2.pyi
--rw-r--r--  2.0 unx     1136 b- defN 24-May-07 07:57 gptvm/proto/storage_pb2_grpc.py
--rw-r--r--  2.0 unx     4949 b- defN 24-May-07 07:57 gptvm/proto/task_pb2.py
--rw-r--r--  2.0 unx     6555 b- defN 24-May-07 07:57 gptvm/proto/task_pb2.pyi
--rw-r--r--  2.0 unx     1133 b- defN 24-May-07 07:57 gptvm/proto/task_pb2_grpc.py
--rw-r--r--  2.0 unx     3797 b- defN 24-May-07 07:57 gptvm/proto/user_pb2.py
--rw-r--r--  2.0 unx     4148 b- defN 24-May-07 07:57 gptvm/proto/user_pb2.pyi
--rw-r--r--  2.0 unx     1133 b- defN 24-May-07 07:57 gptvm/proto/user_pb2_grpc.py
--rw-r--r--  2.0 unx     2004 b- defN 24-May-07 07:57 gptvm/proto/workgroup_pb2.py
--rw-r--r--  2.0 unx     1964 b- defN 24-May-07 07:57 gptvm/proto/workgroup_pb2.pyi
--rw-r--r--  2.0 unx     1138 b- defN 24-May-07 07:57 gptvm/proto/workgroup_pb2_grpc.py
--rw-r--r--  2.0 unx     2752 b- defN 24-May-07 07:57 gptvm/proto/workspace_pb2.py
--rw-r--r--  2.0 unx     3037 b- defN 24-May-07 07:57 gptvm/proto/workspace_pb2.pyi
--rw-r--r--  2.0 unx     1138 b- defN 24-May-07 07:57 gptvm/proto/workspace_pb2_grpc.py
--rw-r--r--  2.0 unx       62 b- defN 24-May-06 03:24 gptvm/runner/__init__.py
--rw-r--r--  2.0 unx      678 b- defN 24-May-06 03:24 gptvm/runner/base.py
--rw-r--r--  2.0 unx      617 b- defN 24-May-06 03:24 gptvm/runner/local.py
--rw-r--r--  2.0 unx     8790 b- defN 24-May-08 23:49 gptvm/runner/remote.py
--rw-r--r--  2.0 unx      549 b- defN 24-May-09 02:11 gptvm-0.1.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-09 02:11 gptvm-0.1.2.dist-info/WHEEL
--rw-r--r--  2.0 unx       46 b- defN 24-May-09 02:11 gptvm-0.1.2.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        6 b- defN 24-May-09 02:11 gptvm-0.1.2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     5595 b- defN 24-May-09 02:11 gptvm-0.1.2.dist-info/RECORD
-70 files, 230074 bytes uncompressed, 51516 bytes compressed:  77.6%
+Zip file size: 70546 bytes, number of entries: 76
+drwxrwxr-x  2.0 unx        0 b- stor 24-May-10 14:47 gptvm/
+drwxrwxr-x  2.0 unx        0 b- stor 24-May-10 14:47 gptvm-0.1.3.dist-info/
+-rw-rw-r--  2.0 unx        6 b- defN 24-May-10 06:47 gptvm-0.1.3.dist-info/top_level.txt
+-rw-------  2.0 unx       93 b- defN 24-May-10 14:47 gptvm-0.1.3.dist-info/WHEEL
+-rw-rw-r--  2.0 unx      549 b- defN 24-May-10 06:47 gptvm-0.1.3.dist-info/METADATA
+-rw-rw-r--  2.0 unx       46 b- defN 24-May-10 06:47 gptvm-0.1.3.dist-info/entry_points.txt
+-rw-------  2.0 unx     5720 b- defN 24-May-10 14:47 gptvm-0.1.3.dist-info/RECORD
+drwxrwxr-x  2.0 unx        0 b- stor 24-May-10 14:47 gptvm/cli/
+drwxrwxr-x  2.0 unx        0 b- stor 24-May-10 14:47 gptvm/proto/
+drwxrwxr-x  2.0 unx        0 b- stor 24-May-10 14:47 gptvm/runner/
+-rw-rw-r--  2.0 unx      753 b- defN 24-May-10 14:47 gptvm/api.pyc
+-rw-rw-r--  2.0 unx     1307 b- defN 24-May-10 14:47 gptvm/config.pyc
+-rw-rw-r--  2.0 unx     1473 b- defN 24-May-10 14:47 gptvm/cls.pyc
+-rw-rw-r--  2.0 unx      506 b- defN 24-May-10 14:47 gptvm/log.pyc
+-rw-rw-r--  2.0 unx     1651 b- defN 24-May-10 14:47 gptvm/vmcfg.pyc
+-rw-rw-r--  2.0 unx      300 b- defN 24-May-10 14:47 gptvm/__main__.pyc
+-rw-rw-r--  2.0 unx     7812 b- defN 24-May-10 14:47 gptvm/app.pyc
+-rw-rw-r--  2.0 unx      155 b- defN 24-May-10 14:47 gptvm/__init__.pyc
+-rw-rw-r--  2.0 unx      118 b- defN 24-May-10 14:47 gptvm/function.pyc
+-rw-rw-r--  2.0 unx      236 b- defN 24-May-10 14:47 gptvm/proto/workgroup_pb2_grpc.pyc
+-rw-rw-r--  2.0 unx     3985 b- defN 24-May-10 14:47 gptvm/proto/api_pb2.pyc
+-rw-rw-r--  2.0 unx     6555 b- defN 24-May-07 07:13 gptvm/proto/task_pb2.pyi
+-rw-rw-r--  2.0 unx     1170 b- defN 24-May-10 14:47 gptvm/proto/hello_pb2.pyc
+-rw-rw-r--  2.0 unx      856 b- defN 24-May-07 07:13 gptvm/proto/hello_pb2.pyi
+-rw-rw-r--  2.0 unx      236 b- defN 24-May-10 14:47 gptvm/proto/workspace_pb2_grpc.pyc
+-rw-rw-r--  2.0 unx    34597 b- defN 24-May-10 14:47 gptvm/proto/api_pb2_grpc.pyc
+-rw-rw-r--  2.0 unx     2591 b- defN 24-May-07 07:13 gptvm/proto/image_pb2.pyi
+-rw-rw-r--  2.0 unx      233 b- defN 24-May-10 14:47 gptvm/proto/device_pb2_grpc.pyc
+-rw-rw-r--  2.0 unx      626 b- defN 24-May-07 07:13 gptvm/proto/device_pb2.pyi
+-rw-rw-r--  2.0 unx      234 b- defN 24-May-10 14:47 gptvm/proto/storage_pb2_grpc.pyc
+-rw-rw-r--  2.0 unx     1134 b- defN 24-May-07 07:13 gptvm/proto/account_pb2.pyi
+-rw-rw-r--  2.0 unx     3037 b- defN 24-May-07 07:13 gptvm/proto/workspace_pb2.pyi
+-rw-rw-r--  2.0 unx     1964 b- defN 24-May-07 07:13 gptvm/proto/workgroup_pb2.pyi
+-rw-rw-r--  2.0 unx     2930 b- defN 24-May-10 14:47 gptvm/proto/task_pb2.pyc
+-rw-rw-r--  2.0 unx    18085 b- defN 24-May-07 07:13 gptvm/proto/app_pb2.pyi
+-rw-rw-r--  2.0 unx      234 b- defN 24-May-10 14:47 gptvm/proto/account_pb2_grpc.pyc
+-rw-rw-r--  2.0 unx      238 b- defN 24-May-10 14:47 gptvm/proto/app_version_pb2_grpc.pyc
+-rw-rw-r--  2.0 unx      231 b- defN 24-May-10 14:47 gptvm/proto/user_pb2_grpc.pyc
+-rw-rw-r--  2.0 unx      233 b- defN 24-May-10 14:47 gptvm/proto/common_pb2_grpc.pyc
+-rw-rw-r--  2.0 unx     1178 b- defN 24-May-10 14:47 gptvm/proto/account_pb2.pyc
+-rw-rw-r--  2.0 unx     4278 b- defN 24-May-07 07:13 gptvm/proto/storage_pb2.pyi
+-rw-rw-r--  2.0 unx     2048 b- defN 24-May-10 14:47 gptvm/proto/storage_pb2.pyc
+-rw-rw-r--  2.0 unx     1760 b- defN 24-May-10 14:47 gptvm/proto/workspace_pb2.pyc
+-rw-rw-r--  2.0 unx     6907 b- defN 24-May-10 14:47 gptvm/proto/app_pb2.pyc
+-rw-rw-r--  2.0 unx      230 b- defN 24-May-10 14:47 gptvm/proto/app_pb2_grpc.pyc
+-rw-rw-r--  2.0 unx     2059 b- defN 24-May-10 14:47 gptvm/proto/env_pb2.pyc
+-rw-rw-r--  2.0 unx     1002 b- defN 24-May-07 07:13 gptvm/proto/app_version_pb2.pyi
+-rw-rw-r--  2.0 unx     1470 b- defN 24-May-10 14:47 gptvm/proto/common_pb2.pyc
+-rw-rw-r--  2.0 unx      980 b- defN 24-May-10 14:47 gptvm/proto/device_pb2.pyc
+-rw-rw-r--  2.0 unx     1656 b- defN 24-May-10 14:47 gptvm/proto/image_pb2.pyc
+-rw-rw-r--  2.0 unx     4148 b- defN 24-May-07 07:13 gptvm/proto/user_pb2.pyi
+-rw-rw-r--  2.0 unx      124 b- defN 24-May-10 14:47 gptvm/proto/__init__.pyc
+-rw-rw-r--  2.0 unx      230 b- defN 24-May-10 14:47 gptvm/proto/env_pb2_grpc.pyc
+-rw-rw-r--  2.0 unx     4204 b- defN 24-May-07 07:13 gptvm/proto/env_pb2.pyi
+-rw-rw-r--  2.0 unx      629 b- defN 24-May-07 07:13 gptvm/proto/api_pb2.pyi
+-rw-rw-r--  2.0 unx      232 b- defN 24-May-10 14:47 gptvm/proto/image_pb2_grpc.pyc
+-rw-rw-r--  2.0 unx      231 b- defN 24-May-10 14:47 gptvm/proto/task_pb2_grpc.pyc
+-rw-rw-r--  2.0 unx     2522 b- defN 24-May-10 14:47 gptvm/proto/hello_pb2_grpc.pyc
+-rw-rw-r--  2.0 unx     1412 b- defN 24-May-10 14:47 gptvm/proto/workgroup_pb2.pyc
+-rw-rw-r--  2.0 unx     2448 b- defN 24-May-10 14:47 gptvm/proto/user_pb2.pyc
+-rw-rw-r--  2.0 unx     1109 b- defN 24-May-10 14:47 gptvm/proto/app_version_pb2.pyc
+-rw-rw-r--  2.0 unx     2256 b- defN 24-May-07 07:13 gptvm/proto/common_pb2.pyi
+-rw-rw-r--  2.0 unx     1566 b- defN 24-May-10 14:47 gptvm/cli/cli.pyc
+-rw-rw-r--  2.0 unx     5792 b- defN 24-May-10 14:47 gptvm/cli/runtime.pyc
+-rw-rw-r--  2.0 unx     1175 b- defN 24-May-10 14:47 gptvm/cli/run.pyc
+-rw-rw-r--  2.0 unx     2612 b- defN 24-May-10 14:47 gptvm/cli/import_vm.pyc
+-rw-rw-r--  2.0 unx     1889 b- defN 24-May-10 14:47 gptvm/cli/serve.pyc
+-rw-rw-r--  2.0 unx     1236 b- defN 24-May-10 14:47 gptvm/cli/runner.pyc
+-rw-rw-r--  2.0 unx     3671 b- defN 24-May-10 14:47 gptvm/cli/app.pyc
+-rw-rw-r--  2.0 unx     1031 b- defN 24-May-10 14:47 gptvm/cli/auth.pyc
+-rw-rw-r--  2.0 unx      122 b- defN 24-May-10 14:47 gptvm/cli/__init__.pyc
+-rw-rw-r--  2.0 unx     1290 b- defN 24-May-10 14:47 gptvm/cli/env.pyc
+-rw-rw-r--  2.0 unx     1404 b- defN 24-May-10 14:47 gptvm/runner/base.pyc
+-rw-rw-r--  2.0 unx     1382 b- defN 24-May-10 14:47 gptvm/runner/local.pyc
+-rw-rw-r--  2.0 unx     7276 b- defN 24-May-10 14:47 gptvm/runner/remote.pyc
+-rw-rw-r--  2.0 unx      181 b- defN 24-May-10 14:47 gptvm/runner/__init__.pyc
+76 files, 173634 bytes uncompressed, 61108 bytes compressed:  64.8%
```

## zipnote {}

```diff
@@ -1,211 +1,229 @@
-Filename: gptvm/__init__.py
+Filename: gptvm/
 Comment: 
 
-Filename: gptvm/__main__.py
+Filename: gptvm-0.1.3.dist-info/
 Comment: 
 
-Filename: gptvm/api.py
+Filename: gptvm-0.1.3.dist-info/top_level.txt
 Comment: 
 
-Filename: gptvm/app.py
+Filename: gptvm-0.1.3.dist-info/WHEEL
 Comment: 
 
-Filename: gptvm/cls.py
+Filename: gptvm-0.1.3.dist-info/METADATA
 Comment: 
 
-Filename: gptvm/config.py
+Filename: gptvm-0.1.3.dist-info/entry_points.txt
 Comment: 
 
-Filename: gptvm/function.py
+Filename: gptvm-0.1.3.dist-info/RECORD
 Comment: 
 
-Filename: gptvm/log.py
+Filename: gptvm/cli/
 Comment: 
 
-Filename: gptvm/vmcfg.py
+Filename: gptvm/proto/
 Comment: 
 
-Filename: gptvm/cli/__init__.py
+Filename: gptvm/runner/
 Comment: 
 
-Filename: gptvm/cli/app.py
+Filename: gptvm/api.pyc
 Comment: 
 
-Filename: gptvm/cli/auth.py
+Filename: gptvm/config.pyc
 Comment: 
 
-Filename: gptvm/cli/cli.py
+Filename: gptvm/cls.pyc
 Comment: 
 
-Filename: gptvm/cli/env.py
+Filename: gptvm/log.pyc
 Comment: 
 
-Filename: gptvm/cli/import_vm.py
+Filename: gptvm/vmcfg.pyc
 Comment: 
 
-Filename: gptvm/cli/run.py
+Filename: gptvm/__main__.pyc
 Comment: 
 
-Filename: gptvm/cli/runtime.py
+Filename: gptvm/app.pyc
 Comment: 
 
-Filename: gptvm/cli/serve.py
+Filename: gptvm/__init__.pyc
 Comment: 
 
-Filename: gptvm/proto/__init__.py
+Filename: gptvm/function.pyc
 Comment: 
 
-Filename: gptvm/proto/account_pb2.py
+Filename: gptvm/proto/workgroup_pb2_grpc.pyc
 Comment: 
 
-Filename: gptvm/proto/account_pb2.pyi
+Filename: gptvm/proto/api_pb2.pyc
 Comment: 
 
-Filename: gptvm/proto/account_pb2_grpc.py
+Filename: gptvm/proto/task_pb2.pyi
 Comment: 
 
-Filename: gptvm/proto/api_pb2.py
+Filename: gptvm/proto/hello_pb2.pyc
 Comment: 
 
-Filename: gptvm/proto/api_pb2.pyi
+Filename: gptvm/proto/hello_pb2.pyi
 Comment: 
 
-Filename: gptvm/proto/api_pb2_grpc.py
+Filename: gptvm/proto/workspace_pb2_grpc.pyc
 Comment: 
 
-Filename: gptvm/proto/app_pb2.py
+Filename: gptvm/proto/api_pb2_grpc.pyc
 Comment: 
 
-Filename: gptvm/proto/app_pb2.pyi
+Filename: gptvm/proto/image_pb2.pyi
 Comment: 
 
-Filename: gptvm/proto/app_pb2_grpc.py
+Filename: gptvm/proto/device_pb2_grpc.pyc
 Comment: 
 
-Filename: gptvm/proto/app_version_pb2.py
+Filename: gptvm/proto/device_pb2.pyi
 Comment: 
 
-Filename: gptvm/proto/app_version_pb2.pyi
+Filename: gptvm/proto/storage_pb2_grpc.pyc
 Comment: 
 
-Filename: gptvm/proto/app_version_pb2_grpc.py
+Filename: gptvm/proto/account_pb2.pyi
 Comment: 
 
-Filename: gptvm/proto/common_pb2.py
+Filename: gptvm/proto/workspace_pb2.pyi
 Comment: 
 
-Filename: gptvm/proto/common_pb2.pyi
+Filename: gptvm/proto/workgroup_pb2.pyi
 Comment: 
 
-Filename: gptvm/proto/common_pb2_grpc.py
+Filename: gptvm/proto/task_pb2.pyc
 Comment: 
 
-Filename: gptvm/proto/device_pb2.py
+Filename: gptvm/proto/app_pb2.pyi
 Comment: 
 
-Filename: gptvm/proto/device_pb2.pyi
+Filename: gptvm/proto/account_pb2_grpc.pyc
 Comment: 
 
-Filename: gptvm/proto/device_pb2_grpc.py
+Filename: gptvm/proto/app_version_pb2_grpc.pyc
 Comment: 
 
-Filename: gptvm/proto/env_pb2.py
+Filename: gptvm/proto/user_pb2_grpc.pyc
 Comment: 
 
-Filename: gptvm/proto/env_pb2.pyi
+Filename: gptvm/proto/common_pb2_grpc.pyc
 Comment: 
 
-Filename: gptvm/proto/env_pb2_grpc.py
+Filename: gptvm/proto/account_pb2.pyc
 Comment: 
 
-Filename: gptvm/proto/hello_pb2.py
+Filename: gptvm/proto/storage_pb2.pyi
 Comment: 
 
-Filename: gptvm/proto/hello_pb2.pyi
+Filename: gptvm/proto/storage_pb2.pyc
 Comment: 
 
-Filename: gptvm/proto/hello_pb2_grpc.py
+Filename: gptvm/proto/workspace_pb2.pyc
 Comment: 
 
-Filename: gptvm/proto/image_pb2.py
+Filename: gptvm/proto/app_pb2.pyc
 Comment: 
 
-Filename: gptvm/proto/image_pb2.pyi
+Filename: gptvm/proto/app_pb2_grpc.pyc
 Comment: 
 
-Filename: gptvm/proto/image_pb2_grpc.py
+Filename: gptvm/proto/env_pb2.pyc
 Comment: 
 
-Filename: gptvm/proto/storage_pb2.py
+Filename: gptvm/proto/app_version_pb2.pyi
 Comment: 
 
-Filename: gptvm/proto/storage_pb2.pyi
+Filename: gptvm/proto/common_pb2.pyc
 Comment: 
 
-Filename: gptvm/proto/storage_pb2_grpc.py
+Filename: gptvm/proto/device_pb2.pyc
 Comment: 
 
-Filename: gptvm/proto/task_pb2.py
+Filename: gptvm/proto/image_pb2.pyc
 Comment: 
 
-Filename: gptvm/proto/task_pb2.pyi
+Filename: gptvm/proto/user_pb2.pyi
 Comment: 
 
-Filename: gptvm/proto/task_pb2_grpc.py
+Filename: gptvm/proto/__init__.pyc
 Comment: 
 
-Filename: gptvm/proto/user_pb2.py
+Filename: gptvm/proto/env_pb2_grpc.pyc
 Comment: 
 
-Filename: gptvm/proto/user_pb2.pyi
+Filename: gptvm/proto/env_pb2.pyi
+Comment: 
+
+Filename: gptvm/proto/api_pb2.pyi
 Comment: 
 
-Filename: gptvm/proto/user_pb2_grpc.py
+Filename: gptvm/proto/image_pb2_grpc.pyc
 Comment: 
 
-Filename: gptvm/proto/workgroup_pb2.py
+Filename: gptvm/proto/task_pb2_grpc.pyc
 Comment: 
 
-Filename: gptvm/proto/workgroup_pb2.pyi
+Filename: gptvm/proto/hello_pb2_grpc.pyc
 Comment: 
 
-Filename: gptvm/proto/workgroup_pb2_grpc.py
+Filename: gptvm/proto/workgroup_pb2.pyc
 Comment: 
 
-Filename: gptvm/proto/workspace_pb2.py
+Filename: gptvm/proto/user_pb2.pyc
 Comment: 
 
-Filename: gptvm/proto/workspace_pb2.pyi
+Filename: gptvm/proto/app_version_pb2.pyc
+Comment: 
+
+Filename: gptvm/proto/common_pb2.pyi
+Comment: 
+
+Filename: gptvm/cli/cli.pyc
+Comment: 
+
+Filename: gptvm/cli/runtime.pyc
+Comment: 
+
+Filename: gptvm/cli/run.pyc
+Comment: 
+
+Filename: gptvm/cli/import_vm.pyc
 Comment: 
 
-Filename: gptvm/proto/workspace_pb2_grpc.py
+Filename: gptvm/cli/serve.pyc
 Comment: 
 
-Filename: gptvm/runner/__init__.py
+Filename: gptvm/cli/runner.pyc
 Comment: 
 
-Filename: gptvm/runner/base.py
+Filename: gptvm/cli/app.pyc
 Comment: 
 
-Filename: gptvm/runner/local.py
+Filename: gptvm/cli/auth.pyc
 Comment: 
 
-Filename: gptvm/runner/remote.py
+Filename: gptvm/cli/__init__.pyc
 Comment: 
 
-Filename: gptvm-0.1.2.dist-info/METADATA
+Filename: gptvm/cli/env.pyc
 Comment: 
 
-Filename: gptvm-0.1.2.dist-info/WHEEL
+Filename: gptvm/runner/base.pyc
 Comment: 
 
-Filename: gptvm-0.1.2.dist-info/entry_points.txt
+Filename: gptvm/runner/local.pyc
 Comment: 
 
-Filename: gptvm-0.1.2.dist-info/top_level.txt
+Filename: gptvm/runner/remote.pyc
 Comment: 
 
-Filename: gptvm-0.1.2.dist-info/RECORD
+Filename: gptvm/runner/__init__.pyc
 Comment: 
 
 Zip file comment:
```

## filetype from file(1)

```diff
@@ -1 +1 @@
-Zip archive data, at least v2.0 to extract, compression method=deflate
+Zip archive data, at least v2.0 to extract, compression method=store
```

