# Comparing `tmp/ghga_event_schemas-3.2.0.tar.gz` & `tmp/ghga_event_schemas-3.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ghga_event_schemas-3.2.0.tar", last modified: Fri May  3 09:48:11 2024, max compression
+gzip compressed data, was "ghga_event_schemas-3.3.0.tar", last modified: Fri May 10 09:22:05 2024, max compression
```

## Comparing `ghga_event_schemas-3.2.0.tar` & `ghga_event_schemas-3.3.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 09:48:11.575693 ghga_event_schemas-3.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11452 2024-05-03 09:48:03.000000 ghga_event_schemas-3.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     9328 2024-05-03 09:48:11.575693 ghga_event_schemas-3.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8411 2024-05-03 09:48:03.000000 ghga_event_schemas-3.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2422 2024-05-03 09:48:03.000000 ghga_event_schemas-3.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 09:48:11.575693 ghga_event_schemas-3.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 09:48:11.571694 ghga_event_schemas-3.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 09:48:11.575693 ghga_event_schemas-3.2.0/src/ghga_event_schemas/
--rw-r--r--   0 runner    (1001) docker     (127)      848 2024-05-03 09:48:03.000000 ghga_event_schemas-3.2.0/src/ghga_event_schemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15432 2024-05-03 09:48:03.000000 ghga_event_schemas-3.2.0/src/ghga_event_schemas/pydantic_.py
--rw-r--r--   0 runner    (1001) docker     (127)     2218 2024-05-03 09:48:03.000000 ghga_event_schemas-3.2.0/src/ghga_event_schemas/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 09:48:11.575693 ghga_event_schemas-3.2.0/src/ghga_event_schemas.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9328 2024-05-03 09:48:11.000000 ghga_event_schemas-3.2.0/src/ghga_event_schemas.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      394 2024-05-03 09:48:11.000000 ghga_event_schemas-3.2.0/src/ghga_event_schemas.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 09:48:11.000000 ghga_event_schemas-3.2.0/src/ghga_event_schemas.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-03 09:48:11.000000 ghga_event_schemas-3.2.0/src/ghga_event_schemas.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-03 09:48:11.000000 ghga_event_schemas-3.2.0/src/ghga_event_schemas.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 09:48:11.575693 ghga_event_schemas-3.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2209 2024-05-03 09:48:03.000000 ghga_event_schemas-3.2.0/tests/test_validation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 09:22:05.964087 ghga_event_schemas-3.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11452 2024-05-10 09:22:01.000000 ghga_event_schemas-3.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     9328 2024-05-10 09:22:05.964087 ghga_event_schemas-3.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8411 2024-05-10 09:22:01.000000 ghga_event_schemas-3.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2422 2024-05-10 09:22:01.000000 ghga_event_schemas-3.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 09:22:05.964087 ghga_event_schemas-3.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 09:22:05.960087 ghga_event_schemas-3.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 09:22:05.960087 ghga_event_schemas-3.3.0/src/ghga_event_schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)      848 2024-05-10 09:22:01.000000 ghga_event_schemas-3.3.0/src/ghga_event_schemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16040 2024-05-10 09:22:01.000000 ghga_event_schemas-3.3.0/src/ghga_event_schemas/pydantic_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2218 2024-05-10 09:22:01.000000 ghga_event_schemas-3.3.0/src/ghga_event_schemas/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 09:22:05.964087 ghga_event_schemas-3.3.0/src/ghga_event_schemas.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9328 2024-05-10 09:22:05.000000 ghga_event_schemas-3.3.0/src/ghga_event_schemas.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      394 2024-05-10 09:22:05.000000 ghga_event_schemas-3.3.0/src/ghga_event_schemas.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 09:22:05.000000 ghga_event_schemas-3.3.0/src/ghga_event_schemas.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-10 09:22:05.000000 ghga_event_schemas-3.3.0/src/ghga_event_schemas.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-10 09:22:05.000000 ghga_event_schemas-3.3.0/src/ghga_event_schemas.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 09:22:05.964087 ghga_event_schemas-3.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2209 2024-05-10 09:22:01.000000 ghga_event_schemas-3.3.0/tests/test_validation.py
```

### Comparing `ghga_event_schemas-3.2.0/LICENSE` & `ghga_event_schemas-3.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ghga_event_schemas-3.2.0/PKG-INFO` & `ghga_event_schemas-3.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ghga_event_schemas
-Version: 3.2.0
+Version: 3.3.0
 Summary: GHGA Event Schemas: A package that collects schemas used for events exchanged between GHGA service.
 Author-email: "German Human Genome Phenome Archive (GHGA)" <contact@ghga.de>
 License: Apache 2.0
 Project-URL: Repository, https://github.com/ghga-de/ghga-event-schemas
 Classifier: Development Status :: 1 - Planning
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
@@ -34,29 +34,29 @@
 
 ## Installation
 
 We recommend using the provided Docker container.
 
 A pre-build version is available at [docker hub](https://hub.docker.com/repository/docker/ghga/ghga-event-schemas):
 ```bash
-docker pull ghga/ghga-event-schemas:3.2.0
+docker pull ghga/ghga-event-schemas:3.3.0
 ```
 
 Or you can build the container yourself from the [`./Dockerfile`](./Dockerfile):
 ```bash
 # Execute in the repo's root dir:
-docker build -t ghga/ghga-event-schemas:3.2.0 .
+docker build -t ghga/ghga-event-schemas:3.3.0 .
 ```
 
 For production-ready deployment, we recommend using Kubernetes, however,
 for simple use cases, you could execute the service using docker
 on a single server:
 ```bash
 # The entrypoint is preconfigured:
-docker run -p 8080:8080 ghga/ghga-event-schemas:3.2.0 --help
+docker run -p 8080:8080 ghga/ghga-event-schemas:3.3.0 --help
 ```
 
 If you prefer not to use containers, you may install the service from source:
 ```bash
 # Execute in the repo's root dir:
 pip install .
```

### Comparing `ghga_event_schemas-3.2.0/README.md` & `ghga_event_schemas-3.3.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -13,29 +13,29 @@
 
 ## Installation
 
 We recommend using the provided Docker container.
 
 A pre-build version is available at [docker hub](https://hub.docker.com/repository/docker/ghga/ghga-event-schemas):
 ```bash
-docker pull ghga/ghga-event-schemas:3.2.0
+docker pull ghga/ghga-event-schemas:3.3.0
 ```
 
 Or you can build the container yourself from the [`./Dockerfile`](./Dockerfile):
 ```bash
 # Execute in the repo's root dir:
-docker build -t ghga/ghga-event-schemas:3.2.0 .
+docker build -t ghga/ghga-event-schemas:3.3.0 .
 ```
 
 For production-ready deployment, we recommend using Kubernetes, however,
 for simple use cases, you could execute the service using docker
 on a single server:
 ```bash
 # The entrypoint is preconfigured:
-docker run -p 8080:8080 ghga/ghga-event-schemas:3.2.0 --help
+docker run -p 8080:8080 ghga/ghga-event-schemas:3.3.0 --help
 ```
 
 If you prefer not to use containers, you may install the service from source:
 ```bash
 # Execute in the repo's root dir:
 pip install .
```

### Comparing `ghga_event_schemas-3.2.0/pyproject.toml` & `ghga_event_schemas-3.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     "Programming Language :: Python :: 3.12",
     "License :: OSI Approved :: Apache Software License",
     "Topic :: Internet :: WWW/HTTP :: HTTP Servers",
     "Topic :: Software Development :: Libraries",
     "Intended Audience :: Developers",
 ]
 name = "ghga_event_schemas"
-version = "3.2.0"
+version = "3.3.0"
 description = "GHGA Event Schemas: A package that collects schemas used for events exchanged between GHGA service."
 dependencies = [
     "jsonschema>=4.21.1,<5.0.0",
     "pydantic[email]>=2,<3",
 ]
 
 [project.license]
```

### Comparing `ghga_event_schemas-3.2.0/src/ghga_event_schemas/__init__.py` & `ghga_event_schemas-3.3.0/src/ghga_event_schemas/__init__.py`

 * *Files identical despite different names*

### Comparing `ghga_event_schemas-3.2.0/src/ghga_event_schemas/pydantic_.py` & `ghga_event_schemas-3.3.0/src/ghga_event_schemas/pydantic_.py`

 * *Files 1% similar despite different names*

```diff
@@ -392,14 +392,39 @@
 
 class UserID(BaseModel):
     """Generic event payload to relay a user ID."""
 
     user_id: str = Field(..., description="The user ID")
 
 
+class AcademicTitle(str, Enum):
+    """Academic title"""
+
+    DR = "Dr."
+    PROF = "Prof."
+
+
+class User(UserID):
+    """Event used to publish user data changes via outbox pattern."""
+
+    name: str = Field(
+        default=...,
+        description="Full name of the user",
+        examples=["Rosalind Franklin"],
+    )
+    title: AcademicTitle | None = Field(
+        default=None, title="Academic title", description="Academic title of the user"
+    )
+    email: EmailStr = Field(
+        default=...,
+        description="Preferred e-mail address of the user",
+        examples=["user@home.org"],
+    )
+
+
 class AccessRequestDetails(UserID):
     """Event used to convey the user ID and dataset ID of an access request."""
 
     dataset_id: str = Field(..., description="The dataset ID")
 
 
 class IvaType(str, Enum):
```

### Comparing `ghga_event_schemas-3.2.0/src/ghga_event_schemas/validation.py` & `ghga_event_schemas-3.3.0/src/ghga_event_schemas/validation.py`

 * *Files identical despite different names*

### Comparing `ghga_event_schemas-3.2.0/src/ghga_event_schemas.egg-info/PKG-INFO` & `ghga_event_schemas-3.3.0/src/ghga_event_schemas.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ghga_event_schemas
-Version: 3.2.0
+Version: 3.3.0
 Summary: GHGA Event Schemas: A package that collects schemas used for events exchanged between GHGA service.
 Author-email: "German Human Genome Phenome Archive (GHGA)" <contact@ghga.de>
 License: Apache 2.0
 Project-URL: Repository, https://github.com/ghga-de/ghga-event-schemas
 Classifier: Development Status :: 1 - Planning
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
@@ -34,29 +34,29 @@
 
 ## Installation
 
 We recommend using the provided Docker container.
 
 A pre-build version is available at [docker hub](https://hub.docker.com/repository/docker/ghga/ghga-event-schemas):
 ```bash
-docker pull ghga/ghga-event-schemas:3.2.0
+docker pull ghga/ghga-event-schemas:3.3.0
 ```
 
 Or you can build the container yourself from the [`./Dockerfile`](./Dockerfile):
 ```bash
 # Execute in the repo's root dir:
-docker build -t ghga/ghga-event-schemas:3.2.0 .
+docker build -t ghga/ghga-event-schemas:3.3.0 .
 ```
 
 For production-ready deployment, we recommend using Kubernetes, however,
 for simple use cases, you could execute the service using docker
 on a single server:
 ```bash
 # The entrypoint is preconfigured:
-docker run -p 8080:8080 ghga/ghga-event-schemas:3.2.0 --help
+docker run -p 8080:8080 ghga/ghga-event-schemas:3.3.0 --help
 ```
 
 If you prefer not to use containers, you may install the service from source:
 ```bash
 # Execute in the repo's root dir:
 pip install .
```

### Comparing `ghga_event_schemas-3.2.0/tests/test_validation.py` & `ghga_event_schemas-3.3.0/tests/test_validation.py`

 * *Files identical despite different names*

