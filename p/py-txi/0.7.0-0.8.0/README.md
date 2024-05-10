# Comparing `tmp/py-txi-0.7.0.tar.gz` & `tmp/py-txi-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-txi-0.7.0.tar", last modified: Sat Apr 13 12:18:47 2024, max compression
+gzip compressed data, was "py-txi-0.8.0.tar", last modified: Fri May 10 07:54:02 2024, max compression
```

## Comparing `py-txi-0.7.0.tar` & `py-txi-0.8.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 12:18:47.333553 py-txi-0.7.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-13 12:18:19.000000 py-txi-0.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3545 2024-04-13 12:18:47.333553 py-txi-0.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3013 2024-04-13 12:18:19.000000 py-txi-0.7.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 12:18:47.333553 py-txi-0.7.0/py_txi/
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-04-13 12:18:19.000000 py-txi-0.7.0/py_txi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7316 2024-04-13 12:18:19.000000 py-txi-0.7.0/py_txi/inference_server.py
--rw-r--r--   0 runner    (1001) docker     (127)     2579 2024-04-13 12:18:19.000000 py-txi-0.7.0/py_txi/text_embedding_inference.py
--rw-r--r--   0 runner    (1001) docker     (127)     3047 2024-04-13 12:18:19.000000 py-txi-0.7.0/py_txi/text_generation_inference.py
--rw-r--r--   0 runner    (1001) docker     (127)     1677 2024-04-13 12:18:19.000000 py-txi-0.7.0/py_txi/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 12:18:47.333553 py-txi-0.7.0/py_txi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3545 2024-04-13 12:18:47.000000 py-txi-0.7.0/py_txi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      323 2024-04-13 12:18:47.000000 py-txi-0.7.0/py_txi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 12:18:47.000000 py-txi-0.7.0/py_txi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-13 12:18:47.000000 py-txi-0.7.0/py_txi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-13 12:18:47.000000 py-txi-0.7.0/py_txi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      367 2024-04-13 12:18:19.000000 py-txi-0.7.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-13 12:18:47.333553 py-txi-0.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      993 2024-04-13 12:18:19.000000 py-txi-0.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 07:54:02.225594 py-txi-0.8.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-10 07:53:50.000000 py-txi-0.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3525 2024-05-10 07:54:02.225594 py-txi-0.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2993 2024-05-10 07:53:50.000000 py-txi-0.8.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 07:54:02.225594 py-txi-0.8.0/py_txi/
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-05-10 07:53:50.000000 py-txi-0.8.0/py_txi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7665 2024-05-10 07:53:50.000000 py-txi-0.8.0/py_txi/inference_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2579 2024-05-10 07:53:50.000000 py-txi-0.8.0/py_txi/text_embedding_inference.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3037 2024-05-10 07:53:50.000000 py-txi-0.8.0/py_txi/text_generation_inference.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1732 2024-05-10 07:53:50.000000 py-txi-0.8.0/py_txi/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 07:54:02.225594 py-txi-0.8.0/py_txi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3525 2024-05-10 07:54:02.000000 py-txi-0.8.0/py_txi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-05-10 07:54:02.000000 py-txi-0.8.0/py_txi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 07:54:02.000000 py-txi-0.8.0/py_txi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-10 07:54:02.000000 py-txi-0.8.0/py_txi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-10 07:54:02.000000 py-txi-0.8.0/py_txi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      367 2024-05-10 07:53:50.000000 py-txi-0.8.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 07:54:02.225594 py-txi-0.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      978 2024-05-10 07:53:50.000000 py-txi-0.8.0/setup.py
```

### Comparing `py-txi-0.7.0/LICENSE` & `py-txi-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `py-txi-0.7.0/PKG-INFO` & `py-txi-0.8.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-txi
-Version: 0.7.0
+Version: 0.8.0
 Summary: A Python wrapper around TGI and TEI servers
 Home-page: https://github.com/IlyasMoutawwakil/py-txi
 Author: Ilyas Moutawwakil
 Author-email: ilyas.moutawwakil@gmail.com
 Keywords: tgi,llm,tei,embedding,huggingface,docker,python
 Platform: linux
 Platform: windows
@@ -12,15 +12,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Natural Language :: English
 Description-Content-Type: text/markdown
 Provides-Extra: quality
 Provides-Extra: testing
 License-File: LICENSE
 
-# Py-TXI (previously Py-TGI)
+# Py-TXI
 
 [![PyPI version](https://badge.fury.io/py/py-txi.svg)](https://badge.fury.io/py/py-txi)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/py-txi)](https://pypi.org/project/py-txi/)
 [![PyPI - Format](https://img.shields.io/pypi/format/py-txi)](https://pypi.org/project/py-txi/)
 [![Downloads](https://pepy.tech/badge/py-txi)](https://pepy.tech/project/py-txi)
 [![PyPI - License](https://img.shields.io/pypi/l/py-txi)](https://pypi.org/project/py-txi/)
 [![Test](https://github.com/IlyasMoutawwakil/py-txi/actions/workflows/test.yaml/badge.svg)](https://github.com/IlyasMoutawwakil/py-txi/actions/workflows/tests.yaml)
```

### Comparing `py-txi-0.7.0/README.md` & `py-txi-0.8.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Py-TXI (previously Py-TGI)
+# Py-TXI
 
 [![PyPI version](https://badge.fury.io/py/py-txi.svg)](https://badge.fury.io/py/py-txi)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/py-txi)](https://pypi.org/project/py-txi/)
 [![PyPI - Format](https://img.shields.io/pypi/format/py-txi)](https://pypi.org/project/py-txi/)
 [![Downloads](https://pepy.tech/badge/py-txi)](https://pepy.tech/project/py-txi)
 [![PyPI - License](https://img.shields.io/pypi/l/py-txi)](https://pypi.org/project/py-txi/)
 [![Test](https://github.com/IlyasMoutawwakil/py-txi/actions/workflows/test.yaml/badge.svg)](https://github.com/IlyasMoutawwakil/py-txi/actions/workflows/tests.yaml)
```

### Comparing `py-txi-0.7.0/py_txi/inference_server.py` & `py-txi-0.8.0/py_txi/inference_server.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 import asyncio
+import logging
 import os
 import re
 import time
 from abc import ABC
 from dataclasses import asdict, dataclass, field
-from logging import INFO, getLogger
+from logging import getLogger
 from typing import Any, Dict, List, Optional, Union
 
-import coloredlogs
 import docker
 import docker.errors
 import docker.types
 from huggingface_hub import AsyncInferenceClient
+from huggingface_hub.constants import HUGGINGFACE_HUB_CACHE
 
 from .utils import get_free_port, styled_logs
 
-coloredlogs.install(level=INFO, fmt="[%(asctime)s][%(filename)s][%(levelname)s] %(message)s")
-
 DOCKER = docker.from_env()
 LOGGER = getLogger("Inference-Server")
+logging.basicConfig(level=logging.INFO)
 
 
 @dataclass
 class InferenceServerConfig:
     # Common options
-    model_id: str
+    model_id: Optional[str] = None
     revision: Optional[str] = "main"
     # Image to use for the container
     image: Optional[str] = None
     # Shared memory size for the container
     shm_size: Optional[str] = None
     # List of custom devices to forward to the container e.g. ["/dev/kfd", "/dev/dri"] for ROCm
     devices: Optional[List[str]] = None
@@ -36,15 +36,15 @@
     gpus: Optional[Union[str, int]] = None
 
     ports: Dict[str, Any] = field(
         default_factory=lambda: {"80/tcp": ("0.0.0.0", 0)},
         metadata={"help": "Dictionary of ports to expose from the container."},
     )
     volumes: Dict[str, Any] = field(
-        default_factory=lambda: {os.path.expanduser("~/.cache/huggingface/hub"): {"bind": "/data", "mode": "rw"}},
+        default_factory=lambda: {HUGGINGFACE_HUB_CACHE: {"bind": "/data", "mode": "rw"}},
         metadata={"help": "Dictionary of volumes to mount inside the container."},
     )
     environment: List[str] = field(
         default_factory=lambda: ["HUGGINGFACE_HUB_TOKEN"],
         metadata={"help": "List of environment variables to forward to the container."},
     )
 
@@ -92,19 +92,25 @@
             self.device_requests = [docker.types.DeviceRequest(device_ids=[self.config.gpus], capabilities=[["gpu"]])]
         else:
             LOGGER.info("\t+ Not using any GPU(s)")
             self.device_requests = None
 
         LOGGER.info(f"\t+ Building {self.NAME} command")
         self.command = []
+
+        if self.config.model_id is not None:
+            self.command = ["--model-id", self.config.model_id]
+        if self.config.revision is not None:
+            self.command.extend(["--revision", self.config.revision])
+
         for k, v in asdict(self.config).items():
             if k in InferenceServerConfig.__annotations__:
                 continue
             elif v is not None:
-                if isinstance(v, bool):
+                if isinstance(v, bool) and not k == "sharded":
                     self.command.append(f"--{k.replace('_', '-')}")
                 else:
                     self.command.append(f"--{k.replace('_', '-')}={str(v).lower()}")
 
         self.command.append("--json-output")
 
         LOGGER.info(f"\t+ Building {self.NAME} environment")
@@ -172,21 +178,23 @@
 
     async def batch_client_call(self, *args, **kwargs) -> Any:
         raise NotImplementedError
 
     def close(self) -> None:
         if hasattr(self, "container"):
             LOGGER.info("\t+ Stoping Docker container")
-            self.container.stop()
-            self.container.wait()
+            if self.container.status == "running":
+                self.container.stop()
+                self.container.wait()
             LOGGER.info("\t+ Docker container stopped")
             del self.container
 
         if hasattr(self, "semaphore"):
-            self.semaphore
+            if self.semaphore.locked():
+                self.semaphore.release()
             del self.semaphore
 
         if hasattr(self, "client"):
             del self.client
 
     def __del__(self) -> None:
         self.close()
```

### Comparing `py-txi-0.7.0/py_txi/text_embedding_inference.py` & `py-txi-0.8.0/py_txi/text_embedding_inference.py`

 * *Files identical despite different names*

### Comparing `py-txi-0.7.0/py_txi/text_generation_inference.py` & `py-txi-0.8.0/py_txi/text_generation_inference.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,38 +13,37 @@
 Quantize_Literal = Literal["bitsandbytes-nf4", "bitsandbytes-fp4", "gptq", "awq", "eetq", "fp8"]
 
 
 @dataclass
 class TGIConfig(InferenceServerConfig):
     # Launcher options
     num_shard: Optional[int] = None
+    speculate: Optional[int] = None
     cuda_graphs: Optional[int] = None
     dtype: Optional[DType_Literal] = None
     sharded: Optional[Shareded_Literal] = None
     quantize: Optional[Quantize_Literal] = None
     disable_custom_kernels: Optional[bool] = None
     trust_remote_code: Optional[bool] = None
     # Concurrency options
     max_concurrent_requests: int = 128
 
     def __post_init__(self) -> None:
         super().__post_init__()
 
         if self.image is None:
             if is_nvidia_system() and self.gpus is not None:
-                LOGGER.info("\t+ Using the latest NVIDIA GPU image for Text-Generation-Inference")
+                LOGGER.info("\t+ Using latest NVIDIA GPU image for Text-Generation-Inference")
                 self.image = "ghcr.io/huggingface/text-generation-inference:latest"
             elif is_rocm_system() and self.devices is not None:
-                LOGGER.info("\t+ Using the latest ROCm AMD GPU image for Text-Generation-Inference")
+                LOGGER.info("\t+ Using latest ROCm AMD GPU image for Text-Generation-Inference")
                 self.image = "ghcr.io/huggingface/text-generation-inference:latest-rocm"
             else:
-                raise ValueError(
-                    "Unsupported system. Please either provide the image to use explicitly "
-                    "or use a supported system (NVIDIA/ROCm) while specifying gpus/devices."
-                )
+                LOGGER.info("\t+ Using version 1.4 image for Text-Generation-Inference (last image with CPU support)")
+                self.image = "ghcr.io/huggingface/text-generation-inference:1.4"
 
         if is_rocm_system() and "rocm" not in self.image:
             LOGGER.warning("\t+ You are running on a ROCm AMD GPU system but using a non-ROCM image.")
 
 
 class TGI(InferenceServer):
     NAME: str = "Text-Generation-Inference"
```

### Comparing `py-txi-0.7.0/py_txi/utils.py` & `py-txi-0.8.0/py_txi/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,24 +31,27 @@
     "INFO": "\033[37m",
     "WARN": "\033[33m",
     "WARNING": "\033[33m",
     "ERROR": "\033[31m",
     "CRITICAL": "\033[31m",
 }
 TIMESTAMP_STYLE = "\033[32m"
-TARGET_STYLE = "\033[0;38"
+TARGET_STYLE = "\033[0;38m"
 LEVEL_STYLE = "\033[1;30m"
 
 
 def color_text(text: str, color: str) -> str:
     return f"{color}{text}\033[0m"
 
 
 def styled_logs(log: str) -> str:
-    dict_log = loads(log)
+    try:
+        dict_log = loads(log)
+    except Exception:
+        return log
 
     fields = dict_log.get("fields", {})
     level = dict_log.get("level", "could not parse level")
     target = dict_log.get("target", "could not parse target")
     timestamp = dict_log.get("timestamp", "could not parse timestamp")
     message = fields.get("message", dict_log.get("message", "could not parse message"))
     timestamp = datetime.strptime(timestamp, "%Y-%m-%dT%H:%M:%S.%fZ").strftime("%Y-%m-%d %H:%M:%S")
```

### Comparing `py-txi-0.7.0/py_txi.egg-info/PKG-INFO` & `py-txi-0.8.0/py_txi.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-txi
-Version: 0.7.0
+Version: 0.8.0
 Summary: A Python wrapper around TGI and TEI servers
 Home-page: https://github.com/IlyasMoutawwakil/py-txi
 Author: Ilyas Moutawwakil
 Author-email: ilyas.moutawwakil@gmail.com
 Keywords: tgi,llm,tei,embedding,huggingface,docker,python
 Platform: linux
 Platform: windows
@@ -12,15 +12,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Natural Language :: English
 Description-Content-Type: text/markdown
 Provides-Extra: quality
 Provides-Extra: testing
 License-File: LICENSE
 
-# Py-TXI (previously Py-TGI)
+# Py-TXI
 
 [![PyPI version](https://badge.fury.io/py/py-txi.svg)](https://badge.fury.io/py/py-txi)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/py-txi)](https://pypi.org/project/py-txi/)
 [![PyPI - Format](https://img.shields.io/pypi/format/py-txi)](https://pypi.org/project/py-txi/)
 [![Downloads](https://pepy.tech/badge/py-txi)](https://pepy.tech/project/py-txi)
 [![PyPI - License](https://img.shields.io/pypi/l/py-txi)](https://pypi.org/project/py-txi/)
 [![Test](https://github.com/IlyasMoutawwakil/py-txi/actions/workflows/test.yaml/badge.svg)](https://github.com/IlyasMoutawwakil/py-txi/actions/workflows/tests.yaml)
```

### Comparing `py-txi-0.7.0/setup.py` & `py-txi-0.8.0/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from pathlib import Path
 
 from setuptools import find_packages, setup
 
-PY_TXI_VERSION = "0.7.0"
+PY_TXI_VERSION = "0.8.0"
 
 common_setup_kwargs = {
     "author": "Ilyas Moutawwakil",
     "author_email": "ilyas.moutawwakil@gmail.com",
     "description": "A Python wrapper around TGI and TEI servers",
     "keywords": ["tgi", "llm", "tei", "embedding", "huggingface", "docker", "python"],
     "url": "https://github.com/IlyasMoutawwakil/py-txi",
@@ -20,11 +20,11 @@
 }
 
 
 setup(
     name="py-txi",
     version=PY_TXI_VERSION,
     packages=find_packages(),
-    install_requires=["docker", "huggingface-hub", "numpy", "aiohttp", "coloredlogs"],
+    install_requires=["docker", "huggingface-hub", "numpy", "aiohttp"],
     extras_require={"quality": ["ruff"], "testing": ["pytest"]},
     **common_setup_kwargs,
 )
```

