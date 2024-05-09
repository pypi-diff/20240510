# Comparing `tmp/flet_contrib_runtime-2024.5.3.1625.tar.gz` & `tmp/flet_contrib_runtime-2024.5.9.2200.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flet_contrib_runtime-2024.5.3.1625.tar", max compression
+gzip compressed data, was "flet_contrib_runtime-2024.5.9.2200.tar", max compression
```

## Comparing `flet_contrib_runtime-2024.5.3.1625.tar` & `flet_contrib_runtime-2024.5.9.2200.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0      204 2024-05-03 16:24:44.694319 flet_contrib_runtime-2024.5.3.1625/README.md
--rw-r--r--   0        0        0      702 2024-05-03 16:25:38.426629 flet_contrib_runtime-2024.5.3.1625/pyproject.toml
--rw-r--r--   0        0        0      242 2024-05-03 16:24:44.698319 flet_contrib_runtime-2024.5.3.1625/src/flet_runtime/__init__.py
--rw-r--r--   0        0        0    15946 2024-05-03 16:24:44.698319 flet_contrib_runtime-2024.5.3.1625/src/flet_runtime/app.py
--rw-r--r--   0        0        0      252 2024-05-03 16:24:44.698319 flet_contrib_runtime-2024.5.3.1625/src/flet_runtime/auth/__init__.py
--rw-r--r--   0        0        0      500 2024-05-03 16:24:44.698319 flet_contrib_runtime-2024.5.3.1625/src/flet_runtime/auth/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     8691 2024-05-03 16:24:44.698319 flet_contrib_runtime-2024.5.3.1625/src/flet_runtime/auth/__pycache__/authorization.cpython-39.pyc
--rw-r--r--   0        0        0      567 2024-05-03 16:24:44.698319 flet_contrib_runtime-2024.5.3.1625/src/flet_runtime/auth/__pycache__/group.cpython-39.pyc
--rw-r--r--   0        0        0     2073 2024-05-03 16:24:44.698319 flet_contrib_runtime-2024.5.3.1625/src/flet_runtime/auth/__pycache__/oauth_provider.cpython-39.pyc
--rw-r--r--   0        0        0     1271 2024-05-03 16:24:44.698319 flet_contrib_runtime-2024.5.3.1625/src/flet_runtime/auth/__pycache__/oauth_token.cpython-39.pyc
--rw-r--r--   0        0        0      578 2024-05-03 16:24:44.698319 flet_contrib_runtime-2024.5.3.1625/src/flet_runtime/auth/__pycache__/user.cpython-39.pyc
--rw-r--r--   0        0        0     9278 2024-05-03 16:24:44.698319 flet_contrib_runtime-2024.5.3.1625/src/flet_runtime/auth/authorization.py
--rw-r--r--   0        0        0      128 2024-05-03 16:24:44.698319 flet_contrib_runtime-2024.5.3.1625/src/flet_runtime/auth/group.py
--rw-r--r--   0        0        0     1806 2024-05-03 16:24:44.698319 flet_contrib_runtime-2024.5.3.1625/src/flet_runtime/auth/oauth_provider.py
--rw-r--r--   0        0        0      847 2024-05-03 16:24:44.698319 flet_contrib_runtime-2024.5.3.1625/src/flet_runtime/auth/oauth_token.py
--rw-r--r--   0        0        0      324 2024-05-03 16:24:44.698319 flet_contrib_runtime-2024.5.3.1625/src/flet_runtime/auth/providers/__init__.py
--rw-r--r--   0        0        0      743 2024-05-03 16:24:44.698319 flet_contrib_runtime-2024.5.3.1625/src/flet_runtime/auth/providers/auth0_oauth_provider.py
--rw-r--r--   0        0        0      848 2024-05-03 16:24:44.698319 flet_contrib_runtime-2024.5.3.1625/src/flet_runtime/auth/providers/azure_oauth_provider.py
--rw-r--r--   0        0        0     3683 2024-05-03 16:24:44.698319 flet_contrib_runtime-2024.5.3.1625/src/flet_runtime/auth/providers/github_oauth_provider.py
--rw-r--r--   0        0        0      807 2024-05-03 16:24:44.698319 flet_contrib_runtime-2024.5.3.1625/src/flet_runtime/auth/providers/google_oauth_provider.py
--rw-r--r--   0        0        0      146 2024-05-03 16:24:44.698319 flet_contrib_runtime-2024.5.3.1625/src/flet_runtime/auth/user.py
--rw-r--r--   0        0        0     7402 2024-05-03 16:24:44.698319 flet_contrib_runtime-2024.5.3.1625/src/flet_runtime/flet_socket_server.py
--rw-r--r--   0        0        0     2163 2024-05-03 16:24:44.698319 flet_contrib_runtime-2024.5.3.1625/src/flet_runtime/security/__init__.py
--rw-r--r--   0        0        0     1587 2024-05-03 16:24:44.698319 flet_contrib_runtime-2024.5.3.1625/src/flet_runtime/uploads.py
--rw-r--r--   0        0        0     4787 2024-05-03 16:24:44.698319 flet_contrib_runtime-2024.5.3.1625/src/flet_runtime/utils/__init__.py
--rw-r--r--   0        0        0     6025 2024-05-03 16:24:44.698319 flet_contrib_runtime-2024.5.3.1625/src/flet_runtime/utils/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0      750 2024-05-03 16:24:44.698319 flet_contrib_runtime-2024.5.3.1625/src/flet_runtime/utils/__pycache__/once.cpython-39.pyc
--rw-r--r--   0        0        0     2726 2024-05-03 16:24:44.698319 flet_contrib_runtime-2024.5.3.1625/src/flet_runtime/utils/__pycache__/patch_index.cpython-39.pyc
--rw-r--r--   0        0        0      347 2024-05-03 16:24:44.698319 flet_contrib_runtime-2024.5.3.1625/src/flet_runtime/utils/once.py
--rw-r--r--   0        0        0     3202 2024-05-03 16:24:44.698319 flet_contrib_runtime-2024.5.3.1625/src/flet_runtime/utils/patch_index.py
--rw-r--r--   0        0        0      103 2024-05-03 16:24:44.698319 flet_contrib_runtime-2024.5.3.1625/src/flet_runtime/version.py
--rw-r--r--   0        0        0     1134 1970-01-01 00:00:00.000000 flet_contrib_runtime-2024.5.3.1625/PKG-INFO
+-rw-r--r--   0        0        0      204 2024-05-09 22:00:05.022540 flet_contrib_runtime-2024.5.9.2200/README.md
+-rw-r--r--   0        0        0      702 2024-05-09 22:00:53.915442 flet_contrib_runtime-2024.5.9.2200/pyproject.toml
+-rw-r--r--   0        0        0      242 2024-05-09 22:00:05.022540 flet_contrib_runtime-2024.5.9.2200/src/flet_runtime/__init__.py
+-rw-r--r--   0        0        0    15946 2024-05-09 22:00:05.022540 flet_contrib_runtime-2024.5.9.2200/src/flet_runtime/app.py
+-rw-r--r--   0        0        0      252 2024-05-09 22:00:05.022540 flet_contrib_runtime-2024.5.9.2200/src/flet_runtime/auth/__init__.py
+-rw-r--r--   0        0        0      500 2024-05-09 22:00:05.022540 flet_contrib_runtime-2024.5.9.2200/src/flet_runtime/auth/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     8691 2024-05-09 22:00:05.022540 flet_contrib_runtime-2024.5.9.2200/src/flet_runtime/auth/__pycache__/authorization.cpython-39.pyc
+-rw-r--r--   0        0        0      567 2024-05-09 22:00:05.022540 flet_contrib_runtime-2024.5.9.2200/src/flet_runtime/auth/__pycache__/group.cpython-39.pyc
+-rw-r--r--   0        0        0     2073 2024-05-09 22:00:05.022540 flet_contrib_runtime-2024.5.9.2200/src/flet_runtime/auth/__pycache__/oauth_provider.cpython-39.pyc
+-rw-r--r--   0        0        0     1271 2024-05-09 22:00:05.022540 flet_contrib_runtime-2024.5.9.2200/src/flet_runtime/auth/__pycache__/oauth_token.cpython-39.pyc
+-rw-r--r--   0        0        0      578 2024-05-09 22:00:05.022540 flet_contrib_runtime-2024.5.9.2200/src/flet_runtime/auth/__pycache__/user.cpython-39.pyc
+-rw-r--r--   0        0        0     9278 2024-05-09 22:00:05.022540 flet_contrib_runtime-2024.5.9.2200/src/flet_runtime/auth/authorization.py
+-rw-r--r--   0        0        0      128 2024-05-09 22:00:05.022540 flet_contrib_runtime-2024.5.9.2200/src/flet_runtime/auth/group.py
+-rw-r--r--   0        0        0     1806 2024-05-09 22:00:05.022540 flet_contrib_runtime-2024.5.9.2200/src/flet_runtime/auth/oauth_provider.py
+-rw-r--r--   0        0        0      847 2024-05-09 22:00:05.022540 flet_contrib_runtime-2024.5.9.2200/src/flet_runtime/auth/oauth_token.py
+-rw-r--r--   0        0        0      324 2024-05-09 22:00:05.022540 flet_contrib_runtime-2024.5.9.2200/src/flet_runtime/auth/providers/__init__.py
+-rw-r--r--   0        0        0      743 2024-05-09 22:00:05.022540 flet_contrib_runtime-2024.5.9.2200/src/flet_runtime/auth/providers/auth0_oauth_provider.py
+-rw-r--r--   0        0        0      848 2024-05-09 22:00:05.022540 flet_contrib_runtime-2024.5.9.2200/src/flet_runtime/auth/providers/azure_oauth_provider.py
+-rw-r--r--   0        0        0     3683 2024-05-09 22:00:05.022540 flet_contrib_runtime-2024.5.9.2200/src/flet_runtime/auth/providers/github_oauth_provider.py
+-rw-r--r--   0        0        0      807 2024-05-09 22:00:05.022540 flet_contrib_runtime-2024.5.9.2200/src/flet_runtime/auth/providers/google_oauth_provider.py
+-rw-r--r--   0        0        0      146 2024-05-09 22:00:05.022540 flet_contrib_runtime-2024.5.9.2200/src/flet_runtime/auth/user.py
+-rw-r--r--   0        0        0     7402 2024-05-09 22:00:05.022540 flet_contrib_runtime-2024.5.9.2200/src/flet_runtime/flet_socket_server.py
+-rw-r--r--   0        0        0     2163 2024-05-09 22:00:05.026541 flet_contrib_runtime-2024.5.9.2200/src/flet_runtime/security/__init__.py
+-rw-r--r--   0        0        0     1587 2024-05-09 22:00:05.026541 flet_contrib_runtime-2024.5.9.2200/src/flet_runtime/uploads.py
+-rw-r--r--   0        0        0     4787 2024-05-09 22:00:05.026541 flet_contrib_runtime-2024.5.9.2200/src/flet_runtime/utils/__init__.py
+-rw-r--r--   0        0        0     6025 2024-05-09 22:00:05.026541 flet_contrib_runtime-2024.5.9.2200/src/flet_runtime/utils/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0      750 2024-05-09 22:00:05.026541 flet_contrib_runtime-2024.5.9.2200/src/flet_runtime/utils/__pycache__/once.cpython-39.pyc
+-rw-r--r--   0        0        0     2726 2024-05-09 22:00:05.026541 flet_contrib_runtime-2024.5.9.2200/src/flet_runtime/utils/__pycache__/patch_index.cpython-39.pyc
+-rw-r--r--   0        0        0      347 2024-05-09 22:00:05.026541 flet_contrib_runtime-2024.5.9.2200/src/flet_runtime/utils/once.py
+-rw-r--r--   0        0        0     3202 2024-05-09 22:00:05.026541 flet_contrib_runtime-2024.5.9.2200/src/flet_runtime/utils/patch_index.py
+-rw-r--r--   0        0        0      103 2024-05-09 22:00:05.026541 flet_contrib_runtime-2024.5.9.2200/src/flet_runtime/version.py
+-rw-r--r--   0        0        0     1134 1970-01-01 00:00:00.000000 flet_contrib_runtime-2024.5.9.2200/PKG-INFO
```

### Comparing `flet_contrib_runtime-2024.5.3.1625/pyproject.toml` & `flet_contrib_runtime-2024.5.9.2200/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "flet-contrib-runtime"
-version = "2024.05.03.1625"
+version = "2024.05.09.2200"
 description = "Flet Runtime - a base package for Flet desktop and Flet mobile."
 authors = ["Appveyor Systems Inc. <hello@flet.dev>"]
 license = "Apache-2.0"
 readme = "README.md"
 
 packages = [
     { include = "flet_runtime", from = "src" },
@@ -13,15 +13,15 @@
 [tool.poetry.urls]
 homepage = "https://flet.dev"
 repository = "https://github.com/flet-dev/flet"
 documentation = "https://flet.dev/docs"
 
 [tool.poetry.dependencies]
 python = "^3.8"
-flet-contrib-core = "2024.05.03.1625"
+flet-contrib-core = "2024.05.09.2200"
 oauthlib = "^3.2.2"
 httpx = "^0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `flet_contrib_runtime-2024.5.3.1625/src/flet_runtime/app.py` & `flet_contrib_runtime-2024.5.9.2200/src/flet_runtime/app.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_runtime-2024.5.3.1625/src/flet_runtime/auth/__pycache__/authorization.cpython-39.pyc` & `flet_contrib_runtime-2024.5.9.2200/src/flet_runtime/auth/__pycache__/authorization.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu May  2 17:51:38 2024 UTC, .py size: 9278 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 aad2 3366 3e24 0000  a.........3f>$..
+00000000: 610d 0d0a 0000 0000 e0ed 3c66 3e24 0000  a.........<f>$..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 ba00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a02 6400 6401 6c03 5a03 6400  d.l.Z.d.d.l.Z.d.
 00000050: 6401 6c04 5a04 6400 6402 6c05 6d06 5a06  d.l.Z.d.d.l.m.Z.
 00000060: 6d07 5a07 6d08 5a08 0100 6400 6401 6c09  m.Z.m.Z...d.d.l.
 00000070: 5a09 6400 6403 6c0a 6d0b 5a0b 0100 6400  Z.d.d.l.m.Z...d.
```

### Comparing `flet_contrib_runtime-2024.5.3.1625/src/flet_runtime/auth/__pycache__/group.cpython-39.pyc` & `flet_contrib_runtime-2024.5.9.2200/src/flet_runtime/auth/__pycache__/group.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu May  2 17:51:38 2024 UTC, .py size: 128 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 aad2 3366 8000 0000  a.........3f....
+00000000: 610d 0d0a 0000 0000 e0ed 3c66 8000 0000  a.........<f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 1400 0000 4700  .....@...s....G.
 00000030: 6400 6401 8400 6401 6500 8303 5a01 6402  d.d...d.e...Z.d.
 00000040: 5300 2903 6300 0000 0000 0000 0000 0000  S.).c...........
 00000050: 0000 0000 0004 0000 0000 0000 0073 2400  .............s$.
 00000060: 0000 6500 5a01 6400 5a02 6503 6401 6402  ..e.Z.d.Z.e.d.d.
 00000070: 9c02 8700 6601 6403 6404 840c 5a04 8700  ....f.d.d...Z...
```

### Comparing `flet_contrib_runtime-2024.5.3.1625/src/flet_runtime/auth/__pycache__/oauth_provider.cpython-39.pyc` & `flet_contrib_runtime-2024.5.9.2200/src/flet_runtime/auth/__pycache__/oauth_provider.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu May  2 17:51:38 2024 UTC, .py size: 1806 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 aad2 3366 0e07 0000  a.........3f....
+00000000: 610d 0d0a 0000 0000 e0ed 3c66 0e07 0000  a.........<f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 3e00 0000 6400  .....@...s>...d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 6d03 5a03  d.l.m.Z.m.Z.m.Z.
 00000040: 0100 6400 6402 6c04 6d05 5a05 0100 6400  ..d.d.l.m.Z...d.
 00000050: 6403 6c06 6d07 5a07 0100 4700 6404 6405  d.l.m.Z...G.d.d.
 00000060: 8400 6405 8302 5a08 6406 5300 2907 e900  ..d...Z.d.S.)...
 00000070: 0000 0029 03da 0843 616c 6c61 626c 65da  ...)...Callable.
```

### Comparing `flet_contrib_runtime-2024.5.3.1625/src/flet_runtime/auth/__pycache__/oauth_token.cpython-39.pyc` & `flet_contrib_runtime-2024.5.9.2200/src/flet_runtime/auth/__pycache__/oauth_token.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu May  2 17:51:38 2024 UTC, .py size: 847 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 aad2 3366 4f03 0000  a.........3fO...
+00000000: 610d 0d0a 0000 0000 e0ed 3c66 4f03 0000  a.........<fO...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 3600 0000 6400  .....@...s6...d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 6d03 5a03 0100 6400 6403 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
 00000050: 0100 4700 6404 6405 8400 6405 8302 5a06  ..G.d.d...d...Z.
 00000060: 6401 5300 2906 e900 0000 004e 2902 da04  d.S.)......N)...
 00000070: 4c69 7374 da08 4f70 7469 6f6e 616c 2901  List..Optional).
```

### Comparing `flet_contrib_runtime-2024.5.3.1625/src/flet_runtime/auth/authorization.py` & `flet_contrib_runtime-2024.5.9.2200/src/flet_runtime/auth/authorization.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_runtime-2024.5.3.1625/src/flet_runtime/auth/oauth_provider.py` & `flet_contrib_runtime-2024.5.9.2200/src/flet_runtime/auth/oauth_provider.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_runtime-2024.5.3.1625/src/flet_runtime/auth/oauth_token.py` & `flet_contrib_runtime-2024.5.9.2200/src/flet_runtime/auth/oauth_token.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_runtime-2024.5.3.1625/src/flet_runtime/auth/providers/auth0_oauth_provider.py` & `flet_contrib_runtime-2024.5.9.2200/src/flet_runtime/auth/providers/auth0_oauth_provider.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_runtime-2024.5.3.1625/src/flet_runtime/auth/providers/azure_oauth_provider.py` & `flet_contrib_runtime-2024.5.9.2200/src/flet_runtime/auth/providers/azure_oauth_provider.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_runtime-2024.5.3.1625/src/flet_runtime/auth/providers/github_oauth_provider.py` & `flet_contrib_runtime-2024.5.9.2200/src/flet_runtime/auth/providers/github_oauth_provider.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_runtime-2024.5.3.1625/src/flet_runtime/auth/providers/google_oauth_provider.py` & `flet_contrib_runtime-2024.5.9.2200/src/flet_runtime/auth/providers/google_oauth_provider.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_runtime-2024.5.3.1625/src/flet_runtime/flet_socket_server.py` & `flet_contrib_runtime-2024.5.9.2200/src/flet_runtime/flet_socket_server.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_runtime-2024.5.3.1625/src/flet_runtime/security/__init__.py` & `flet_contrib_runtime-2024.5.9.2200/src/flet_runtime/security/__init__.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_runtime-2024.5.3.1625/src/flet_runtime/uploads.py` & `flet_contrib_runtime-2024.5.9.2200/src/flet_runtime/uploads.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_runtime-2024.5.3.1625/src/flet_runtime/utils/__init__.py` & `flet_contrib_runtime-2024.5.9.2200/src/flet_runtime/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_runtime-2024.5.3.1625/src/flet_runtime/utils/__pycache__/__init__.cpython-39.pyc` & `flet_contrib_runtime-2024.5.9.2200/src/flet_runtime/utils/__pycache__/__init__.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu May  2 17:51:38 2024 UTC, .py size: 4787 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 aad2 3366 b312 0000  a.........3f....
+00000000: 610d 0d0a 0000 0000 e0ed 3c66 b312 0000  a.........<f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0008 0000 0040 0000 0073 7801 0000 6400  .....@...sx...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a02 6400 6401 6c03 5a03 6400  d.l.Z.d.d.l.Z.d.
 00000050: 6401 6c04 5a04 6400 6402 6c05 6d06 5a06  d.l.Z.d.d.l.m.Z.
 00000060: 0100 6400 6403 6c07 6d08 5a08 0100 6400  ..d.d.l.m.Z...d.
 00000070: 6404 6c09 6d0a 5a0a 0100 6400 6405 6c0b  d.l.m.Z...d.d.l.
```

### Comparing `flet_contrib_runtime-2024.5.3.1625/src/flet_runtime/utils/__pycache__/once.cpython-39.pyc` & `flet_contrib_runtime-2024.5.9.2200/src/flet_runtime/utils/__pycache__/once.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu May  2 17:51:38 2024 UTC, .py size: 347 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 aad2 3366 5b01 0000  a.........3f[...
+00000000: 610d 0d0a 0000 0000 e0ed 3c66 5b01 0000  a.........<f[...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 1a00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 4700 6402 6403 8400 6403  d.l.Z.G.d.d...d.
 00000040: 8302 5a01 6401 5300 2904 e900 0000 004e  ..Z.d.S.)......N
 00000050: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
 00000060: 0002 0000 0040 0000 0073 1c00 0000 6500  .....@...s....e.
 00000070: 5a01 6400 5a02 6401 6402 8400 5a03 6403  Z.d.Z.d.d...Z.d.
```

### Comparing `flet_contrib_runtime-2024.5.3.1625/src/flet_runtime/utils/__pycache__/patch_index.cpython-39.pyc` & `flet_contrib_runtime-2024.5.9.2200/src/flet_runtime/utils/__pycache__/patch_index.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu May  2 17:51:38 2024 UTC, .py size: 3202 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 aad2 3366 820c 0000  a.........3f....
+00000000: 610d 0d0a 0000 0000 e0ed 3c66 820c 0000  a.........<f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 000d 0000 0040 0000 0073 9e00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6402 6c02 6d03 5a03 0100 6400 6403 6c04  d.l.m.Z...d.d.l.
 00000050: 6d05 5a05 0100 6400 6404 6c06 6d07 5a07  m.Z...d.d.l.m.Z.
 00000060: 0100 6401 6401 6401 6405 6405 6406 6507  ..d.d.d.d.d.d.e.
 00000070: 6a08 6405 6407 6609 6509 6509 6505 6509  j.d.d.f.e.e.e.e.
```

### Comparing `flet_contrib_runtime-2024.5.3.1625/src/flet_runtime/utils/patch_index.py` & `flet_contrib_runtime-2024.5.9.2200/src/flet_runtime/utils/patch_index.py`

 * *Files identical despite different names*

### Comparing `flet_contrib_runtime-2024.5.3.1625/PKG-INFO` & `flet_contrib_runtime-2024.5.9.2200/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: flet-contrib-runtime
-Version: 2024.5.3.1625
+Version: 2024.5.9.2200
 Summary: Flet Runtime - a base package for Flet desktop and Flet mobile.
 License: Apache-2.0
 Author: Appveyor Systems Inc.
 Author-email: hello@flet.dev
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: flet-contrib-core (==2024.05.03.1625)
+Requires-Dist: flet-contrib-core (==2024.05.09.2200)
 Requires-Dist: httpx (>=0,<1)
 Requires-Dist: oauthlib (>=3.2.2,<4.0.0)
 Project-URL: documentation, https://flet.dev/docs
 Project-URL: homepage, https://flet.dev
 Project-URL: repository, https://github.com/flet-dev/flet
 Description-Content-Type: text/markdown
```

