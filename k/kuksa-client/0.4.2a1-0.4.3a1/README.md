# Comparing `tmp/kuksa_client-0.4.2a1.tar.gz` & `tmp/kuksa_client-0.4.3a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kuksa_client-0.4.2a1.tar", last modified: Thu Nov 16 14:11:43 2023, max compression
+gzip compressed data, was "kuksa_client-0.4.3a1.tar", last modified: Fri May 10 09:26:27 2024, max compression
```

## Comparing `kuksa_client-0.4.2a1.tar` & `kuksa_client-0.4.3a1.tar`

### file list

```diff
@@ -1,68 +1,49 @@
-drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2023-11-16 14:11:43.107621 kuksa_client-0.4.2a1/
--rw-r--r--   0 erik      (1000) erik      (1000)    11357 2023-11-15 13:27:56.000000 kuksa_client-0.4.2a1/LICENSE
--rw-r--r--   0 erik      (1000) erik      (1000)       35 2023-11-15 13:27:56.000000 kuksa_client-0.4.2a1/MANIFEST.in
--rw-r--r--   0 erik      (1000) erik      (1000)     4563 2023-11-16 14:11:43.107621 kuksa_client-0.4.2a1/PKG-INFO
--rw-r--r--   0 erik      (1000) erik      (1000)     3324 2023-11-16 13:47:33.000000 kuksa_client-0.4.2a1/README.md
-drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2023-11-16 14:11:43.083633 kuksa_client-0.4.2a1/kuksa/
--rw-r--r--   0 erik      (1000) erik      (1000)      580 2023-11-15 13:27:56.000000 kuksa_client-0.4.2a1/kuksa/__init__.py
-drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2023-11-16 14:11:43.083633 kuksa_client-0.4.2a1/kuksa/val/
--rw-r--r--   0 erik      (1000) erik      (1000)      580 2023-11-15 13:27:56.000000 kuksa_client-0.4.2a1/kuksa/val/__init__.py
-drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2023-11-16 14:11:43.087631 kuksa_client-0.4.2a1/kuksa/val/v1/
--rw-r--r--   0 erik      (1000) erik      (1000)      580 2023-11-15 13:27:56.000000 kuksa_client-0.4.2a1/kuksa/val/v1/__init__.py
--rw-r--r--   0 erik      (1000) erik      (1000)     9992 2023-11-16 14:11:43.000000 kuksa_client-0.4.2a1/kuksa/val/v1/types_pb2.py
--rw-r--r--   0 erik      (1000) erik      (1000)      159 2023-11-16 14:11:43.000000 kuksa_client-0.4.2a1/kuksa/val/v1/types_pb2_grpc.py
--rw-r--r--   0 erik      (1000) erik      (1000)     4057 2023-11-16 14:11:43.000000 kuksa_client-0.4.2a1/kuksa/val/v1/val_pb2.py
--rw-r--r--   0 erik      (1000) erik      (1000)     8731 2023-11-16 14:11:43.000000 kuksa_client-0.4.2a1/kuksa/val/v1/val_pb2_grpc.py
-drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2023-11-16 14:11:43.087631 kuksa_client-0.4.2a1/kuksa_client/
--rw-r--r--   0 erik      (1000) erik      (1000)     3850 2023-11-15 15:04:51.000000 kuksa_client-0.4.2a1/kuksa_client/__init__.py
--rwxr-xr-x   0 erik      (1000) erik      (1000)    27132 2023-11-15 13:27:56.000000 kuksa_client-0.4.2a1/kuksa_client/__main__.py
--rw-r--r--   0 erik      (1000) erik      (1000)     1707 2023-11-15 13:27:56.000000 kuksa_client-0.4.2a1/kuksa_client/_metadata.py
-drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2023-11-16 14:11:43.095627 kuksa_client-0.4.2a1/kuksa_client/cli_backend/
--rw-r--r--   0 erik      (1000) erik      (1000)     2289 2023-11-15 13:27:56.000000 kuksa_client-0.4.2a1/kuksa_client/cli_backend/__init__.py
--rw-r--r--   0 erik      (1000) erik      (1000)    11762 2023-11-15 13:27:56.000000 kuksa_client-0.4.2a1/kuksa_client/cli_backend/grpc.py
--rw-r--r--   0 erik      (1000) erik      (1000)    12495 2023-11-15 13:27:56.000000 kuksa_client-0.4.2a1/kuksa_client/cli_backend/ws.py
-drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2023-11-16 14:11:43.095627 kuksa_client-0.4.2a1/kuksa_client/grpc/
--rw-r--r--   0 erik      (1000) erik      (1000)    41287 2023-11-15 13:27:56.000000 kuksa_client-0.4.2a1/kuksa_client/grpc/__init__.py
--rw-r--r--   0 erik      (1000) erik      (1000)    17846 2023-11-15 13:27:56.000000 kuksa_client-0.4.2a1/kuksa_client/grpc/aio.py
-drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2023-11-16 14:11:43.103623 kuksa_client-0.4.2a1/kuksa_client/kuksa_server_certificates/
--rw-r--r--   0 erik      (1000) erik      (1000)     1675 2023-11-15 14:57:48.000000 kuksa_client-0.4.2a1/kuksa_client/kuksa_server_certificates/CA.key
--rw-r--r--   0 erik      (1000) erik      (1000)     1342 2023-11-15 14:57:48.000000 kuksa_client-0.4.2a1/kuksa_client/kuksa_server_certificates/CA.pem
--rw-r--r--   0 erik      (1000) erik      (1000)     1679 2023-11-15 14:57:48.000000 kuksa_client-0.4.2a1/kuksa_client/kuksa_server_certificates/Client.key
--rw-r--r--   0 erik      (1000) erik      (1000)     1704 2023-11-15 14:57:48.000000 kuksa_client-0.4.2a1/kuksa_client/kuksa_server_certificates/Client.pem
--rw-r--r--   0 erik      (1000) erik      (1000)     3541 2023-11-15 14:57:48.000000 kuksa_client-0.4.2a1/kuksa_client/kuksa_server_certificates/README.md
--rw-r--r--   0 erik      (1000) erik      (1000)     1679 2023-11-15 14:57:48.000000 kuksa_client-0.4.2a1/kuksa_client/kuksa_server_certificates/Server.key
--rw-r--r--   0 erik      (1000) erik      (1000)     1704 2023-11-15 14:57:48.000000 kuksa_client-0.4.2a1/kuksa_client/kuksa_server_certificates/Server.pem
--rw-r--r--   0 erik      (1000) erik      (1000)      114 2023-11-15 14:57:48.000000 kuksa_client-0.4.2a1/kuksa_client/kuksa_server_certificates/__init__.py
--rwxr-xr-x   0 erik      (1000) erik      (1000)     2076 2023-11-15 14:57:48.000000 kuksa_client-0.4.2a1/kuksa_client/kuksa_server_certificates/genCerts.sh
-drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2023-11-16 14:11:43.107621 kuksa_client-0.4.2a1/kuksa_client/kuksa_server_certificates/jwt/
--rw-r--r--   0 erik      (1000) erik      (1000)      849 2023-11-15 14:57:48.000000 kuksa_client-0.4.2a1/kuksa_client/kuksa_server_certificates/jwt/README.md
--rw-r--r--   0 erik      (1000) erik      (1000)      151 2023-11-15 14:57:48.000000 kuksa_client-0.4.2a1/kuksa_client/kuksa_server_certificates/jwt/all-read-write.json
--rw-r--r--   0 erik      (1000) erik      (1000)      875 2023-11-15 14:57:48.000000 kuksa_client-0.4.2a1/kuksa_client/kuksa_server_certificates/jwt/all-read-write.json.token
--rwxr-xr-x   0 erik      (1000) erik      (1000)     1879 2023-11-15 14:57:48.000000 kuksa_client-0.4.2a1/kuksa_client/kuksa_server_certificates/jwt/createToken.py
--rw-r--r--   0 erik      (1000) erik      (1000)     3243 2023-11-15 14:57:48.000000 kuksa_client-0.4.2a1/kuksa_client/kuksa_server_certificates/jwt/jwt.key
--rw-r--r--   0 erik      (1000) erik      (1000)      800 2023-11-15 14:57:48.000000 kuksa_client-0.4.2a1/kuksa_client/kuksa_server_certificates/jwt/jwt.key.pub
--rwxr-xr-x   0 erik      (1000) erik      (1000)      901 2023-11-15 14:57:48.000000 kuksa_client-0.4.2a1/kuksa_client/kuksa_server_certificates/jwt/recreateJWTkeyPair.sh
--rw-r--r--   0 erik      (1000) erik      (1000)       34 2023-11-15 14:57:48.000000 kuksa_client-0.4.2a1/kuksa_client/kuksa_server_certificates/jwt/requirements.txt
--rw-r--r--   0 erik      (1000) erik      (1000)      167 2023-11-15 14:57:48.000000 kuksa_client-0.4.2a1/kuksa_client/kuksa_server_certificates/jwt/single-read.json
--rw-r--r--   0 erik      (1000) erik      (1000)      895 2023-11-15 14:57:48.000000 kuksa_client-0.4.2a1/kuksa_client/kuksa_server_certificates/jwt/single-read.json.token
--rw-r--r--   0 erik      (1000) erik      (1000)      175 2023-11-15 14:57:48.000000 kuksa_client-0.4.2a1/kuksa_client/kuksa_server_certificates/jwt/super-admin.json
--rw-r--r--   0 erik      (1000) erik      (1000)      899 2023-11-15 14:57:48.000000 kuksa_client-0.4.2a1/kuksa_client/kuksa_server_certificates/jwt/super-admin.json.token
--rw-r--r--   0 erik      (1000) erik      (1000)      385 2023-11-15 13:27:56.000000 kuksa_client-0.4.2a1/kuksa_client/logging.ini
--rw-r--r--   0 erik      (1000) erik      (1000)      626 2023-11-15 13:27:56.000000 kuksa_client-0.4.2a1/kuksa_client/logo
-drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2023-11-16 14:11:43.107621 kuksa_client-0.4.2a1/kuksa_client/ws/
--rw-r--r--   0 erik      (1000) erik      (1000)      580 2023-11-15 13:27:56.000000 kuksa_client-0.4.2a1/kuksa_client/ws/__init__.py
-drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2023-11-16 14:11:43.091629 kuksa_client-0.4.2a1/kuksa_client.egg-info/
--rw-r--r--   0 erik      (1000) erik      (1000)     4563 2023-11-16 14:11:43.000000 kuksa_client-0.4.2a1/kuksa_client.egg-info/PKG-INFO
--rw-r--r--   0 erik      (1000) erik      (1000)     2007 2023-11-16 14:11:43.000000 kuksa_client-0.4.2a1/kuksa_client.egg-info/SOURCES.txt
--rw-r--r--   0 erik      (1000) erik      (1000)        1 2023-11-16 14:11:43.000000 kuksa_client-0.4.2a1/kuksa_client.egg-info/dependency_links.txt
--rw-r--r--   0 erik      (1000) erik      (1000)       60 2023-11-16 14:11:43.000000 kuksa_client-0.4.2a1/kuksa_client.egg-info/entry_points.txt
--rw-r--r--   0 erik      (1000) erik      (1000)      162 2023-11-16 14:11:43.000000 kuksa_client-0.4.2a1/kuksa_client.egg-info/requires.txt
--rw-r--r--   0 erik      (1000) erik      (1000)       25 2023-11-16 14:11:43.000000 kuksa_client-0.4.2a1/kuksa_client.egg-info/top_level.txt
--rw-r--r--   0 erik      (1000) erik      (1000)      661 2023-11-15 13:27:56.000000 kuksa_client-0.4.2a1/pyproject.toml
--rw-r--r--   0 erik      (1000) erik      (1000)     1283 2023-11-16 14:11:43.111619 kuksa_client-0.4.2a1/setup.cfg
--rw-r--r--   0 erik      (1000) erik      (1000)     1768 2023-11-15 13:27:56.000000 kuksa_client-0.4.2a1/setup.py
-drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2023-11-16 14:11:43.107621 kuksa_client-0.4.2a1/tests/
--rw-r--r--   0 erik      (1000) erik      (1000)      580 2023-11-15 13:27:56.000000 kuksa_client-0.4.2a1/tests/__init__.py
--rw-r--r--   0 erik      (1000) erik      (1000)     2545 2023-11-15 13:27:56.000000 kuksa_client-0.4.2a1/tests/conftest.py
--rw-r--r--   0 erik      (1000) erik      (1000)     6133 2023-11-15 13:27:56.000000 kuksa_client-0.4.2a1/tests/test_datapoint.py
--rw-r--r--   0 erik      (1000) erik      (1000)    64656 2023-11-15 13:27:56.000000 kuksa_client-0.4.2a1/tests/test_grpc.py
+drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2024-05-10 09:26:27.664031 kuksa_client-0.4.3a1/
+-rw-r--r--   0 erik      (1000) erik      (1000)    11357 2024-04-29 08:15:50.000000 kuksa_client-0.4.3a1/LICENSE
+-rw-r--r--   0 erik      (1000) erik      (1000)       35 2024-04-29 08:15:50.000000 kuksa_client-0.4.3a1/MANIFEST.in
+-rw-r--r--   0 erik      (1000) erik      (1000)     4180 2024-05-10 09:26:27.664031 kuksa_client-0.4.3a1/PKG-INFO
+-rw-r--r--   0 erik      (1000) erik      (1000)     2941 2024-04-29 08:15:50.000000 kuksa_client-0.4.3a1/README.md
+drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2024-05-10 09:26:27.660031 kuksa_client-0.4.3a1/kuksa/
+-rw-r--r--   0 erik      (1000) erik      (1000)      580 2024-04-29 08:15:50.000000 kuksa_client-0.4.3a1/kuksa/__init__.py
+drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2024-05-10 09:26:27.660031 kuksa_client-0.4.3a1/kuksa/val/
+-rw-r--r--   0 erik      (1000) erik      (1000)      580 2024-04-29 08:15:50.000000 kuksa_client-0.4.3a1/kuksa/val/__init__.py
+drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2024-05-10 09:26:27.660031 kuksa_client-0.4.3a1/kuksa/val/v1/
+-rw-r--r--   0 erik      (1000) erik      (1000)      580 2024-04-29 08:15:50.000000 kuksa_client-0.4.3a1/kuksa/val/v1/__init__.py
+-rw-r--r--   0 erik      (1000) erik      (1000)    10052 2024-05-10 09:26:27.000000 kuksa_client-0.4.3a1/kuksa/val/v1/types_pb2.py
+-rw-r--r--   0 erik      (1000) erik      (1000)    13964 2024-05-10 09:26:27.000000 kuksa_client-0.4.3a1/kuksa/val/v1/types_pb2.pyi
+-rw-r--r--   0 erik      (1000) erik      (1000)     1135 2024-05-10 09:26:27.000000 kuksa_client-0.4.3a1/kuksa/val/v1/types_pb2_grpc.py
+-rw-r--r--   0 erik      (1000) erik      (1000)     4117 2024-05-10 09:26:27.000000 kuksa_client-0.4.3a1/kuksa/val/v1/val_pb2.py
+-rw-r--r--   0 erik      (1000) erik      (1000)     4416 2024-05-10 09:26:27.000000 kuksa_client-0.4.3a1/kuksa/val/v1/val_pb2.pyi
+-rw-r--r--   0 erik      (1000) erik      (1000)    10435 2024-05-10 09:26:27.000000 kuksa_client-0.4.3a1/kuksa/val/v1/val_pb2_grpc.py
+drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2024-05-10 09:26:27.660031 kuksa_client-0.4.3a1/kuksa_client/
+-rw-r--r--   0 erik      (1000) erik      (1000)     4630 2024-04-29 12:30:35.000000 kuksa_client-0.4.3a1/kuksa_client/__init__.py
+-rwxr-xr-x   0 erik      (1000) erik      (1000)    26983 2024-05-08 14:12:35.000000 kuksa_client-0.4.3a1/kuksa_client/__main__.py
+-rw-r--r--   0 erik      (1000) erik      (1000)     1761 2024-05-08 14:12:35.000000 kuksa_client-0.4.3a1/kuksa_client/_metadata.py
+drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2024-05-10 09:26:27.660031 kuksa_client-0.4.3a1/kuksa_client/cli_backend/
+-rw-r--r--   0 erik      (1000) erik      (1000)     2083 2024-05-07 11:27:06.000000 kuksa_client-0.4.3a1/kuksa_client/cli_backend/__init__.py
+-rw-r--r--   0 erik      (1000) erik      (1000)    12316 2024-05-08 14:12:58.000000 kuksa_client-0.4.3a1/kuksa_client/cli_backend/grpc.py
+-rw-r--r--   0 erik      (1000) erik      (1000)    12763 2024-05-08 14:12:35.000000 kuksa_client-0.4.3a1/kuksa_client/cli_backend/ws.py
+drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2024-05-10 09:26:27.664031 kuksa_client-0.4.3a1/kuksa_client/grpc/
+-rw-r--r--   0 erik      (1000) erik      (1000)    42873 2024-05-08 14:12:35.000000 kuksa_client-0.4.3a1/kuksa_client/grpc/__init__.py
+-rw-r--r--   0 erik      (1000) erik      (1000)    17846 2024-04-29 08:15:50.000000 kuksa_client-0.4.3a1/kuksa_client/grpc/aio.py
+drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2024-05-10 09:26:27.664031 kuksa_client-0.4.3a1/kuksa_client/kuksa_logger/
+-rw-r--r--   0 erik      (1000) erik      (1000)     4583 2024-05-08 14:12:35.000000 kuksa_client-0.4.3a1/kuksa_client/kuksa_logger/__init__.py
+-rw-r--r--   0 erik      (1000) erik      (1000)      626 2024-04-29 08:15:50.000000 kuksa_client-0.4.3a1/kuksa_client/logo
+drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2024-05-10 09:26:27.664031 kuksa_client-0.4.3a1/kuksa_client/ws/
+-rw-r--r--   0 erik      (1000) erik      (1000)      580 2024-04-29 08:15:50.000000 kuksa_client-0.4.3a1/kuksa_client/ws/__init__.py
+drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2024-05-10 09:26:27.664031 kuksa_client-0.4.3a1/kuksa_client.egg-info/
+-rw-r--r--   0 erik      (1000) erik      (1000)     4180 2024-05-10 09:26:27.000000 kuksa_client-0.4.3a1/kuksa_client.egg-info/PKG-INFO
+-rw-r--r--   0 erik      (1000) erik      (1000)      931 2024-05-10 09:26:27.000000 kuksa_client-0.4.3a1/kuksa_client.egg-info/SOURCES.txt
+-rw-r--r--   0 erik      (1000) erik      (1000)        1 2024-05-10 09:26:27.000000 kuksa_client-0.4.3a1/kuksa_client.egg-info/dependency_links.txt
+-rw-r--r--   0 erik      (1000) erik      (1000)       60 2024-05-10 09:26:27.000000 kuksa_client-0.4.3a1/kuksa_client.egg-info/entry_points.txt
+-rw-r--r--   0 erik      (1000) erik      (1000)      162 2024-05-10 09:26:27.000000 kuksa_client-0.4.3a1/kuksa_client.egg-info/requires.txt
+-rw-r--r--   0 erik      (1000) erik      (1000)       25 2024-05-10 09:26:27.000000 kuksa_client-0.4.3a1/kuksa_client.egg-info/top_level.txt
+-rw-r--r--   0 erik      (1000) erik      (1000)      661 2024-05-08 14:12:35.000000 kuksa_client-0.4.3a1/pyproject.toml
+-rw-r--r--   0 erik      (1000) erik      (1000)     1221 2024-05-10 09:26:27.664031 kuksa_client-0.4.3a1/setup.cfg
+-rw-r--r--   0 erik      (1000) erik      (1000)     1768 2024-04-29 08:15:50.000000 kuksa_client-0.4.3a1/setup.py
+drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2024-05-10 09:26:27.664031 kuksa_client-0.4.3a1/tests/
+-rw-r--r--   0 erik      (1000) erik      (1000)      580 2024-04-29 08:15:50.000000 kuksa_client-0.4.3a1/tests/__init__.py
+-rw-r--r--   0 erik      (1000) erik      (1000)     2545 2024-04-29 08:15:50.000000 kuksa_client-0.4.3a1/tests/conftest.py
+-rw-r--r--   0 erik      (1000) erik      (1000)     4157 2024-04-29 08:15:50.000000 kuksa_client-0.4.3a1/tests/test_basevssclient.py
+-rw-r--r--   0 erik      (1000) erik      (1000)     7647 2024-04-29 08:15:50.000000 kuksa_client-0.4.3a1/tests/test_datapoint.py
+-rw-r--r--   0 erik      (1000) erik      (1000)    67181 2024-04-29 08:15:50.000000 kuksa_client-0.4.3a1/tests/test_grpc.py
```

### Comparing `kuksa_client-0.4.2a1/LICENSE` & `kuksa_client-0.4.3a1/LICENSE`

 * *Files identical despite different names*

### Comparing `kuksa_client-0.4.2a1/PKG-INFO` & `kuksa_client-0.4.3a1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kuksa_client
-Version: 0.4.2a1
+Version: 0.4.3a1
 Summary: KUKSA Python Client and SDK
 Home-page: https://github.com/eclipse-kuksa/kuksa-python-sdk
 Author: Eclipse KUKSA Project
 Author-email: kuksa-dev@eclipse.org
 Project-URL: Source, https://github.com/eclipse-kuksa/kuksa-python-sdk
 Project-URL: Bug Tracker, https://github.com/eclipse-kuksa/kuksa-python-sdk/issues
 Classifier: Intended Audience :: Developers
@@ -16,33 +16,26 @@
 Classifier: Topic :: Software Development
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: websockets>=10.1
 Requires-Dist: cmd2<2.0,>=1.4
 Requires-Dist: pygments>=2.15
-Requires-Dist: grpcio-tools>=1.54.2
+Requires-Dist: grpcio-tools>=1.63.0
 Requires-Dist: jsonpath-ng>=1.5.3
 Provides-Extra: test
 Requires-Dist: pylint; extra == "test"
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: pytest-asyncio; extra == "test"
 Requires-Dist: pytest-cov; extra == "test"
 Requires-Dist: pytest-mock; extra == "test"
 Requires-Dist: pytest-timeout; extra == "test"
 
 # KUKSA Python SDK
-![kuksa.val Logo](https://github.com/eclipse-kuksa/kuksa-python-sdk/blob/main/docs/pictures/logo.png)
-
-
-**Note: The KUKSA project is currently in the process of moving the KUKSA Python SDK (kuksa-client)**
-**from the [kuksa.val](https://github.com/eclipse/kuksa.val/tree/master/kuksa-client) repository**
-**to this repository. This repository is still in *draft* status!**
-**Use kuksa.val for development, pull requests and issues until kuksa-client has been removed**
-**from that repository!**
+![kuksa.val Logo](https://raw.githubusercontent.com/eclipse-kuksa/kuksa-python-sdk/main/docs/pictures/logo.png)
 
 KUKSA Python Client and SDK is a part of the open source project [Eclipse KUKSA](https://www.eclipse.org/kuksa/).
 More about Eclipse KUKSA can be found in the [repository](https://github.com/eclipse/kuksa.val).
 
 ## Introduction
 
 KUKSA Python SDK provides both a command-line interface (CLI) and a standalone library to interact with either
```

### Comparing `kuksa_client-0.4.2a1/README.md` & `kuksa_client-0.4.3a1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,9 @@
 # KUKSA Python SDK
-![kuksa.val Logo](https://github.com/eclipse-kuksa/kuksa-python-sdk/blob/main/docs/pictures/logo.png)
-
-
-**Note: The KUKSA project is currently in the process of moving the KUKSA Python SDK (kuksa-client)**
-**from the [kuksa.val](https://github.com/eclipse/kuksa.val/tree/master/kuksa-client) repository**
-**to this repository. This repository is still in *draft* status!**
-**Use kuksa.val for development, pull requests and issues until kuksa-client has been removed**
-**from that repository!**
+![kuksa.val Logo](https://raw.githubusercontent.com/eclipse-kuksa/kuksa-python-sdk/main/docs/pictures/logo.png)
 
 KUKSA Python Client and SDK is a part of the open source project [Eclipse KUKSA](https://www.eclipse.org/kuksa/).
 More about Eclipse KUKSA can be found in the [repository](https://github.com/eclipse/kuksa.val).
 
 ## Introduction
 
 KUKSA Python SDK provides both a command-line interface (CLI) and a standalone library to interact with either
```

### Comparing `kuksa_client-0.4.2a1/kuksa/__init__.py` & `kuksa_client-0.4.3a1/kuksa/__init__.py`

 * *Files identical despite different names*

### Comparing `kuksa_client-0.4.2a1/kuksa/val/__init__.py` & `kuksa_client-0.4.3a1/kuksa/val/__init__.py`

 * *Files identical despite different names*

### Comparing `kuksa_client-0.4.2a1/kuksa/val/v1/__init__.py` & `kuksa_client-0.4.3a1/kuksa/val/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `kuksa_client-0.4.2a1/kuksa/val/v1/types_pb2.py` & `kuksa_client-0.4.3a1/kuksa/val/v1/types_pb2.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: kuksa/val/v1/types.proto
+# Protobuf Python Version: 5.26.1
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
@@ -15,17 +16,17 @@
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x18kuksa/val/v1/types.proto\x12\x0ckuksa.val.v1\x1a\x1fgoogle/protobuf/timestamp.proto\"\x9d\x01\n\tDataEntry\x12\x0c\n\x04path\x18\x01 \x01(\t\x12&\n\x05value\x18\x02 \x01(\x0b\x32\x17.kuksa.val.v1.Datapoint\x12\x30\n\x0f\x61\x63tuator_target\x18\x03 \x01(\x0b\x32\x17.kuksa.val.v1.Datapoint\x12(\n\x08metadata\x18\n \x01(\x0b\x32\x16.kuksa.val.v1.Metadata\"\xdc\x04\n\tDatapoint\x12-\n\ttimestamp\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x10\n\x06string\x18\x0b \x01(\tH\x00\x12\x0e\n\x04\x62ool\x18\x0c \x01(\x08H\x00\x12\x0f\n\x05int32\x18\r \x01(\x11H\x00\x12\x0f\n\x05int64\x18\x0e \x01(\x12H\x00\x12\x10\n\x06uint32\x18\x0f \x01(\rH\x00\x12\x10\n\x06uint64\x18\x10 \x01(\x04H\x00\x12\x0f\n\x05\x66loat\x18\x11 \x01(\x02H\x00\x12\x10\n\x06\x64ouble\x18\x12 \x01(\x01H\x00\x12\x31\n\x0cstring_array\x18\x15 \x01(\x0b\x32\x19.kuksa.val.v1.StringArrayH\x00\x12-\n\nbool_array\x18\x16 \x01(\x0b\x32\x17.kuksa.val.v1.BoolArrayH\x00\x12/\n\x0bint32_array\x18\x17 \x01(\x0b\x32\x18.kuksa.val.v1.Int32ArrayH\x00\x12/\n\x0bint64_array\x18\x18 \x01(\x0b\x32\x18.kuksa.val.v1.Int64ArrayH\x00\x12\x31\n\x0cuint32_array\x18\x19 \x01(\x0b\x32\x19.kuksa.val.v1.Uint32ArrayH\x00\x12\x31\n\x0cuint64_array\x18\x1a \x01(\x0b\x32\x19.kuksa.val.v1.Uint64ArrayH\x00\x12/\n\x0b\x66loat_array\x18\x1b \x01(\x0b\x32\x18.kuksa.val.v1.FloatArrayH\x00\x12\x31\n\x0c\x64ouble_array\x18\x1c \x01(\x0b\x32\x19.kuksa.val.v1.DoubleArrayH\x00\x42\x07\n\x05value\"\xc3\x03\n\x08Metadata\x12)\n\tdata_type\x18\x0b \x01(\x0e\x32\x16.kuksa.val.v1.DataType\x12+\n\nentry_type\x18\x0c \x01(\x0e\x32\x17.kuksa.val.v1.EntryType\x12\x18\n\x0b\x64\x65scription\x18\r \x01(\tH\x01\x88\x01\x01\x12\x14\n\x07\x63omment\x18\x0e \x01(\tH\x02\x88\x01\x01\x12\x18\n\x0b\x64\x65precation\x18\x0f \x01(\tH\x03\x88\x01\x01\x12\x11\n\x04unit\x18\x10 \x01(\tH\x04\x88\x01\x01\x12\x39\n\x11value_restriction\x18\x11 \x01(\x0b\x32\x1e.kuksa.val.v1.ValueRestriction\x12*\n\x08\x61\x63tuator\x18\x14 \x01(\x0b\x32\x16.kuksa.val.v1.ActuatorH\x00\x12&\n\x06sensor\x18\x1e \x01(\x0b\x32\x14.kuksa.val.v1.SensorH\x00\x12,\n\tattribute\x18( \x01(\x0b\x32\x17.kuksa.val.v1.AttributeH\x00\x42\x10\n\x0e\x65ntry_specificB\x0e\n\x0c_descriptionB\n\n\x08_commentB\x0e\n\x0c_deprecationB\x07\n\x05_unit\"\n\n\x08\x41\x63tuator\"\x08\n\x06Sensor\"\x0b\n\tAttribute\"\xfe\x01\n\x10ValueRestriction\x12\x36\n\x06string\x18\x15 \x01(\x0b\x32$.kuksa.val.v1.ValueRestrictionStringH\x00\x12\x33\n\x06signed\x18\x16 \x01(\x0b\x32!.kuksa.val.v1.ValueRestrictionIntH\x00\x12\x36\n\x08unsigned\x18\x17 \x01(\x0b\x32\".kuksa.val.v1.ValueRestrictionUintH\x00\x12=\n\x0e\x66loating_point\x18\x18 \x01(\x0b\x32#.kuksa.val.v1.ValueRestrictionFloatH\x00\x42\x06\n\x04type\"a\n\x13ValueRestrictionInt\x12\x10\n\x03min\x18\x01 \x01(\x12H\x00\x88\x01\x01\x12\x10\n\x03max\x18\x02 \x01(\x12H\x01\x88\x01\x01\x12\x16\n\x0e\x61llowed_values\x18\x03 \x03(\x12\x42\x06\n\x04_minB\x06\n\x04_max\"b\n\x14ValueRestrictionUint\x12\x10\n\x03min\x18\x01 \x01(\x04H\x00\x88\x01\x01\x12\x10\n\x03max\x18\x02 \x01(\x04H\x01\x88\x01\x01\x12\x16\n\x0e\x61llowed_values\x18\x03 \x03(\x04\x42\x06\n\x04_minB\x06\n\x04_max\"c\n\x15ValueRestrictionFloat\x12\x10\n\x03min\x18\x01 \x01(\x01H\x00\x88\x01\x01\x12\x10\n\x03max\x18\x02 \x01(\x01H\x01\x88\x01\x01\x12\x16\n\x0e\x61llowed_values\x18\x03 \x03(\x01\x42\x06\n\x04_minB\x06\n\x04_max\"0\n\x16ValueRestrictionString\x12\x16\n\x0e\x61llowed_values\x18\x03 \x03(\t\"6\n\x05\x45rror\x12\x0c\n\x04\x63ode\x18\x01 \x01(\r\x12\x0e\n\x06reason\x18\x02 \x01(\t\x12\x0f\n\x07message\x18\x03 \x01(\t\"B\n\x0e\x44\x61taEntryError\x12\x0c\n\x04path\x18\x01 \x01(\t\x12\"\n\x05\x65rror\x18\x02 \x01(\x0b\x32\x13.kuksa.val.v1.Error\"\x1d\n\x0bStringArray\x12\x0e\n\x06values\x18\x01 \x03(\t\"\x1b\n\tBoolArray\x12\x0e\n\x06values\x18\x01 \x03(\x08\"\x1c\n\nInt32Array\x12\x0e\n\x06values\x18\x01 \x03(\x11\"\x1c\n\nInt64Array\x12\x0e\n\x06values\x18\x01 \x03(\x12\"\x1d\n\x0bUint32Array\x12\x0e\n\x06values\x18\x01 \x03(\r\"\x1d\n\x0bUint64Array\x12\x0e\n\x06values\x18\x01 \x03(\x04\"\x1c\n\nFloatArray\x12\x0e\n\x06values\x18\x01 \x03(\x02\"\x1d\n\x0b\x44oubleArray\x12\x0e\n\x06values\x18\x01 \x03(\x01*\xa9\x05\n\x08\x44\x61taType\x12\x19\n\x15\x44\x41TA_TYPE_UNSPECIFIED\x10\x00\x12\x14\n\x10\x44\x41TA_TYPE_STRING\x10\x01\x12\x15\n\x11\x44\x41TA_TYPE_BOOLEAN\x10\x02\x12\x12\n\x0e\x44\x41TA_TYPE_INT8\x10\x03\x12\x13\n\x0f\x44\x41TA_TYPE_INT16\x10\x04\x12\x13\n\x0f\x44\x41TA_TYPE_INT32\x10\x05\x12\x13\n\x0f\x44\x41TA_TYPE_INT64\x10\x06\x12\x13\n\x0f\x44\x41TA_TYPE_UINT8\x10\x07\x12\x14\n\x10\x44\x41TA_TYPE_UINT16\x10\x08\x12\x14\n\x10\x44\x41TA_TYPE_UINT32\x10\t\x12\x14\n\x10\x44\x41TA_TYPE_UINT64\x10\n\x12\x13\n\x0f\x44\x41TA_TYPE_FLOAT\x10\x0b\x12\x14\n\x10\x44\x41TA_TYPE_DOUBLE\x10\x0c\x12\x17\n\x13\x44\x41TA_TYPE_TIMESTAMP\x10\r\x12\x1a\n\x16\x44\x41TA_TYPE_STRING_ARRAY\x10\x14\x12\x1b\n\x17\x44\x41TA_TYPE_BOOLEAN_ARRAY\x10\x15\x12\x18\n\x14\x44\x41TA_TYPE_INT8_ARRAY\x10\x16\x12\x19\n\x15\x44\x41TA_TYPE_INT16_ARRAY\x10\x17\x12\x19\n\x15\x44\x41TA_TYPE_INT32_ARRAY\x10\x18\x12\x19\n\x15\x44\x41TA_TYPE_INT64_ARRAY\x10\x19\x12\x19\n\x15\x44\x41TA_TYPE_UINT8_ARRAY\x10\x1a\x12\x1a\n\x16\x44\x41TA_TYPE_UINT16_ARRAY\x10\x1b\x12\x1a\n\x16\x44\x41TA_TYPE_UINT32_ARRAY\x10\x1c\x12\x1a\n\x16\x44\x41TA_TYPE_UINT64_ARRAY\x10\x1d\x12\x19\n\x15\x44\x41TA_TYPE_FLOAT_ARRAY\x10\x1e\x12\x1a\n\x16\x44\x41TA_TYPE_DOUBLE_ARRAY\x10\x1f\x12\x1d\n\x19\x44\x41TA_TYPE_TIMESTAMP_ARRAY\x10 *q\n\tEntryType\x12\x1a\n\x16\x45NTRY_TYPE_UNSPECIFIED\x10\x00\x12\x18\n\x14\x45NTRY_TYPE_ATTRIBUTE\x10\x01\x12\x15\n\x11\x45NTRY_TYPE_SENSOR\x10\x02\x12\x17\n\x13\x45NTRY_TYPE_ACTUATOR\x10\x03*}\n\x04View\x12\x14\n\x10VIEW_UNSPECIFIED\x10\x00\x12\x16\n\x12VIEW_CURRENT_VALUE\x10\x01\x12\x15\n\x11VIEW_TARGET_VALUE\x10\x02\x12\x11\n\rVIEW_METADATA\x10\x03\x12\x0f\n\x0bVIEW_FIELDS\x10\n\x12\x0c\n\x08VIEW_ALL\x10\x14*\x9c\x03\n\x05\x46ield\x12\x15\n\x11\x46IELD_UNSPECIFIED\x10\x00\x12\x0e\n\nFIELD_PATH\x10\x01\x12\x0f\n\x0b\x46IELD_VALUE\x10\x02\x12\x19\n\x15\x46IELD_ACTUATOR_TARGET\x10\x03\x12\x12\n\x0e\x46IELD_METADATA\x10\n\x12\x1c\n\x18\x46IELD_METADATA_DATA_TYPE\x10\x0b\x12\x1e\n\x1a\x46IELD_METADATA_DESCRIPTION\x10\x0c\x12\x1d\n\x19\x46IELD_METADATA_ENTRY_TYPE\x10\r\x12\x1a\n\x16\x46IELD_METADATA_COMMENT\x10\x0e\x12\x1e\n\x1a\x46IELD_METADATA_DEPRECATION\x10\x0f\x12\x17\n\x13\x46IELD_METADATA_UNIT\x10\x10\x12$\n FIELD_METADATA_VALUE_RESTRICTION\x10\x11\x12\x1b\n\x17\x46IELD_METADATA_ACTUATOR\x10\x14\x12\x19\n\x15\x46IELD_METADATA_SENSOR\x10\x1e\x12\x1c\n\x18\x46IELD_METADATA_ATTRIBUTE\x10(B\x0eZ\x0ckuksa/val/v1b\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'kuksa.val.v1.types_pb2', _globals)
-if _descriptor._USE_C_DESCRIPTORS == False:
-  DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'Z\014kuksa/val/v1'
+if not _descriptor._USE_C_DESCRIPTORS:
+  _globals['DESCRIPTOR']._loaded_options = None
+  _globals['DESCRIPTOR']._serialized_options = b'Z\014kuksa/val/v1'
   _globals['_DATATYPE']._serialized_start=2306
   _globals['_DATATYPE']._serialized_end=2987
   _globals['_ENTRYTYPE']._serialized_start=2989
   _globals['_ENTRYTYPE']._serialized_end=3102
   _globals['_VIEW']._serialized_start=3104
   _globals['_VIEW']._serialized_end=3229
   _globals['_FIELD']._serialized_start=3232
```

### Comparing `kuksa_client-0.4.2a1/kuksa/val/v1/val_pb2.py` & `kuksa_client-0.4.3a1/kuksa/val/v1/val_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: kuksa/val/v1/val.proto
+# Protobuf Python Version: 5.26.1
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
@@ -15,17 +16,17 @@
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x16kuksa/val/v1/val.proto\x12\x0ckuksa.val.v1\x1a\x18kuksa/val/v1/types.proto\"c\n\x0c\x45ntryRequest\x12\x0c\n\x04path\x18\x01 \x01(\t\x12 \n\x04view\x18\x02 \x01(\x0e\x32\x12.kuksa.val.v1.View\x12#\n\x06\x66ields\x18\x03 \x03(\x0e\x32\x13.kuksa.val.v1.Field\"9\n\nGetRequest\x12+\n\x07\x65ntries\x18\x01 \x03(\x0b\x32\x1a.kuksa.val.v1.EntryRequest\"\x89\x01\n\x0bGetResponse\x12(\n\x07\x65ntries\x18\x01 \x03(\x0b\x32\x17.kuksa.val.v1.DataEntry\x12,\n\x06\x65rrors\x18\x02 \x03(\x0b\x32\x1c.kuksa.val.v1.DataEntryError\x12\"\n\x05\x65rror\x18\x03 \x01(\x0b\x32\x13.kuksa.val.v1.Error\"Z\n\x0b\x45ntryUpdate\x12&\n\x05\x65ntry\x18\x01 \x01(\x0b\x32\x17.kuksa.val.v1.DataEntry\x12#\n\x06\x66ields\x18\x02 \x03(\x0e\x32\x13.kuksa.val.v1.Field\"8\n\nSetRequest\x12*\n\x07updates\x18\x01 \x03(\x0b\x32\x19.kuksa.val.v1.EntryUpdate\"_\n\x0bSetResponse\x12\"\n\x05\x65rror\x18\x01 \x01(\x0b\x32\x13.kuksa.val.v1.Error\x12,\n\x06\x65rrors\x18\x02 \x03(\x0b\x32\x1c.kuksa.val.v1.DataEntryError\"e\n\x0eSubscribeEntry\x12\x0c\n\x04path\x18\x01 \x01(\t\x12 \n\x04view\x18\x02 \x01(\x0e\x32\x12.kuksa.val.v1.View\x12#\n\x06\x66ields\x18\x03 \x03(\x0e\x32\x13.kuksa.val.v1.Field\"A\n\x10SubscribeRequest\x12-\n\x07\x65ntries\x18\x01 \x03(\x0b\x32\x1c.kuksa.val.v1.SubscribeEntry\"?\n\x11SubscribeResponse\x12*\n\x07updates\x18\x01 \x03(\x0b\x32\x19.kuksa.val.v1.EntryUpdate\"\x16\n\x14GetServerInfoRequest\"6\n\x15GetServerInfoResponse\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0f\n\x07version\x18\x02 \x01(\t2\xa7\x02\n\x03VAL\x12:\n\x03Get\x12\x18.kuksa.val.v1.GetRequest\x1a\x19.kuksa.val.v1.GetResponse\x12:\n\x03Set\x12\x18.kuksa.val.v1.SetRequest\x1a\x19.kuksa.val.v1.SetResponse\x12N\n\tSubscribe\x12\x1e.kuksa.val.v1.SubscribeRequest\x1a\x1f.kuksa.val.v1.SubscribeResponse0\x01\x12X\n\rGetServerInfo\x12\".kuksa.val.v1.GetServerInfoRequest\x1a#.kuksa.val.v1.GetServerInfoResponseB\x0eZ\x0ckuksa/val/v1b\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'kuksa.val.v1.val_pb2', _globals)
-if _descriptor._USE_C_DESCRIPTORS == False:
-  DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'Z\014kuksa/val/v1'
+if not _descriptor._USE_C_DESCRIPTORS:
+  _globals['DESCRIPTOR']._loaded_options = None
+  _globals['DESCRIPTOR']._serialized_options = b'Z\014kuksa/val/v1'
   _globals['_ENTRYREQUEST']._serialized_start=66
   _globals['_ENTRYREQUEST']._serialized_end=165
   _globals['_GETREQUEST']._serialized_start=167
   _globals['_GETREQUEST']._serialized_end=224
   _globals['_GETRESPONSE']._serialized_start=227
   _globals['_GETRESPONSE']._serialized_end=364
   _globals['_ENTRYUPDATE']._serialized_start=366
```

### Comparing `kuksa_client-0.4.2a1/kuksa/val/v1/val_pb2_grpc.py` & `kuksa_client-0.4.3a1/kuksa/val/v1/val_pb2_grpc.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,22 +1,47 @@
 # Generated by the gRPC Python protocol compiler plugin. DO NOT EDIT!
 """Client and server classes corresponding to protobuf-defined services."""
 import grpc
+import warnings
 
 from kuksa.val.v1 import val_pb2 as kuksa_dot_val_dot_v1_dot_val__pb2
 
+GRPC_GENERATED_VERSION = '1.63.0'
+GRPC_VERSION = grpc.__version__
+EXPECTED_ERROR_RELEASE = '1.65.0'
+SCHEDULED_RELEASE_DATE = 'June 25, 2024'
+_version_not_supported = False
+
+try:
+    from grpc._utilities import first_version_is_lower
+    _version_not_supported = first_version_is_lower(GRPC_VERSION, GRPC_GENERATED_VERSION)
+except ImportError:
+    _version_not_supported = True
+
+if _version_not_supported:
+    warnings.warn(
+        f'The grpc package installed is at version {GRPC_VERSION},'
+        + f' but the generated code in kuksa/val/v1/val_pb2_grpc.py depends on'
+        + f' grpcio>={GRPC_GENERATED_VERSION}.'
+        + f' Please upgrade your grpc module to grpcio>={GRPC_GENERATED_VERSION}'
+        + f' or downgrade your generated code using grpcio-tools<={GRPC_VERSION}.'
+        + f' This warning will become an error in {EXPECTED_ERROR_RELEASE},'
+        + f' scheduled for release on {SCHEDULED_RELEASE_DATE}.',
+        RuntimeWarning
+    )
+
 
 class VALStub(object):
     """Note on authorization:
     Tokens (auth-token or auth-uuid) are sent as (GRPC / http2) metadata.
 
     The auth-token is a JWT compliant token as the examples found here:
-    https://github.com/eclipse/kuksa.val/tree/master/kuksa_certificates/jwt
+    https://github.com/eclipse-kuksa/kuksa-databrokertree/master/certificates/jwt
 
-    See also https://github.com/eclipse/kuksa.val/blob/master/doc/jwt.md
+    See also https://github.com/eclipse-kuksa/kuksa-databrokerblob/master/doc/jwt.md
 
     Upon reception of auth-token, server shall generate an auth-uuid in metadata
     that the client can use instead of auth-token in subsequent calls.
 
     """
 
     def __init__(self, channel):
@@ -25,40 +50,40 @@
         Args:
             channel: A grpc.Channel.
         """
         self.Get = channel.unary_unary(
                 '/kuksa.val.v1.VAL/Get',
                 request_serializer=kuksa_dot_val_dot_v1_dot_val__pb2.GetRequest.SerializeToString,
                 response_deserializer=kuksa_dot_val_dot_v1_dot_val__pb2.GetResponse.FromString,
-                )
+                _registered_method=True)
         self.Set = channel.unary_unary(
                 '/kuksa.val.v1.VAL/Set',
                 request_serializer=kuksa_dot_val_dot_v1_dot_val__pb2.SetRequest.SerializeToString,
                 response_deserializer=kuksa_dot_val_dot_v1_dot_val__pb2.SetResponse.FromString,
-                )
+                _registered_method=True)
         self.Subscribe = channel.unary_stream(
                 '/kuksa.val.v1.VAL/Subscribe',
                 request_serializer=kuksa_dot_val_dot_v1_dot_val__pb2.SubscribeRequest.SerializeToString,
                 response_deserializer=kuksa_dot_val_dot_v1_dot_val__pb2.SubscribeResponse.FromString,
-                )
+                _registered_method=True)
         self.GetServerInfo = channel.unary_unary(
                 '/kuksa.val.v1.VAL/GetServerInfo',
                 request_serializer=kuksa_dot_val_dot_v1_dot_val__pb2.GetServerInfoRequest.SerializeToString,
                 response_deserializer=kuksa_dot_val_dot_v1_dot_val__pb2.GetServerInfoResponse.FromString,
-                )
+                _registered_method=True)
 
 
 class VALServicer(object):
     """Note on authorization:
     Tokens (auth-token or auth-uuid) are sent as (GRPC / http2) metadata.
 
     The auth-token is a JWT compliant token as the examples found here:
-    https://github.com/eclipse/kuksa.val/tree/master/kuksa_certificates/jwt
+    https://github.com/eclipse-kuksa/kuksa-databrokertree/master/certificates/jwt
 
-    See also https://github.com/eclipse/kuksa.val/blob/master/doc/jwt.md
+    See also https://github.com/eclipse-kuksa/kuksa-databrokerblob/master/doc/jwt.md
 
     Upon reception of auth-token, server shall generate an auth-uuid in metadata
     that the client can use instead of auth-token in subsequent calls.
 
     """
 
     def Get(self, request, context):
@@ -126,17 +151,17 @@
 
  # This class is part of an EXPERIMENTAL API.
 class VAL(object):
     """Note on authorization:
     Tokens (auth-token or auth-uuid) are sent as (GRPC / http2) metadata.
 
     The auth-token is a JWT compliant token as the examples found here:
-    https://github.com/eclipse/kuksa.val/tree/master/kuksa_certificates/jwt
+    https://github.com/eclipse-kuksa/kuksa-databrokertree/master/certificates/jwt
 
-    See also https://github.com/eclipse/kuksa.val/blob/master/doc/jwt.md
+    See also https://github.com/eclipse-kuksa/kuksa-databrokerblob/master/doc/jwt.md
 
     Upon reception of auth-token, server shall generate an auth-uuid in metadata
     that the client can use instead of auth-token in subsequent calls.
 
     """
 
     @staticmethod
@@ -146,63 +171,103 @@
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/kuksa.val.v1.VAL/Get',
+        return grpc.experimental.unary_unary(
+            request,
+            target,
+            '/kuksa.val.v1.VAL/Get',
             kuksa_dot_val_dot_v1_dot_val__pb2.GetRequest.SerializeToString,
             kuksa_dot_val_dot_v1_dot_val__pb2.GetResponse.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+            options,
+            channel_credentials,
+            insecure,
+            call_credentials,
+            compression,
+            wait_for_ready,
+            timeout,
+            metadata,
+            _registered_method=True)
 
     @staticmethod
     def Set(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/kuksa.val.v1.VAL/Set',
+        return grpc.experimental.unary_unary(
+            request,
+            target,
+            '/kuksa.val.v1.VAL/Set',
             kuksa_dot_val_dot_v1_dot_val__pb2.SetRequest.SerializeToString,
             kuksa_dot_val_dot_v1_dot_val__pb2.SetResponse.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+            options,
+            channel_credentials,
+            insecure,
+            call_credentials,
+            compression,
+            wait_for_ready,
+            timeout,
+            metadata,
+            _registered_method=True)
 
     @staticmethod
     def Subscribe(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_stream(request, target, '/kuksa.val.v1.VAL/Subscribe',
+        return grpc.experimental.unary_stream(
+            request,
+            target,
+            '/kuksa.val.v1.VAL/Subscribe',
             kuksa_dot_val_dot_v1_dot_val__pb2.SubscribeRequest.SerializeToString,
             kuksa_dot_val_dot_v1_dot_val__pb2.SubscribeResponse.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+            options,
+            channel_credentials,
+            insecure,
+            call_credentials,
+            compression,
+            wait_for_ready,
+            timeout,
+            metadata,
+            _registered_method=True)
 
     @staticmethod
     def GetServerInfo(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/kuksa.val.v1.VAL/GetServerInfo',
+        return grpc.experimental.unary_unary(
+            request,
+            target,
+            '/kuksa.val.v1.VAL/GetServerInfo',
             kuksa_dot_val_dot_v1_dot_val__pb2.GetServerInfoRequest.SerializeToString,
             kuksa_dot_val_dot_v1_dot_val__pb2.GetServerInfoResponse.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+            options,
+            channel_credentials,
+            insecure,
+            call_credentials,
+            compression,
+            wait_for_ready,
+            timeout,
+            metadata,
+            _registered_method=True)
```

### Comparing `kuksa_client-0.4.2a1/kuksa_client/__init__.py` & `kuksa_client-0.4.3a1/kuksa_client/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -33,16 +33,31 @@
     # Constructor
     def __init__(self, config):
         super().__init__()
 
         self.backend = cli_backend.Backend.from_config(config)
         self.loop = None
 
-    def checkConnection(self):
-        return self.backend.checkConnection()
+    # PEP 702 deprecated decorator available first in Python 3.13
+    def checkConnection(self) -> bool:
+        """
+        Check if thread has established a connection to the broker/server.
+        Note that this method does not indicate the current state of the connection,
+        This method may return True even if the broker/server currently is not reachable.
+        Deprecated - Use connection_established() instead"
+        """
+        return self.connection_established()
+
+    def connection_established(self) -> bool:
+        """
+        Check if thread has established a connection to the broker/server.
+        Note that this method does not indicate the current state of the connection,
+        This method may return True even if the broker/server currently is not reachable.
+        """
+        return self.backend.connection_established()
 
     def stop(self):
         self.backend.stop()
 
     # Do authorization by passing a jwt token or a token file
     def authorize(self, token_or_tokenfile: Optional[str] = None, timeout=5):
         return self.backend.authorize(token_or_tokenfile, timeout)
```

### Comparing `kuksa_client-0.4.2a1/kuksa_client/__main__.py` & `kuksa_client-0.4.3a1/kuksa_client/__main__.py`

 * *Files 5% similar despite different names*

```diff
@@ -35,24 +35,21 @@
 from cmd2 import CompletionItem
 from cmd2 import with_argparser
 from cmd2 import with_category
 from cmd2 import constants
 from cmd2.utils import basic_complete
 from urllib.parse import urlparse
 
-from kuksa_client import kuksa_server_certificates
 from kuksa_client import KuksaClientThread
 from kuksa_client import _metadata
+from kuksa_client.kuksa_logger import KuksaLogger
 
 scriptDir = os.path.dirname(os.path.realpath(__file__))
 
 DEFAULT_KUKSA_ADDRESS = os.environ.get("KUKSA_ADDRESS", "grpc://127.0.0.1:55555")
-DEFAULT_LOGGING_CONFIG = os.environ.get(
-    "LOGGING_CONFIG", os.path.join(scriptDir, "logging.ini")
-)
 DEFAULT_TOKEN_OR_TOKENFILE = os.environ.get("TOKEN_OR_TOKENFILE", None)
 DEFAULT_CERTIFICATE = os.environ.get("CERTIFICATE", None)
 DEFAULT_KEYFILE = os.environ.get("KEYFILE", None)
 DEFAULT_CACERTIFICATE = os.environ.get("CACERTIFICATE", None)
 DEFAULT_TLS_SERVER_NAME = os.environ.get("TLS_SERVER_NAME", None)
 
 
@@ -108,15 +105,15 @@
         else:
             entries = json.loads(self.getMetaData(""))
             if "metadata" in entries:
                 # Convert to dict with paths as key
                 self.metadata = metadata_tree_to_dict(entries["metadata"])
 
     def path_completer(self, text, line, begidx, endidx):
-        if not self.checkConnection():
+        if not self.connection_established():
             return None
 
         if len(self.pathCompletionItems) == 0:
             self.refresh_metadata()
 
         # Normalize the delimiter used
         delimiter = "."
@@ -155,15 +152,16 @@
     def subscriptionIdCompleter(self, text, line, begidx, endidx):
         self.pathCompletionItems = []
         for sub_id in self.subscribeIds:
             self.pathCompletionItems.append(CompletionItem(sub_id))
         return basic_complete(text, line, begidx, endidx, self.pathCompletionItems)
 
     COMM_SETUP_COMMANDS = "Communication Set-up Commands"
-    VSS_COMMANDS = "Kuksa Interaction Commands"
+    VSS_COMMANDS = "Kuksa Interaction Commands (Supported by both KUKSA Databroker and KUKSA Server)"
+    VSS_COMMANDS_SERVER = "Kuksa Interaction Commands (Only supported by KUKSA Server)"
     INFO_COMMANDS = "Info Commands"
 
     ap_connect = argparse.ArgumentParser()
     ap_connect.add_argument(
         "server",
         help=f"VSS server to connect to. Format: protocol://host[:port]. \
         Supported protocols: [grpc, grpcs, ws, wss]. Example: {DEFAULT_KUKSA_ADDRESS}",
@@ -346,34 +344,33 @@
         self.keyfile = keyfile
         self.cacertificate = cacertificate
         self.tls_server_name = tls_server_name
 
         with (pathlib.Path(scriptDir) / "logo").open("r", encoding="utf-8") as f:
             logo = f.read()
             print(logo.replace("%ver%", str(_metadata.__version__)))
-        print("Default tokens directory: " + self.getDefaultTokenDir())
 
         print()
         self.connect()
 
     @with_category(COMM_SETUP_COMMANDS)
     @with_argparser(ap_authorize)
     def do_authorize(self, args):
         """Authorize the client to interact with the server"""
         if args.token_or_tokenfile is not None:
             self.token_or_tokenfile = args.token_or_tokenfile
-        if self.checkConnection():
+        if self.connection_established():
             resp = self.commThread.authorize(self.token_or_tokenfile)
             print(highlight(resp, lexers.JsonLexer(), formatters.TerminalFormatter()))
 
     @with_category(VSS_COMMANDS)
     @with_argparser(ap_setValue)
     def do_setValue(self, args):
         """Set the value of a path"""
-        if self.checkConnection():
+        if self.connection_established():
             # If there is a blank before a single/double quote on the kuksa-client cli then
             # the argparser shell will remove it, there is nothing we can do to it
             # This gives off behavior for examples like:
             # setValue Vehicle.OBD.DTCList [ "dtc1, dtc2", ddd]
             # which will be treated as input of 3 elements
             # The recommended approach is to have quotes (of a different type) around the whole value
             # if your strings includes quotes, commas or other items
@@ -389,82 +386,82 @@
             print(highlight(resp, lexers.JsonLexer(), formatters.TerminalFormatter()))
         self.pathCompletionItems = []
 
     @with_category(VSS_COMMANDS)
     @with_argparser(ap_setValues)
     def do_setValues(self, args):
         """Set the value of given paths"""
-        if self.checkConnection():
+        if self.connection_established():
             resp = self.commThread.setValues(
                 dict(getattr(args, "Path=Value")), args.attribute
             )
             print(highlight(resp, lexers.JsonLexer(), formatters.TerminalFormatter()))
         self.pathCompletionItems = []
 
     @with_category(VSS_COMMANDS)
     @with_argparser(ap_setTargetValue)
     def do_setTargetValue(self, args):
         """Set the target value of a path"""
-        if self.checkConnection():
+        if self.connection_established():
             resp = self.commThread.setValue(args.Path, args.Value, "targetValue")
             print(highlight(resp, lexers.JsonLexer(), formatters.TerminalFormatter()))
         self.pathCompletionItems = []
 
     @with_category(VSS_COMMANDS)
     @with_argparser(ap_setTargetValues)
     def do_setTargetValues(self, args):
         """Set the target value of given paths"""
-        if self.checkConnection():
+        if self.connection_established():
             resp = self.commThread.setValues(
                 dict(getattr(args, "Path=Value")), "targetValue"
             )
             print(highlight(resp, lexers.JsonLexer(), formatters.TerminalFormatter()))
         self.pathCompletionItems = []
 
     @with_category(VSS_COMMANDS)
     @with_argparser(ap_getValue)
     def do_getValue(self, args):
         """Get the value of a path"""
-        if self.checkConnection():
+        if self.connection_established():
             resp = self.commThread.getValue(args.Path, args.attribute)
             print(highlight(resp, lexers.JsonLexer(), formatters.TerminalFormatter()))
         self.pathCompletionItems = []
 
     @with_category(VSS_COMMANDS)
     @with_argparser(ap_getValues)
     def do_getValues(self, args):
         """Get the value of given paths"""
-        if self.checkConnection():
+        if self.connection_established():
             resp = self.commThread.getValues(args.Path, args.attribute)
             print(highlight(resp, lexers.JsonLexer(), formatters.TerminalFormatter()))
         self.pathCompletionItems = []
 
     @with_category(VSS_COMMANDS)
     @with_argparser(ap_getTargetValue)
     def do_getTargetValue(self, args):
         """Get the value of a path"""
-        if self.checkConnection():
+        if self.connection_established():
             resp = self.commThread.getValue(args.Path, "targetValue")
             print(highlight(resp, lexers.JsonLexer(), formatters.TerminalFormatter()))
         self.pathCompletionItems = []
 
     @with_category(VSS_COMMANDS)
     @with_argparser(ap_getTargetValues)
     def do_getTargetValues(self, args):
         """Get the value of given paths"""
-        if self.checkConnection():
+        if self.connection_established():
             resp = self.commThread.getValues(args.Path, "targetValue")
             print(highlight(resp, lexers.JsonLexer(), formatters.TerminalFormatter()))
         self.pathCompletionItems = []
 
     @with_category(VSS_COMMANDS)
     @with_argparser(ap_subscribe)
     def do_subscribe(self, args):
         """Subscribe the value of a path"""
-        if self.checkConnection():
+        if self.connection_established():
             if args.output_to_file:
                 logPath = (
                     pathlib.Path.cwd()
                     / f"log_{args.Path.replace('/', '.')}_{args.attribute}_{str(time.time())}"
                 )
                 callback = functools.partial(self.subscribeCallback, logPath)
             else:
@@ -480,15 +477,15 @@
             print(highlight(resp, lexers.JsonLexer(), formatters.TerminalFormatter()))
         self.pathCompletionItems = []
 
     @with_category(VSS_COMMANDS)
     @with_argparser(ap_subscribeMultiple)
     def do_subscribeMultiple(self, args):
         """Subscribe to updates of given paths"""
-        if self.checkConnection():
+        if self.connection_established():
             if args.output_to_file:
                 logPath = (
                     pathlib.Path.cwd()
                     / f"subscribeMultiple_{args.attribute}_{str(time.time())}.log"
                 )
                 callback = functools.partial(self.subscribeCallback, logPath)
             else:
@@ -505,44 +502,45 @@
             print(highlight(resp, lexers.JsonLexer(), formatters.TerminalFormatter()))
         self.pathCompletionItems = []
 
     @with_category(VSS_COMMANDS)
     @with_argparser(ap_unsubscribe)
     def do_unsubscribe(self, args):
         """Unsubscribe an existing subscription"""
-        if self.checkConnection():
+        if self.connection_established():
             resp = self.commThread.unsubscribe(args.SubscribeId)
             print(highlight(resp, lexers.JsonLexer(), formatters.TerminalFormatter()))
             self.subscribeIds.discard(args.SubscribeId)
             self.pathCompletionItems = []
 
     def stop(self):
         if self.commThread is not None:
             self.commThread.stop()
             self.commThread.join()
 
     def getMetaData(self, path):
         """Get MetaData of the path"""
-        if self.checkConnection():
+        if self.connection_established():
             return self.commThread.getMetaData(path)
         return "{}"
 
-    @with_category(VSS_COMMANDS)
+    @with_category(VSS_COMMANDS_SERVER)
     @with_argparser(ap_updateVSSTree)
     def do_updateVSSTree(self, args):
         """Update VSS Tree Entry"""
-        if self.checkConnection():
+        if self.connection_established():
             resp = self.commThread.updateVSSTree(args.Json)
-            print(highlight(resp, lexers.JsonLexer(), formatters.TerminalFormatter()))
+            if resp is not None:
+                print(highlight(resp, lexers.JsonLexer(), formatters.TerminalFormatter()))
 
     @with_category(VSS_COMMANDS)
     @with_argparser(ap_updateMetaData)
     def do_updateMetaData(self, args):
         """Update MetaData of a given path"""
-        if self.checkConnection():
+        if self.connection_established():
             resp = self.commThread.updateMetaData(args.Path, args.Json)
             print(highlight(resp, lexers.JsonLexer(), formatters.TerminalFormatter()))
 
     @with_category(VSS_COMMANDS)
     @with_argparser(ap_getMetaData)
     def do_getMetaData(self, args):
         """Get MetaData of the path"""
@@ -555,18 +553,23 @@
     def do_disconnect(self, _args):
         """Disconnect from the VISS/gRPC Server"""
         if hasattr(self, "commThread"):
             if self.commThread is not None:
                 self.commThread.stop()
                 self.commThread = None
 
-    def checkConnection(self):
-        if self.commThread is None or not self.commThread.checkConnection():
+    def connection_established(self) -> bool:
+        """
+        Check if thread has established a connection to the broker/server.
+        Note that this method does not indicate the current state of the connection,
+        This method may return True even if the broker/server currently is not reachable.
+        """
+        if self.commThread is None or not self.commThread.connection_established():
             self.connect()
-        return self.commThread.checkConnection()
+        return self.commThread.connection_established()
 
     def connect(self):
         """Connect to the VISS/gRPC Server"""
         if hasattr(self, "commThread"):
             if self.commThread is not None:
                 self.commThread.stop()
                 self.commThread = None
@@ -584,15 +587,18 @@
             print(f"Invalid server URI. Unsupported protocol: {srv.scheme} ")
             return
 
         if srv.port is not None:
             config["port"] = srv.port
 
         if srv.scheme in ["grpcs", "wss"]:
-            config["insecure"] = False
+            if self.cacertificate is None:
+                print("TLS cannot be used as no CA Certificate specifed!")
+            else:
+                config["insecure"] = False
 
         if srv.hostname is None:
             print("No hostname or IP given")
             return
 
         config["ip"] = srv.hostname
 
@@ -616,18 +622,18 @@
             config["tls_server_name"] = self.tls_server_name
 
         self.commThread = KuksaClientThread(config)
         self.commThread.start()
 
         waitForConnection = threading.Condition()
         waitForConnection.acquire()
-        waitForConnection.wait_for(self.commThread.checkConnection, timeout=1)
+        waitForConnection.wait_for(self.commThread.connection_established, timeout=1)
         waitForConnection.release()
 
-        if self.commThread.checkConnection():
+        if self.commThread.connection_established():
             pass
         else:
             print(
                 "Error: Websocket could not be connected or the gRPC channel could not be created."
             )
             self.commThread.stop()
             self.commThread = None
@@ -635,64 +641,47 @@
     @with_category(COMM_SETUP_COMMANDS)
     @with_argparser(ap_connect)
     def do_connect(self, args):
         """Connect to a VSS server"""
         self.server = args.server
         self.connect()
 
-    def getDefaultTokenDir(self):
-        try:
-            return os.path.join(kuksa_server_certificates.__certificate_dir__, "jwt")
-        except AttributeError:
-            guessTokenDir = os.path.join(scriptDir, "kuksa_server_certificates/jwt")
-            if os.path.isdir(guessTokenDir):
-                return guessTokenDir
-            return "Unknown"
-
     @with_category(INFO_COMMANDS)
     def do_info(self, _args):
         """Show summary info of the client"""
         print("kuksa-client version " + _metadata.__version__)
         print("Uri: " + _metadata.__uri__)
         print("Author: " + _metadata.__author__)
         print("Copyright: " + _metadata.__copyright__)
-        print("Default tokens directory: " + self.getDefaultTokenDir())
 
     @with_category(INFO_COMMANDS)
     def do_version(self, _args):
         """Show version of the client"""
         print(_metadata.__version__)
 
-    @with_category(INFO_COMMANDS)
-    def do_printTokenDir(self, _args):
-        """Show default token directory"""
-        print(self.getDefaultTokenDir())
-
 
 # pylint: enable=too-many-public-methods
 # pylint: enable=too-many-instance-attributes
 
 # Main Function
 
-
 def main():
+
+    kuksa_logger = KuksaLogger()
+    kuksa_logger.init_logging()
+
     parser = argparse.ArgumentParser()
     parser.add_argument(
         "server",
         nargs="?",
         help=f"VSS server to connect to. Format: protocol://host[:port]. \
         Supported protocols: [grpc, grpcs, ws, wss]. Example: {DEFAULT_KUKSA_ADDRESS}",
         default=DEFAULT_KUKSA_ADDRESS,
     )
     parser.add_argument(
-        "--logging-config",
-        default=DEFAULT_LOGGING_CONFIG,
-        help="Path to logging configuration file",
-    )
-    parser.add_argument(
         "--token_or_tokenfile",
         default=DEFAULT_TOKEN_OR_TOKENFILE,
         help="JWT token or path to a JWT token file (.token)",
     )
 
     # Add TLS arguments
     # Note: Databroker does not yet support mutual authentication, so no need to use two first arguments
@@ -720,16 +709,14 @@
         "--tls-server-name",
         default=DEFAULT_TLS_SERVER_NAME,
         help="CA name of server, needed in some cases where subjectAltName does not suffice",
     )
 
     args = parser.parse_args()
 
-    logging.config.fileConfig(args.logging_config)
-
     clientApp = TestClient(
         args.server,
         token_or_tokenfile=args.token_or_tokenfile,
         certificate=args.certificate,
         keyfile=args.keyfile,
         cacertificate=args.cacertificate,
         tls_server_name=args.tls_server_name,
```

### Comparing `kuksa_client-0.4.2a1/kuksa_client/_metadata.py` & `kuksa_client-0.4.3a1/kuksa_client/_metadata.py`

 * *Files 14% similar despite different names*

```diff
@@ -14,14 +14,17 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 # SPDX-License-Identifier: Apache-2.0
 ########################################################################
 
+
+import logging
+
 __all__ = (
     "__title__",
     "__summary__",
     "__uri__",
     "__version__",
     "__author__",
     "__email__",
@@ -52,9 +55,9 @@
     __uri__ = metadata["home-page"]
     __version__ = metadata["version"]
     __author__ = metadata["author"]
     __email__ = metadata["author-email"]
     __license__ = metadata["license"]
 
 except importlib_metadata.PackageNotFoundError as e:
-    print(e)
-    print("skip configuring metadata")
+    logger = logging.getLogger(__name__)
+    logger.info("skip configuring metadata", e)
```

### Comparing `kuksa_client-0.4.2a1/kuksa_client/cli_backend/grpc.py` & `kuksa_client-0.4.3a1/kuksa_client/cli_backend/grpc.py`

 * *Files 10% similar despite different names*

```diff
@@ -24,25 +24,32 @@
 from typing import Any
 from typing import Callable
 from typing import Dict
 from typing import Iterable
 from typing import Optional
 import uuid
 import os
+import logging
 
 from kuksa_client import cli_backend
 import kuksa_client.grpc
 import kuksa_client.grpc.aio
 from kuksa_client.grpc import EntryUpdate
 from kuksa.val.v1 import types_pb2
 
 
+logger = logging.getLogger(__name__)
+
+
 def callback_wrapper(callback: Callable[[str], None]) -> Callable[[Iterable[EntryUpdate]], None]:
     def wrapper(updates: Iterable[EntryUpdate]) -> None:
-        callback(json.dumps([update.to_dict() for update in updates]))
+        try:
+            callback(json.dumps([update.to_dict() for update in updates], cls=DatabrokerEncoder))
+        except Exception as e:
+            logger.error("Callback could not be executed", e)
     return wrapper
 
 
 class DatabrokerEncoder(json.JSONEncoder):
     def default(self, obj):
         if isinstance(obj, (types_pb2.StringArray, types_pb2.BoolArray, types_pb2.Uint32Array, types_pb2.Uint64Array,
                             types_pb2.FloatArray, types_pb2.Int32Array, types_pb2.Int64Array, types_pb2.DoubleArray)):
@@ -53,48 +60,51 @@
             return {'values': string_values}
         return super().default(obj)
 
 
 class Backend(cli_backend.Backend):
     def __init__(self, config):
         super().__init__(config)
-        self.cacertificate = pathlib.Path(self.cacertificate)
-        self.keyfile = pathlib.Path(self.keyfile)
-        self.certificate = pathlib.Path(self.certificate)
+        if self.cacertificate is not None:
+            self.cacertificate = pathlib.Path(self.cacertificate)
+        if self.keyfile is not None:
+            self.keyfile = pathlib.Path(self.keyfile)
+        if self.certificate is not None:
+            self.certificate = pathlib.Path(self.certificate)
         if self.token_or_tokenfile is not None:
             if os.path.isfile(self.token_or_tokenfile):
                 self.token_or_tokenfile = pathlib.Path(self.token_or_tokenfile)
                 self.token = self.token_or_tokenfile.expanduser(
                 ).read_text(encoding='utf-8').rstrip('\n')
             else:
                 self.token = str(self.token_or_tokenfile)
         else:
             self.token = ""
-        self.grpcConnected = False
+        self.grpc_connection_established = False
 
         self.sendMsgQueue = queue.Queue()
         self.run = False
 
         self.AttrDict = {
             "value": (kuksa_client.grpc.Field.VALUE, kuksa_client.grpc.View.CURRENT_VALUE),
             "targetValue": (kuksa_client.grpc.Field.ACTUATOR_TARGET, kuksa_client.grpc.View.TARGET_VALUE),
             "metadata": (kuksa_client.grpc.Field.METADATA, kuksa_client.grpc.View.METADATA),
         }
 
-    # Function to check connection status
-    def checkConnection(self):
-        if self.grpcConnected:
-            return True
-        return False
+    def connection_established(self) -> bool:
+        """
+        Function to check connection status
+        """
+        return self.grpc_connection_established
 
     # Function to stop the communication
     def stop(self):
         self.disconnect()
         self.run = False
-        print("gRPC channel disconnected.")
+        logger.info("gRPC channel disconnected.")
 
     # Function to implement fetching of metadata
     def getMetaData(self, path: str, timeout=5):
         return self.getValue(path, "metadata", timeout)
 
     def updateMetaData(self, path: str, jsonStr, timeout=5):
         return self.setValue(path, jsonStr, "metadata", timeout)
@@ -211,18 +221,18 @@
                 respJson = "OK"
         except queue.Empty:
             respJson = json.dumps({"error": "Timeout"})
         return respJson
 
     # Async function to handle the gRPC calls
     async def _grpcHandler(self, vss_client: kuksa_client.grpc.aio.VSSClient):
-        self.grpcConnected = True
         self.run = True
         subscriber_manager = kuksa_client.grpc.aio.SubscriberManager(
             vss_client)
+        self.grpc_connection_established = True
         while self.run:
             try:
                 (call, requestArgs, responseQueue) = self.sendMsgQueue.get_nowait()
             except queue.Empty:
                 await asyncio.sleep(0.01)
                 continue
             try:
@@ -253,28 +263,32 @@
                 responseQueue.put((resp, None))
             except kuksa_client.grpc.VSSClientError as exc:
                 responseQueue.put((None, exc.to_dict()))
             except ValueError:
                 responseQueue.put(
                     (None, {"error": "ValueError in casting the value."}))
 
-        self.grpcConnected = False
+        self.grpc_connection_established = False
+
+    # Update VSS Tree Entry
+    def updateVSSTree(self, jsonStr, timeout=5):
+        logger.warning("Command not supported by KUKSA Databroker or KUKSA gRPC!")
 
     # Main loop for handling gRPC communication
     async def mainLoop(self):
         if self.insecure:
 
             async with kuksa_client.grpc.aio.VSSClient(self.serverIP, self.serverPort, token=self.token) as vss_client:
-                print("gRPC channel connected.")
+                logger.info("gRPC channel connected.")
                 await self._grpcHandler(vss_client)
         else:
             async with kuksa_client.grpc.aio.VSSClient(
                 self.serverIP,
                 self.serverPort,
                 root_certificates=self.cacertificate,
                 private_key=self.keyfile,
                 certificate_chain=self.certificate,
                 tls_server_name=self.tls_server_name,
                 token=self.token
             ) as vss_client:
-                print("Secure gRPC channel connected.")
+                logger.info("Secure gRPC channel connected.")
                 await self._grpcHandler(vss_client)
```

### Comparing `kuksa_client-0.4.2a1/kuksa_client/cli_backend/ws.py` & `kuksa_client-0.4.3a1/kuksa_client/cli_backend/ws.py`

 * *Files 9% similar despite different names*

```diff
@@ -22,24 +22,27 @@
 import json
 import os.path
 import pathlib
 import queue
 import ssl
 import time
 import uuid
+import logging
 
 import websockets
 
 from kuksa_client import cli_backend
 
+logger = logging.getLogger(__name__)
+
 
 class Backend(cli_backend.Backend):
     def __init__(self, config):
         super().__init__(config)
-        self.wsConnected = False
+        self.ws_connection_established = False
         self.subprotocol = None
         self.token = None
         self.subscriptionCallbacks = {}
         self.sendMsgQueue = queue.Queue()
         self.recvMsgQueues = {}
         self.run = False
 
@@ -54,29 +57,29 @@
                     del self.recvMsgQueues[resJson["requestId"]]
             else:
                 if "subscriptionId" in resJson and resJson["subscriptionId"] in self.subscriptionCallbacks:
                     try:
                         self.subscriptionCallbacks[resJson["subscriptionId"]](
                             message)
                     except Exception as e:  # pylint: disable=broad-except
-                        print(e)
+                        logger.warning("Receiver Handler exception", e)
 
     async def _sender_handler(self, webSocket):
         while self.run:
             try:
                 req = self.sendMsgQueue.get_nowait()
                 await webSocket.send(req)
             except queue.Empty:
                 await asyncio.sleep(0.01)
             except Exception as e:  # pylint: disable=broad-except
-                print(e)
+                logger.warning("Sender Handler exception", e)
                 return
 
     async def _msgHandler(self, webSocket):
-        self.wsConnected = True
+        self.ws_connection_established = True
         self.run = True
         recv = asyncio.Task(self._receiver_handler(webSocket))
         send = asyncio.Task(self._sender_handler(webSocket))
 
         await asyncio.wait([recv, send], return_when=asyncio.FIRST_COMPLETED)
         recv.cancel()
         send.cancel()
@@ -107,17 +110,17 @@
                 return json.dumps(resJson, indent=2)
         except queue.Empty:
             req["error"] = "timeout"
             return json.dumps(req, indent=2)
 
     # Function to stop the communication
     def stop(self):
-        self.wsConnected = False
+        self.ws_connection_established = False
         self.run = False
-        print("Server disconnected.")
+        logger.info("Server disconnected.")
 
     def disconnect(self, _):
         self.stop()
 
     # Function to authorize against the kuksa.val server
     def authorize(self, token_or_tokenfile=None, timeout=2):
         if token_or_tokenfile is None:
@@ -280,57 +283,59 @@
             errMsg["message"] = "Could not unsubscribe"
             errMsg["reason"] = "Subscription ID does not exist"
             res["error"] = errMsg
             res = json.dumps(res)
 
         return res
 
-    # Function to check connection
-    def checkConnection(self):
-        return self.wsConnected
+    def connection_established(self) -> bool:
+        """
+        Function to check connection
+        """
+        return self.ws_connection_established
 
     async def connect(self, _=None):
         subprotocols = ["VISSv2"]
         if not self.insecure:
             context = ssl.create_default_context()
             context.load_cert_chain(
                 certfile=self.certificate, keyfile=self.keyfile)
             context.load_verify_locations(cafile=self.cacertificate)
             # We want host name to match
             # For example certificates we use subjectAltName to make it match for Server, localahost and 127.0.0.1
             # If using your own certificates make sure that name is included or use tls_server_name work-around
             context.check_hostname = True
             try:
-                print("connect to wss://"+self.serverIP+":"+str(self.serverPort))
+                logger.info("connect to wss://"+self.serverIP+":"+str(self.serverPort))
                 args = {
                     "uri": "wss://"+self.serverIP+":"+str(self.serverPort),
                     "ssl": context,
                     "subprotocols": subprotocols,
                 }
                 # If your certificates does not contain the name of the server
                 # (for example during testing, in production it should match)
                 # then you can specify that checks should be against a different name
                 if self.tls_server_name:
                     args['server_hostname'] = self.tls_server_name
 
                 async with websockets.connect(**args) as ws:
                     self.subprotocol = ws.subprotocol
-                    print(f"Websocket connected. Negotiated subprotocol {self.subprotocol}")
+                    logger.info(f"Websocket connected. Negotiated subprotocol {self.subprotocol}")
                     await self._msgHandler(ws)
             except OSError as e:
-                print("Disconnected!! " + str(e))
+                logger.warning("Disconnected!!", e)
         else:
             try:
                 uri = "ws://"+self.serverIP+":"+str(self.serverPort)
-                print(f"connect to {uri}")
+                logger.info("connect to %s", uri)
                 async with websockets.connect(uri, subprotocols=subprotocols) as ws:
                     self.subprotocol = ws.subprotocol
                     if self.subprotocol == "VISSv2":
-                        print("subprotocol matches condition")
-                    print(f"Websocket connected. Negotiated subprotocol {self.subprotocol}")
+                        logger.info("subprotocol matches condition")
+                    logger.info("Websocket connected. Negotiated subprotocol %s", self.subprotocol)
                     await self._msgHandler(ws)
             except OSError as e:
-                print("Disconnected!! " + str(e))
+                logger.warning("Disconnected!!", e)
 
     # Main loop for handling websocket communication
     async def mainLoop(self):
         await self.connect()
```

### Comparing `kuksa_client-0.4.2a1/kuksa_client/grpc/__init__.py` & `kuksa_client-0.4.3a1/kuksa_client/grpc/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,19 +12,19 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 # SPDX-License-Identifier: Apache-2.0
 ########################################################################
 
+from __future__ import absolute_import
 import contextlib
 import dataclasses
 import datetime
 import enum
-import http
 import logging
 import re
 from typing import Any
 from typing import Collection
 from typing import Dict
 from typing import Iterable
 from typing import Iterator
@@ -160,28 +160,37 @@
     def from_message(cls, message: types_pb2.Metadata):
         metadata = cls(data_type=DataType(message.data_type),
                        entry_type=EntryType(message.entry_type))
         for field in ('description', 'comment', 'deprecation', 'unit'):
             if message.HasField(field):
                 setattr(metadata, field, getattr(message, field))
         if message.HasField('value_restriction'):
-            value_restriction = getattr(
-                message.value_restriction, message.value_restriction.WhichOneof('type'))
-            metadata.value_restriction = ValueRestriction()
-            for field in ('min', 'max'):
-                if value_restriction.HasField(field):
-                    setattr(metadata.value_restriction, field,
-                            getattr(value_restriction, field))
-            if value_restriction.allowed_values:
-                metadata.value_restriction.allowed_values = list(
-                    value_restriction.allowed_values)
+            restriction_type = message.value_restriction.WhichOneof('type')
+            # Make sure that a type actually is set
+            if restriction_type:
+                value_restriction = getattr(
+                    message.value_restriction, restriction_type)
+                metadata.value_restriction = ValueRestriction()
+                # All types except string support min/max
+                if restriction_type != 'string':
+                    for field in ('min', 'max'):
+                        if value_restriction.HasField(field):
+                            setattr(metadata.value_restriction, field,
+                                    getattr(value_restriction, field))
+                if value_restriction.allowed_values:
+                    metadata.value_restriction.allowed_values = list(
+                        value_restriction.allowed_values)
         return metadata
 
     # pylint: disable=too-many-branches
     def to_message(self, value_type: DataType = DataType.UNSPECIFIED) -> types_pb2.Metadata:
+        """
+        to_message/from_message aligned to use None rather than empty list for
+        representing allowed values in value restrictions
+        """
         message = types_pb2.Metadata(
             data_type=self.data_type.value, entry_type=self.entry_type.value)
         for field in ('description', 'comment', 'deprecation', 'unit'):
             field_value = getattr(self, field, None)
             if field_value is not None:
                 setattr(message, field, field_value)
         if self.value_restriction is not None:
@@ -197,15 +206,15 @@
             ):
                 if self.value_restriction.min is not None:
                     message.value_restriction.signed.min = int(
                         self.value_restriction.min)
                 if self.value_restriction.max is not None:
                     message.value_restriction.signed.max = int(
                         self.value_restriction.max)
-                if self.value_restriction.allowed_values is not None:
+                if self.value_restriction.allowed_values:
                     message.value_restriction.signed.allowed_values.extend(
                         (int(value)
                          for value in self.value_restriction.allowed_values),
                     )
             elif value_type in (
                 DataType.UINT8,
                 DataType.UINT16,
@@ -218,15 +227,15 @@
             ):
                 if self.value_restriction.min is not None:
                     message.value_restriction.unsigned.min = int(
                         self.value_restriction.min)
                 if self.value_restriction.max is not None:
                     message.value_restriction.unsigned.max = int(
                         self.value_restriction.max)
-                if self.value_restriction.allowed_values is not None:
+                if self.value_restriction.allowed_values:
                     message.value_restriction.unsigned.allowed_values.extend(
                         (int(value)
                          for value in self.value_restriction.allowed_values),
                     )
             elif value_type in (
                 DataType.FLOAT,
                 DataType.DOUBLE,
@@ -235,24 +244,24 @@
             ):
                 if self.value_restriction.min is not None:
                     message.value_restriction.floating_point.min = float(
                         self.value_restriction.min)
                 if self.value_restriction.max is not None:
                     message.value_restriction.floating_point.max = float(
                         self.value_restriction.max)
-                if self.value_restriction.allowed_values is not None:
+                if self.value_restriction.allowed_values:
                     message.value_restriction.floating_point.allowed_values.extend(
                         (float(value)
                          for value in self.value_restriction.allowed_values),
                     )
             elif value_type in (
                 DataType.STRING,
                 DataType.STRING_ARRAY,
             ):
-                if self.value_restriction.allowed_values is not None:
+                if self.value_restriction.allowed_values:
                     message.value_restriction.string.allowed_values.extend(
                         (str(value)
                          for value in self.value_restriction.allowed_values),
                     )
             else:
                 raise ValueError(
                     f"Cannot set value_restriction from data type {value_type.name}")
@@ -304,19 +313,40 @@
 @dataclasses.dataclass
 class Datapoint:
     value: Optional[Any] = None
     timestamp: Optional[datetime.datetime] = None
 
     @classmethod
     def from_message(cls, message: types_pb2.Datapoint):
+        """
+        Return internal Datapoint representation or None on error
+        """
+        if message.WhichOneof('value') is None:
+            logger.warning("No value provided in datapoint!")
+            return None
+
+        if message.HasField('timestamp'):
+            # gRPC timestamp supports date up to including year 9999
+            # If timestamp by any reason contains a larger number for seconds than supported
+            # you may get an overflow error
+            try:
+                timestamp = message.timestamp.ToDatetime(
+                            tzinfo=datetime.timezone.utc,
+                            )
+            except ValueError:
+
+                logger.error("Timestamp %d out of accepted range, value ignored!",
+                             message.timestamp.seconds)
+                return None
+        else:
+            timestamp = None
+
         return cls(
             value=getattr(message, message.WhichOneof('value')),
-            timestamp=message.timestamp.ToDatetime(
-                tzinfo=datetime.timezone.utc,
-            ) if message.HasField('timestamp') else None,
+            timestamp=timestamp,
         )
 
     def cast_array_values(cast, array):
         """
         Parses array input and cast individual values to wanted type.
         Note that input value to this function is not the same as given if you use kuksa-client command line
         as parts (e.g. surrounding quotes) are removed by shell, and then do_setValue also do some magic.
@@ -631,17 +661,29 @@
         else:
             error = {}
         if response.errors:
             errors = [json_format.MessageToDict(
                 err, preserving_proto_field_name=True) for err in response.errors]
         else:
             errors = []
-        if (error and error['code'] is not http.HTTPStatus.OK) or any(
-            sub_error['error']['code'] is not http.HTTPStatus.OK for sub_error in errors
-        ):
+
+        raise_error = False
+        if (error and error.get('code') != 200):
+            raise_error = True
+        else:
+            for sub_error in errors:
+                if 'error' in sub_error:
+                    if sub_error['error'].get('code') != 200:
+                        logger.debug("Sub-error %d but no top level error", sub_error['error'].get('code'))
+                        raise_error = True
+                else:
+                    logger.error("No error field for sub-error")
+                    raise_error = True
+
+        if raise_error:
             raise VSSClientError(error, errors)
 
     def get_authorization_header(self, token: str):
         if token is None:
             return None
         return "Bearer " + token
```

### Comparing `kuksa_client-0.4.2a1/kuksa_client/grpc/aio.py` & `kuksa_client-0.4.3a1/kuksa_client/grpc/aio.py`

 * *Files identical despite different names*

### Comparing `kuksa_client-0.4.2a1/kuksa_client/logo` & `kuksa_client-0.4.3a1/kuksa_client/logo`

 * *Files identical despite different names*

### Comparing `kuksa_client-0.4.2a1/kuksa_client/ws/__init__.py` & `kuksa_client-0.4.3a1/kuksa_client/ws/__init__.py`

 * *Files identical despite different names*

### Comparing `kuksa_client-0.4.2a1/kuksa_client.egg-info/PKG-INFO` & `kuksa_client-0.4.3a1/kuksa_client.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: kuksa-client
-Version: 0.4.2a1
+Name: kuksa_client
+Version: 0.4.3a1
 Summary: KUKSA Python Client and SDK
 Home-page: https://github.com/eclipse-kuksa/kuksa-python-sdk
 Author: Eclipse KUKSA Project
 Author-email: kuksa-dev@eclipse.org
 Project-URL: Source, https://github.com/eclipse-kuksa/kuksa-python-sdk
 Project-URL: Bug Tracker, https://github.com/eclipse-kuksa/kuksa-python-sdk/issues
 Classifier: Intended Audience :: Developers
@@ -16,33 +16,26 @@
 Classifier: Topic :: Software Development
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: websockets>=10.1
 Requires-Dist: cmd2<2.0,>=1.4
 Requires-Dist: pygments>=2.15
-Requires-Dist: grpcio-tools>=1.54.2
+Requires-Dist: grpcio-tools>=1.63.0
 Requires-Dist: jsonpath-ng>=1.5.3
 Provides-Extra: test
 Requires-Dist: pylint; extra == "test"
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: pytest-asyncio; extra == "test"
 Requires-Dist: pytest-cov; extra == "test"
 Requires-Dist: pytest-mock; extra == "test"
 Requires-Dist: pytest-timeout; extra == "test"
 
 # KUKSA Python SDK
-![kuksa.val Logo](https://github.com/eclipse-kuksa/kuksa-python-sdk/blob/main/docs/pictures/logo.png)
-
-
-**Note: The KUKSA project is currently in the process of moving the KUKSA Python SDK (kuksa-client)**
-**from the [kuksa.val](https://github.com/eclipse/kuksa.val/tree/master/kuksa-client) repository**
-**to this repository. This repository is still in *draft* status!**
-**Use kuksa.val for development, pull requests and issues until kuksa-client has been removed**
-**from that repository!**
+![kuksa.val Logo](https://raw.githubusercontent.com/eclipse-kuksa/kuksa-python-sdk/main/docs/pictures/logo.png)
 
 KUKSA Python Client and SDK is a part of the open source project [Eclipse KUKSA](https://www.eclipse.org/kuksa/).
 More about Eclipse KUKSA can be found in the [repository](https://github.com/eclipse/kuksa.val).
 
 ## Introduction
 
 KUKSA Python SDK provides both a command-line interface (CLI) and a standalone library to interact with either
```

### Comparing `kuksa_client-0.4.2a1/pyproject.toml` & `kuksa_client-0.4.3a1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [build-system]
 requires = [
-    "grpcio-tools>=1.54.2",
+    "grpcio-tools>=1.63.0",
     "setuptools>=42",
     "setuptools-git-versioning",
     "wheel",
 ]
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools-git-versioning]
```

### Comparing `kuksa_client-0.4.2a1/setup.cfg` & `kuksa_client-0.4.3a1/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 [options]
 python_requires = >=3.8
 install_requires = 
 	websockets >= 10.1
 	cmd2 >= 1.4, <2.0
 	pygments >= 2.15
-	grpcio-tools >= 1.54.2
+	grpcio-tools >= 1.63.0
 	jsonpath-ng >= 1.5.3
 packages = find:
 
 [options.extras_require]
 test = 
 	pylint
 	pytest
@@ -39,16 +39,14 @@
 	pytest-mock
 	pytest-timeout
 
 [options.package_data]
 kuksa_client = 
 	logging.ini
 	logo
-	kuksa_server_certificates/*
-	kuksa_server_certificates/jwt/*
 
 [options.packages.find]
 where = .
 
 [options.entry_points]
 console_scripts = 
 	kuksa-client = kuksa_client.__main__:main
```

### Comparing `kuksa_client-0.4.2a1/setup.py` & `kuksa_client-0.4.3a1/setup.py`

 * *Files identical despite different names*

### Comparing `kuksa_client-0.4.2a1/tests/__init__.py` & `kuksa_client-0.4.3a1/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `kuksa_client-0.4.2a1/tests/conftest.py` & `kuksa_client-0.4.3a1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `kuksa_client-0.4.2a1/tests/test_datapoint.py` & `kuksa_client-0.4.3a1/tests/test_datapoint.py`

 * *Files 24% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 # * http://www.apache.org/licenses/LICENSE-2.0
 # *
 # * SPDX-License-Identifier: Apache-2.0
 # ********************************************************************************/
 
 import pytest
 from kuksa_client.grpc import Datapoint
+from kuksa.val.v1 import types_pb2
+from google.protobuf import timestamp_pb2
 
 #
 # Client rules:
 # For simple strings like abd it is optional to quote them ("abc") or not (abc)
 # Quotes are needed if you have commas ("ab, c")
 # If you have duoble quotes in strings you must escape them
 #
@@ -119,15 +121,15 @@
     assert my_array[0] == "dtc1, dtc2"
     assert my_array[1] == "dtc3"
     assert my_array[2] == "\" dtc4"
     assert my_array[3] == "dtc4\""
 
 
 def test_quotes_in_string_values_2():
-    """Doubee quotes in double quotes so in total three values"""
+    """Double quotes in double quotes so in total three values"""
     test_str = "['dtc1, dtc2', dtc3, \" dtc4, dtc4\"]"
     my_array = list(Datapoint.cast_array_values(Datapoint.cast_str, test_str))
     assert len(my_array) == 3
     assert my_array[0] == 'dtc1, dtc2'
     assert my_array[1] == "dtc3"
     assert my_array[2] == " dtc4, dtc4"
 
@@ -175,7 +177,50 @@
     assert Datapoint.cast_bool("F") is False
     assert Datapoint.cast_bool("f") is False
 
     # And then some other, treated as true for now
     assert Datapoint.cast_bool("Ja") is True
     assert Datapoint.cast_bool("Nein") is True
     assert Datapoint.cast_bool("Doch") is True
+
+
+def test_from_message_none():
+    """
+    There shall always be a value
+    """
+    msg = types_pb2.Datapoint()
+    datapoint = Datapoint.from_message(msg)
+    assert datapoint is None
+
+
+def test_from_message_uint32():
+    msg = types_pb2.Datapoint(uint32=456)
+    datapoint = Datapoint.from_message(msg)
+    assert datapoint.value == 456
+
+
+def test_from_message_time():
+    """
+    Make sure that we can handle values out of range (by discarding them)
+    gRPC supports year up to including 9999, so any date in year 10000 or later shall
+    result in that None is returned
+    """
+    # Wed Jan 17 2024 10:02:27 GMT+0000
+    timestamp = timestamp_pb2.Timestamp(seconds=1705485747)
+    msg = types_pb2.Datapoint(uint32=456, timestamp=timestamp)
+    datapoint = Datapoint.from_message(msg)
+    assert datapoint.timestamp.year == 2024
+
+    # Thu Dec 30 9999 07:13:22 GMT+0000
+    timestamp = timestamp_pb2.Timestamp(seconds=253402154002)
+    msg = types_pb2.Datapoint(uint32=456, timestamp=timestamp)
+    datapoint = Datapoint.from_message(msg)
+    assert datapoint.timestamp.year == 9999
+
+    # Sat Jan 29 10000 07:13:22 GMT+0000
+    # Currently the constructors does not check range
+    timestamp = timestamp_pb2.Timestamp(seconds=253404746002)
+    msg = types_pb2.Datapoint(uint32=456, timestamp=timestamp)
+
+    # But the from_message method handle the checks
+    datapoint = Datapoint.from_message(msg)
+    assert datapoint is None
```

### Comparing `kuksa_client-0.4.2a1/tests/test_grpc.py` & `kuksa_client-0.4.3a1/tests/test_grpc.py`

 * *Files 3% similar despite different names*

```diff
@@ -115,25 +115,37 @@
         (0, None, None),
         (-42, None, None),
         (None, 0, None),
         (None, 42, None),
         (None, None, [-42, 0, 42]),
         (-42, 42, [-42, 0, 42]),
     ])
-    def test_to_message_signed_value_restriction(self, value_type, min_value, max_value, allowed_values):
+    def test_to_from_message_signed_value_restriction(self, value_type, min_value, max_value, allowed_values):
+
+        input_metadata = Metadata(value_restriction=ValueRestriction(
+                            min=min_value, max=max_value, allowed_values=allowed_values,
+                            ))
+
+        if not allowed_values:
+            # Empty array treated as None by KUKSA Metadata class
+            allowed_values = None
+
         if (min_value, max_value, allowed_values) == (None, None, None):
             expected_message = types_pb2.Metadata()
+            output_metadata = Metadata()
         else:
             expected_message = types_pb2.Metadata(value_restriction=types_pb2.ValueRestriction(
                 signed=types_pb2.ValueRestrictionInt(
                     min=min_value, max=max_value, allowed_values=allowed_values),
             ))
-        assert Metadata(value_restriction=ValueRestriction(
-            min=min_value, max=max_value, allowed_values=allowed_values,
-        )).to_message(value_type) == expected_message
+            output_metadata = Metadata(value_restriction=ValueRestriction(
+                                min=min_value, max=max_value, allowed_values=allowed_values,
+                                ))
+        assert input_metadata.to_message(value_type) == expected_message
+        assert Metadata.from_message(expected_message) == output_metadata
 
     @pytest.mark.parametrize('value_type', (
         DataType.UINT8,
         DataType.UINT16,
         DataType.UINT32,
         DataType.UINT64,
         DataType.UINT8_ARRAY,
@@ -146,25 +158,38 @@
         (None, None, []),
         (0, None, None),
         (None, 0, None),
         (None, 42, None),
         (None, None, [0, 12, 42]),
         (0, 42, [0, 12, 42]),
     ])
-    def test_to_message_unsigned_value_restriction(self, value_type, min_value, max_value, allowed_values):
+    def test_to_from_message_unsigned_value_restriction(self, value_type, min_value, max_value, allowed_values):
+
+        input_metadata = Metadata(value_restriction=ValueRestriction(
+                            min=min_value, max=max_value, allowed_values=allowed_values,
+                            ))
+
+        if not allowed_values:
+            # Empty array treated as None by KUKSA Metadata class
+            allowed_values = None
+
         if (min_value, max_value, allowed_values) == (None, None, None):
             expected_message = types_pb2.Metadata()
+            output_metadata = Metadata()
         else:
             expected_message = types_pb2.Metadata(value_restriction=types_pb2.ValueRestriction(
                 unsigned=types_pb2.ValueRestrictionUint(
                     min=min_value, max=max_value, allowed_values=allowed_values),
             ))
-        assert Metadata(value_restriction=ValueRestriction(
-            min=min_value, max=max_value, allowed_values=allowed_values,
-        )).to_message(value_type) == expected_message
+            output_metadata = Metadata(value_restriction=ValueRestriction(
+                                min=min_value, max=max_value, allowed_values=allowed_values,
+                                ))
+
+        assert input_metadata.to_message(value_type) == expected_message
+        assert Metadata.from_message(expected_message) == output_metadata
 
     @pytest.mark.parametrize('value_type', (
         DataType.FLOAT,
         DataType.DOUBLE,
         DataType.FLOAT_ARRAY,
         DataType.DOUBLE_ARRAY,
     ))
@@ -174,39 +199,74 @@
         (0, None, None),
         (0.5, None, None),
         (None, 0, None),
         (None, 41.5, None),
         (None, None, [0.5, 12., 41.5]),
         (0.5, 41.5, [0.5, 12., 41.5]),
     ])
-    def test_to_message_float_value_restriction(self, value_type, min_value, max_value, allowed_values):
+    def test_to_from_message_float_value_restriction(self, value_type, min_value, max_value, allowed_values):
+
+        input_metadata = Metadata(value_restriction=ValueRestriction(
+                            min=min_value, max=max_value, allowed_values=allowed_values,
+                            ))
+
+        if not allowed_values:
+            # Empty array treated as None by KUKSA Metadata class
+            allowed_values = None
+
         if (min_value, max_value, allowed_values) == (None, None, None):
             expected_message = types_pb2.Metadata()
+            output_metadata = Metadata()
         else:
             expected_message = types_pb2.Metadata(value_restriction=types_pb2.ValueRestriction(
                 floating_point=types_pb2.ValueRestrictionFloat(
                     min=min_value, max=max_value, allowed_values=allowed_values),
             ))
-        assert Metadata(value_restriction=ValueRestriction(
-            min=min_value, max=max_value, allowed_values=allowed_values,
-        )).to_message(value_type) == expected_message
+            output_metadata = Metadata(value_restriction=ValueRestriction(
+                                min=min_value, max=max_value, allowed_values=allowed_values,
+                                ))
+
+        assert input_metadata.to_message(value_type) == expected_message
+        assert Metadata.from_message(expected_message) == output_metadata
 
     @pytest.mark.parametrize('value_type', (DataType.STRING, DataType.STRING_ARRAY))
     @pytest.mark.parametrize('allowed_values', [None, [], ['Hello', 'world']])
-    def test_to_message_string_value_restriction(self, value_type, allowed_values):
+    def test_to_from_message_string_value_restriction(self, value_type, allowed_values):
+
+        input_metadata = Metadata(value_restriction=ValueRestriction(
+                            allowed_values=allowed_values,
+                            ))
+
+        if not allowed_values:
+            # Empty array treated as None by KUKSA Metadata class
+            allowed_values = None
+
         if allowed_values is None:
             expected_message = types_pb2.Metadata()
+            output_metadata = Metadata()
         else:
             expected_message = types_pb2.Metadata(value_restriction=types_pb2.ValueRestriction(
                 string=types_pb2.ValueRestrictionString(
                     allowed_values=allowed_values),
             ))
-        assert Metadata(value_restriction=ValueRestriction(
-            allowed_values=allowed_values,
-        )).to_message(value_type) == expected_message
+            output_metadata = Metadata(value_restriction=ValueRestriction(
+                            allowed_values=allowed_values,
+                            ))
+
+        assert input_metadata.to_message(value_type) == expected_message
+        assert Metadata.from_message(expected_message) == output_metadata
+
+    def test_metadata_from_message_value_restriction_no_type(self):
+        """
+        This intends to cover the case when the proto message has a value restriction, but
+        no contents (type not specified)
+        """
+        input_message = types_pb2.Metadata(value_restriction=types_pb2.ValueRestriction())
+        expected_metadata = Metadata()
+        assert Metadata.from_message(input_message) == expected_metadata
 
     @pytest.mark.parametrize('metadata_dict, init_kwargs', [
         ({}, {}),
         ({'entry_type': 1}, {'entry_type': EntryType.ATTRIBUTE}),
         ({'entry_type': EntryType.ATTRIBUTE},
          {'entry_type': EntryType.ATTRIBUTE}),
         ({'entry_type': 'ATTRIBUTE'}, {'entry_type': EntryType.ATTRIBUTE}),
```

