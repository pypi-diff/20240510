# Comparing `tmp/enola-0.6.0.tar.gz` & `tmp/enola-0.7.0.tar.gz`

## Comparing `enola-0.6.0.tar` & `enola-0.7.0.tar`

### file list

```diff
@@ -1,46 +1,46 @@
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 enola-0.6.0/requirements.txt
--rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 enola-0.6.0/.vscode/launch.json
--rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 enola-0.6.0/mi_entorno/pyvenv.cfg
--rw-r--r--   0        0        0    26199 2020-02-02 00:00:00.000000 enola-0.6.0/mi_entorno/Scripts/Activate.ps1
--rw-r--r--   0        0        0     2110 2020-02-02 00:00:00.000000 enola-0.6.0/mi_entorno/Scripts/activate
--rwxr-xr-x   0        0        0     1039 2020-02-02 00:00:00.000000 enola-0.6.0/mi_entorno/Scripts/activate.bat
--rwxr-xr-x   0        0        0      393 2020-02-02 00:00:00.000000 enola-0.6.0/mi_entorno/Scripts/deactivate.bat
--rwxr-xr-x   0        0        0   108448 2020-02-02 00:00:00.000000 enola-0.6.0/mi_entorno/Scripts/normalizer.exe
--rwxr-xr-x   0        0        0   108436 2020-02-02 00:00:00.000000 enola-0.6.0/mi_entorno/Scripts/pip.exe
--rwxr-xr-x   0        0        0   108436 2020-02-02 00:00:00.000000 enola-0.6.0/mi_entorno/Scripts/pip3.11.exe
--rwxr-xr-x   0        0        0   108436 2020-02-02 00:00:00.000000 enola-0.6.0/mi_entorno/Scripts/pip3.exe
--rwxr-xr-x   0        0        0   270608 2020-02-02 00:00:00.000000 enola-0.6.0/mi_entorno/Scripts/python.exe
--rwxr-xr-x   0        0        0   259352 2020-02-02 00:00:00.000000 enola-0.6.0/mi_entorno/Scripts/pythonw.exe
--rw-r--r--   0        0        0     3237 2020-02-02 00:00:00.000000 enola-0.6.0/src/test.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 enola-0.6.0/src/enola/__init__.py
--rw-r--r--   0        0        0    16261 2020-02-02 00:00:00.000000 enola-0.6.0/src/enola/agent.py
--rw-r--r--   0        0        0     6533 2020-02-02 00:00:00.000000 enola-0.6.0/src/enola/step.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 enola-0.6.0/src/enola/base/__init__.py
--rw-r--r--   0        0        0     2924 2020-02-02 00:00:00.000000 enola-0.6.0/src/enola/base/connect.py
--rw-r--r--   0        0        0     6468 2020-02-02 00:00:00.000000 enola-0.6.0/src/enola/base/enola_types.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 enola-0.6.0/src/enola/base/common/__init__.py
--rw-r--r--   0        0        0     3794 2020-02-02 00:00:00.000000 enola-0.6.0/src/enola/base/common/huemul_common.py
--rw-r--r--   0        0        0     6187 2020-02-02 00:00:00.000000 enola-0.6.0/src/enola/base/common/huemul_connection.py
--rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 enola-0.6.0/src/enola/base/common/huemul_datetime_part.py
--rw-r--r--   0        0        0     3217 2020-02-02 00:00:00.000000 enola-0.6.0/src/enola/base/common/huemul_error.py
--rw-r--r--   0        0        0     1484 2020-02-02 00:00:00.000000 enola-0.6.0/src/enola/base/common/huemul_functions.py
--rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 enola-0.6.0/src/enola/base/common/huemul_http_info.py
--rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 enola-0.6.0/src/enola/base/common/huemul_logging.py
--rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 enola-0.6.0/src/enola/base/common/huemul_param.py
--rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 enola-0.6.0/src/enola/base/common/huemul_response_error.py
--rw-r--r--   0        0        0     3041 2020-02-02 00:00:00.000000 enola-0.6.0/src/enola/base/common/huemul_response_provider.py
--rw-r--r--   0        0        0     6294 2020-02-02 00:00:00.000000 enola-0.6.0/src/enola/base/common/huemul_response_to_bloc.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 enola-0.6.0/src/enola/base/common/auth/__init__.py
--rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 enola-0.6.0/src/enola/base/common/auth/auth_model.py
--rw-r--r--   0        0        0     1049 2020-02-02 00:00:00.000000 enola-0.6.0/src/enola/base/common/auth/auth_service_bloc.py
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 enola-0.6.0/src/enola/base/common/auth/auth_service_model.py
--rw-r--r--   0        0        0     1613 2020-02-02 00:00:00.000000 enola-0.6.0/src/enola/base/common/auth/auth_service_provider.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 enola-0.6.0/src/enola/base/internal/__init__.py
--rw-r--r--   0        0        0     2811 2020-02-02 00:00:00.000000 enola-0.6.0/src/enola/base/internal/enola_agent.py
--rw-r--r--   0        0        0      967 2020-02-02 00:00:00.000000 enola-0.6.0/src/enola/base/internal/enola_agent_bloc.py
--rw-r--r--   0        0        0     1962 2020-02-02 00:00:00.000000 enola-0.6.0/src/enola/base/internal/enola_agent_provider.py
--rw-r--r--   0        0        0     3270 2020-02-02 00:00:00.000000 enola-0.6.0/.gitignore
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 enola-0.6.0/LICENSE
--rw-r--r--   0        0        0      602 2020-02-02 00:00:00.000000 enola-0.6.0/README.md
--rw-r--r--   0        0        0      779 2020-02-02 00:00:00.000000 enola-0.6.0/pyproject.toml
--rw-r--r--   0        0        0     1235 2020-02-02 00:00:00.000000 enola-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 enola-0.7.0/requirements.txt
+-rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 enola-0.7.0/.vscode/launch.json
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 enola-0.7.0/mi_entorno/pyvenv.cfg
+-rw-r--r--   0        0        0    26199 2020-02-02 00:00:00.000000 enola-0.7.0/mi_entorno/Scripts/Activate.ps1
+-rw-r--r--   0        0        0     2110 2020-02-02 00:00:00.000000 enola-0.7.0/mi_entorno/Scripts/activate
+-rwxr-xr-x   0        0        0     1039 2020-02-02 00:00:00.000000 enola-0.7.0/mi_entorno/Scripts/activate.bat
+-rwxr-xr-x   0        0        0      393 2020-02-02 00:00:00.000000 enola-0.7.0/mi_entorno/Scripts/deactivate.bat
+-rwxr-xr-x   0        0        0   108448 2020-02-02 00:00:00.000000 enola-0.7.0/mi_entorno/Scripts/normalizer.exe
+-rwxr-xr-x   0        0        0   108436 2020-02-02 00:00:00.000000 enola-0.7.0/mi_entorno/Scripts/pip.exe
+-rwxr-xr-x   0        0        0   108436 2020-02-02 00:00:00.000000 enola-0.7.0/mi_entorno/Scripts/pip3.11.exe
+-rwxr-xr-x   0        0        0   108436 2020-02-02 00:00:00.000000 enola-0.7.0/mi_entorno/Scripts/pip3.exe
+-rwxr-xr-x   0        0        0   270608 2020-02-02 00:00:00.000000 enola-0.7.0/mi_entorno/Scripts/python.exe
+-rwxr-xr-x   0        0        0   259352 2020-02-02 00:00:00.000000 enola-0.7.0/mi_entorno/Scripts/pythonw.exe
+-rw-r--r--   0        0        0     3237 2020-02-02 00:00:00.000000 enola-0.7.0/src/test.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 enola-0.7.0/src/enola/__init__.py
+-rw-r--r--   0        0        0    16261 2020-02-02 00:00:00.000000 enola-0.7.0/src/enola/agent.py
+-rw-r--r--   0        0        0     6533 2020-02-02 00:00:00.000000 enola-0.7.0/src/enola/step.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 enola-0.7.0/src/enola/base/__init__.py
+-rw-r--r--   0        0        0     2924 2020-02-02 00:00:00.000000 enola-0.7.0/src/enola/base/connect.py
+-rw-r--r--   0        0        0     6468 2020-02-02 00:00:00.000000 enola-0.7.0/src/enola/base/enola_types.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 enola-0.7.0/src/enola/base/common/__init__.py
+-rw-r--r--   0        0        0     3794 2020-02-02 00:00:00.000000 enola-0.7.0/src/enola/base/common/huemul_common.py
+-rw-r--r--   0        0        0     6187 2020-02-02 00:00:00.000000 enola-0.7.0/src/enola/base/common/huemul_connection.py
+-rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 enola-0.7.0/src/enola/base/common/huemul_datetime_part.py
+-rw-r--r--   0        0        0     3217 2020-02-02 00:00:00.000000 enola-0.7.0/src/enola/base/common/huemul_error.py
+-rw-r--r--   0        0        0     1484 2020-02-02 00:00:00.000000 enola-0.7.0/src/enola/base/common/huemul_functions.py
+-rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 enola-0.7.0/src/enola/base/common/huemul_http_info.py
+-rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 enola-0.7.0/src/enola/base/common/huemul_logging.py
+-rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 enola-0.7.0/src/enola/base/common/huemul_param.py
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 enola-0.7.0/src/enola/base/common/huemul_response_error.py
+-rw-r--r--   0        0        0     3041 2020-02-02 00:00:00.000000 enola-0.7.0/src/enola/base/common/huemul_response_provider.py
+-rw-r--r--   0        0        0     6294 2020-02-02 00:00:00.000000 enola-0.7.0/src/enola/base/common/huemul_response_to_bloc.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 enola-0.7.0/src/enola/base/common/auth/__init__.py
+-rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 enola-0.7.0/src/enola/base/common/auth/auth_model.py
+-rw-r--r--   0        0        0     1049 2020-02-02 00:00:00.000000 enola-0.7.0/src/enola/base/common/auth/auth_service_bloc.py
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 enola-0.7.0/src/enola/base/common/auth/auth_service_model.py
+-rw-r--r--   0        0        0     1613 2020-02-02 00:00:00.000000 enola-0.7.0/src/enola/base/common/auth/auth_service_provider.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 enola-0.7.0/src/enola/base/internal/__init__.py
+-rw-r--r--   0        0        0     2811 2020-02-02 00:00:00.000000 enola-0.7.0/src/enola/base/internal/enola_agent.py
+-rw-r--r--   0        0        0      967 2020-02-02 00:00:00.000000 enola-0.7.0/src/enola/base/internal/enola_agent_bloc.py
+-rw-r--r--   0        0        0     1962 2020-02-02 00:00:00.000000 enola-0.7.0/src/enola/base/internal/enola_agent_provider.py
+-rw-r--r--   0        0        0     3270 2020-02-02 00:00:00.000000 enola-0.7.0/.gitignore
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 enola-0.7.0/LICENSE
+-rw-r--r--   0        0        0      602 2020-02-02 00:00:00.000000 enola-0.7.0/README.md
+-rw-r--r--   0        0        0      779 2020-02-02 00:00:00.000000 enola-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0     1235 2020-02-02 00:00:00.000000 enola-0.7.0/PKG-INFO
```

### Comparing `enola-0.6.0/mi_entorno/Scripts/Activate.ps1` & `enola-0.7.0/mi_entorno/Scripts/Activate.ps1`

 * *Files identical despite different names*

### Comparing `enola-0.6.0/mi_entorno/Scripts/activate` & `enola-0.7.0/mi_entorno/Scripts/activate`

 * *Files identical despite different names*

### Comparing `enola-0.6.0/mi_entorno/Scripts/activate.bat` & `enola-0.7.0/mi_entorno/Scripts/activate.bat`

 * *Files identical despite different names*

### Comparing `enola-0.6.0/mi_entorno/Scripts/normalizer.exe` & `enola-0.7.0/mi_entorno/Scripts/normalizer.exe`

 * *Files identical despite different names*

### Comparing `enola-0.6.0/mi_entorno/Scripts/pip.exe` & `enola-0.7.0/mi_entorno/Scripts/pip.exe`

 * *Files identical despite different names*

### Comparing `enola-0.6.0/mi_entorno/Scripts/pip3.11.exe` & `enola-0.7.0/mi_entorno/Scripts/pip3.11.exe`

 * *Files identical despite different names*

### Comparing `enola-0.6.0/mi_entorno/Scripts/pip3.exe` & `enola-0.7.0/mi_entorno/Scripts/pip3.exe`

 * *Files identical despite different names*

### Comparing `enola-0.6.0/mi_entorno/Scripts/python.exe` & `enola-0.7.0/mi_entorno/Scripts/python.exe`

 * *Files identical despite different names*

### Comparing `enola-0.6.0/mi_entorno/Scripts/pythonw.exe` & `enola-0.7.0/mi_entorno/Scripts/pythonw.exe`

 * *Files identical despite different names*

### Comparing `enola-0.6.0/src/test.py` & `enola-0.7.0/src/test.py`

 * *Files identical despite different names*

### Comparing `enola-0.6.0/src/enola/agent.py` & `enola-0.7.0/src/enola/agent.py`

 * *Files identical despite different names*

### Comparing `enola-0.6.0/src/enola/step.py` & `enola-0.7.0/src/enola/step.py`

 * *Files identical despite different names*

### Comparing `enola-0.6.0/src/enola/base/connect.py` & `enola-0.7.0/src/enola/base/connect.py`

 * *Files identical despite different names*

### Comparing `enola-0.6.0/src/enola/base/enola_types.py` & `enola-0.7.0/src/enola/base/enola_types.py`

 * *Files identical despite different names*

### Comparing `enola-0.6.0/src/enola/base/common/huemul_common.py` & `enola-0.7.0/src/enola/base/common/huemul_common.py`

 * *Files identical despite different names*

### Comparing `enola-0.6.0/src/enola/base/common/huemul_connection.py` & `enola-0.7.0/src/enola/base/common/huemul_connection.py`

 * *Files identical despite different names*

### Comparing `enola-0.6.0/src/enola/base/common/huemul_error.py` & `enola-0.7.0/src/enola/base/common/huemul_error.py`

 * *Files identical despite different names*

### Comparing `enola-0.6.0/src/enola/base/common/huemul_functions.py` & `enola-0.7.0/src/enola/base/common/huemul_functions.py`

 * *Files identical despite different names*

### Comparing `enola-0.6.0/src/enola/base/common/huemul_logging.py` & `enola-0.7.0/src/enola/base/common/huemul_logging.py`

 * *Files identical despite different names*

### Comparing `enola-0.6.0/src/enola/base/common/huemul_response_provider.py` & `enola-0.7.0/src/enola/base/common/huemul_response_provider.py`

 * *Files identical despite different names*

### Comparing `enola-0.6.0/src/enola/base/common/huemul_response_to_bloc.py` & `enola-0.7.0/src/enola/base/common/huemul_response_to_bloc.py`

 * *Files identical despite different names*

### Comparing `enola-0.6.0/src/enola/base/common/auth/auth_model.py` & `enola-0.7.0/src/enola/base/common/auth/auth_model.py`

 * *Files identical despite different names*

### Comparing `enola-0.6.0/src/enola/base/common/auth/auth_service_bloc.py` & `enola-0.7.0/src/enola/base/common/auth/auth_service_bloc.py`

 * *Files identical despite different names*

### Comparing `enola-0.6.0/src/enola/base/common/auth/auth_service_provider.py` & `enola-0.7.0/src/enola/base/common/auth/auth_service_provider.py`

 * *Files identical despite different names*

### Comparing `enola-0.6.0/src/enola/base/internal/enola_agent.py` & `enola-0.7.0/src/enola/base/internal/enola_agent.py`

 * *Files identical despite different names*

### Comparing `enola-0.6.0/src/enola/base/internal/enola_agent_bloc.py` & `enola-0.7.0/src/enola/base/internal/enola_agent_bloc.py`

 * *Files identical despite different names*

### Comparing `enola-0.6.0/src/enola/base/internal/enola_agent_provider.py` & `enola-0.7.0/src/enola/base/internal/enola_agent_provider.py`

 * *Files identical despite different names*

### Comparing `enola-0.6.0/.gitignore` & `enola-0.7.0/.gitignore`

 * *Files identical despite different names*

### Comparing `enola-0.6.0/README.md` & `enola-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `enola-0.6.0/pyproject.toml` & `enola-0.7.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "enola"
-version = "0.6.0"
+version = "0.7.0"
 authors = [
   { name="Sebastian Rodriguez Robotham", email="sebastian.rodriguez@huemulsolutions.com" },
   { name="Developer Code", email="developer.code@huemulsolutions.com" },
 ]
 description = "Observability & Governance of Intelligence Agents"
 keywords = ["AI", "Observability", "agent", "Intelligence"]
 readme = "README.md"
```

### Comparing `enola-0.6.0/PKG-INFO` & `enola-0.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: enola
-Version: 0.6.0
+Version: 0.7.0
 Summary: Observability & Governance of Intelligence Agents
 Project-URL: Homepage, https://github.com/huemulsolutions/enola
 Project-URL: Bug Tracker, https://github.com/huemulsolutions/enola/issues
 Author-email: Sebastian Rodriguez Robotham <sebastian.rodriguez@huemulsolutions.com>, Developer Code <developer.code@huemulsolutions.com>
 License-File: LICENSE
 Keywords: AI,Intelligence,Observability,agent
 Classifier: License :: OSI Approved :: MIT License
```

