# Comparing `tmp/krkn_lib-2.1.2.tar.gz` & `tmp/krkn_lib-2.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "krkn_lib-2.1.2.tar", max compression
+gzip compressed data, was "krkn_lib-2.1.3.tar", max compression
```

## Comparing `krkn_lib-2.1.2.tar` & `krkn_lib-2.1.3.tar`

### file list

```diff
@@ -1,40 +1,42 @@
--rw-r--r--   0        0        0    10173 2024-04-18 14:24:46.633674 krkn_lib-2.1.2/LICENSE
--rw-r--r--   0        0        0     1389 2024-04-18 14:24:46.633674 krkn_lib-2.1.2/README.md
--rw-r--r--   0        0        0     1130 2024-04-18 14:26:35.366471 krkn_lib-2.1.2/pyproject.toml
--rw-r--r--   0        0        0       39 2024-04-18 14:24:46.633674 krkn_lib-2.1.2/src/krkn_lib/k8s/__init__.py
--rw-r--r--   0        0        0   108622 2024-04-18 14:26:38.090491 krkn_lib-2.1.2/src/krkn_lib/k8s/krkn_kubernetes.py
--rw-r--r--   0        0        0     7583 2024-04-18 14:26:38.090491 krkn_lib-2.1.2/src/krkn_lib/k8s/pods_monitor_pool.py
--rw-r--r--   0        0        0      462 2024-04-18 14:24:46.633674 krkn_lib-2.1.2/src/krkn_lib/k8s/templates/node_exec_pod.j2
--rw-r--r--   0        0        0        0 2024-04-18 14:24:46.633674 krkn_lib-2.1.2/src/krkn_lib/models/__init__.py
--rw-r--r--   0        0        0       30 2024-04-18 14:24:46.633674 krkn_lib-2.1.2/src/krkn_lib/models/k8s/__init__.py
--rw-r--r--   0        0        0     6557 2024-04-18 14:26:38.158492 krkn_lib-2.1.2/src/krkn_lib/models/k8s/models.py
--rw-r--r--   0        0        0       30 2024-04-18 14:24:46.633674 krkn_lib-2.1.2/src/krkn_lib/models/krkn/__init__.py
--rw-r--r--   0        0        0     2002 2024-04-18 14:24:46.633674 krkn_lib-2.1.2/src/krkn_lib/models/krkn/models.py
--rw-r--r--   0        0        0       30 2024-04-18 14:24:46.633674 krkn_lib-2.1.2/src/krkn_lib/models/telemetry/__init__.py
--rw-r--r--   0        0        0     7108 2024-04-18 14:24:46.633674 krkn_lib-2.1.2/src/krkn_lib/models/telemetry/models.py
--rw-r--r--   0        0        0       38 2024-04-18 14:24:46.637674 krkn_lib-2.1.2/src/krkn_lib/ocp/__init__.py
--rw-r--r--   0        0        0    15592 2024-04-18 14:26:38.118491 krkn_lib-2.1.2/src/krkn_lib/ocp/krkn_openshift.py
--rw-r--r--   0        0        0        0 2024-04-18 14:24:46.637674 krkn_lib-2.1.2/src/krkn_lib/prometheus/__init__.py
--rw-r--r--   0        0        0     9039 2024-04-18 14:26:38.110491 krkn_lib-2.1.2/src/krkn_lib/prometheus/krkn_prometheus.py
--rw-r--r--   0        0        0        0 2024-04-18 14:24:46.637674 krkn_lib-2.1.2/src/krkn_lib/telemetry/__init__.py
--rw-r--r--   0        0        0     1998 2024-04-18 14:26:38.094491 krkn_lib-2.1.2/src/krkn_lib/telemetry/elastic.py
--rw-r--r--   0        0        0       49 2024-04-18 14:24:46.637674 krkn_lib-2.1.2/src/krkn_lib/telemetry/k8s/__init__.py
--rw-r--r--   0        0        0    26359 2024-04-18 14:26:38.102491 krkn_lib-2.1.2/src/krkn_lib/telemetry/k8s/krkn_telemetry_kubernetes.py
--rw-r--r--   0        0        0       48 2024-04-18 14:24:46.637674 krkn_lib-2.1.2/src/krkn_lib/telemetry/ocp/__init__.py
--rw-r--r--   0        0        0     7085 2024-04-18 14:24:46.637674 krkn_lib-2.1.2/src/krkn_lib/telemetry/ocp/krkn_telemetry_openshift.py
--rw-r--r--   0        0        0       33 2024-04-18 14:24:46.637674 krkn_lib-2.1.2/src/krkn_lib/tests/__init__.py
--rw-r--r--   0        0        0    13973 2024-04-18 14:24:46.637674 krkn_lib-2.1.2/src/krkn_lib/tests/base_test.py
--rw-r--r--   0        0        0     1334 2024-04-18 14:26:38.134492 krkn_lib-2.1.2/src/krkn_lib/tests/test_krkn_elastic.py
--rw-r--r--   0        0        0    48352 2024-04-18 14:26:38.150492 krkn_lib-2.1.2/src/krkn_lib/tests/test_krkn_kubernetes.py
--rw-r--r--   0        0        0     1718 2024-04-18 14:26:38.142491 krkn_lib-2.1.2/src/krkn_lib/tests/test_krkn_kubernetes_models.py
--rw-r--r--   0        0        0     5234 2024-04-18 14:24:46.637674 krkn_lib-2.1.2/src/krkn_lib/tests/test_krkn_kubernetes_pods_monitor_pool.py
--rw-r--r--   0        0        0     3858 2024-04-18 14:24:46.637674 krkn_lib-2.1.2/src/krkn_lib/tests/test_krkn_openshift.py
--rw-r--r--   0        0        0     8807 2024-04-18 14:24:46.637674 krkn_lib-2.1.2/src/krkn_lib/tests/test_krkn_prometheus.py
--rw-r--r--   0        0        0    13447 2024-04-18 14:24:46.637674 krkn_lib-2.1.2/src/krkn_lib/tests/test_krkn_telemetry_kubernetes.py
--rw-r--r--   0        0        0     8348 2024-04-18 14:24:46.637674 krkn_lib-2.1.2/src/krkn_lib/tests/test_krkn_telemetry_models.py
--rw-r--r--   0        0        0     1961 2024-04-18 14:24:46.637674 krkn_lib-2.1.2/src/krkn_lib/tests/test_krkn_telemetry_openshift.py
--rw-r--r--   0        0        0     9874 2024-04-18 14:26:38.154492 krkn_lib-2.1.2/src/krkn_lib/tests/test_utils.py
--rw-r--r--   0        0        0       68 2024-04-18 14:24:46.637674 krkn_lib-2.1.2/src/krkn_lib/utils/__init__.py
--rw-r--r--   0        0        0    13066 2024-04-18 14:26:38.114491 krkn_lib-2.1.2/src/krkn_lib/utils/functions.py
--rw-r--r--   0        0        0     3687 2024-04-18 14:24:46.637674 krkn_lib-2.1.2/src/krkn_lib/utils/safe_logger.py
--rw-r--r--   0        0        0     2545 1970-01-01 00:00:00.000000 krkn_lib-2.1.2/PKG-INFO
+-rw-r--r--   0        0        0    10173 2024-05-10 08:39:47.391381 krkn_lib-2.1.3/LICENSE
+-rw-r--r--   0        0        0     1387 2024-05-10 08:39:47.391381 krkn_lib-2.1.3/README.md
+-rw-r--r--   0        0        0     1130 2024-05-10 08:41:28.743384 krkn_lib-2.1.3/pyproject.toml
+-rw-r--r--   0        0        0       39 2024-05-10 08:39:47.395381 krkn_lib-2.1.3/src/krkn_lib/k8s/__init__.py
+-rw-r--r--   0        0        0   116107 2024-05-10 08:41:33.023383 krkn_lib-2.1.3/src/krkn_lib/k8s/krkn_kubernetes.py
+-rw-r--r--   0        0        0     7583 2024-05-10 08:39:47.395381 krkn_lib-2.1.3/src/krkn_lib/k8s/pods_monitor_pool.py
+-rw-r--r--   0        0        0      462 2024-05-10 08:39:47.395381 krkn_lib-2.1.3/src/krkn_lib/k8s/templates/node_exec_pod.j2
+-rw-r--r--   0        0        0      146 2024-05-10 08:39:47.395381 krkn_lib-2.1.3/src/krkn_lib/k8s/templates/service_hijacking_config_map.j2
+-rw-r--r--   0        0        0      708 2024-05-10 08:39:47.395381 krkn_lib-2.1.3/src/krkn_lib/k8s/templates/service_hijacking_pod.j2
+-rw-r--r--   0        0        0        0 2024-05-10 08:39:47.395381 krkn_lib-2.1.3/src/krkn_lib/models/__init__.py
+-rw-r--r--   0        0        0       30 2024-05-10 08:39:47.395381 krkn_lib-2.1.3/src/krkn_lib/models/k8s/__init__.py
+-rw-r--r--   0        0        0     6951 2024-05-10 08:39:47.395381 krkn_lib-2.1.3/src/krkn_lib/models/k8s/models.py
+-rw-r--r--   0        0        0       30 2024-05-10 08:39:47.395381 krkn_lib-2.1.3/src/krkn_lib/models/krkn/__init__.py
+-rw-r--r--   0        0        0     2002 2024-05-10 08:39:47.395381 krkn_lib-2.1.3/src/krkn_lib/models/krkn/models.py
+-rw-r--r--   0        0        0       30 2024-05-10 08:39:47.395381 krkn_lib-2.1.3/src/krkn_lib/models/telemetry/__init__.py
+-rw-r--r--   0        0        0     7513 2024-05-10 08:39:47.395381 krkn_lib-2.1.3/src/krkn_lib/models/telemetry/models.py
+-rw-r--r--   0        0        0       38 2024-05-10 08:39:47.395381 krkn_lib-2.1.3/src/krkn_lib/ocp/__init__.py
+-rw-r--r--   0        0        0    17725 2024-05-10 08:39:47.395381 krkn_lib-2.1.3/src/krkn_lib/ocp/krkn_openshift.py
+-rw-r--r--   0        0        0        0 2024-05-10 08:39:47.395381 krkn_lib-2.1.3/src/krkn_lib/prometheus/__init__.py
+-rw-r--r--   0        0        0     9039 2024-05-10 08:39:47.395381 krkn_lib-2.1.3/src/krkn_lib/prometheus/krkn_prometheus.py
+-rw-r--r--   0        0        0        0 2024-05-10 08:39:47.395381 krkn_lib-2.1.3/src/krkn_lib/telemetry/__init__.py
+-rw-r--r--   0        0        0     1998 2024-05-10 08:39:47.395381 krkn_lib-2.1.3/src/krkn_lib/telemetry/elastic.py
+-rw-r--r--   0        0        0       49 2024-05-10 08:39:47.395381 krkn_lib-2.1.3/src/krkn_lib/telemetry/k8s/__init__.py
+-rw-r--r--   0        0        0    26359 2024-05-10 08:39:47.395381 krkn_lib-2.1.3/src/krkn_lib/telemetry/k8s/krkn_telemetry_kubernetes.py
+-rw-r--r--   0        0        0       48 2024-05-10 08:39:47.395381 krkn_lib-2.1.3/src/krkn_lib/telemetry/ocp/__init__.py
+-rw-r--r--   0        0        0     7153 2024-05-10 08:39:47.395381 krkn_lib-2.1.3/src/krkn_lib/telemetry/ocp/krkn_telemetry_openshift.py
+-rw-r--r--   0        0        0       33 2024-05-10 08:39:47.395381 krkn_lib-2.1.3/src/krkn_lib/tests/__init__.py
+-rw-r--r--   0        0        0    13973 2024-05-10 08:39:47.395381 krkn_lib-2.1.3/src/krkn_lib/tests/base_test.py
+-rw-r--r--   0        0        0     1334 2024-05-10 08:39:47.395381 krkn_lib-2.1.3/src/krkn_lib/tests/test_krkn_elastic.py
+-rw-r--r--   0        0        0    52333 2024-05-10 08:39:47.395381 krkn_lib-2.1.3/src/krkn_lib/tests/test_krkn_kubernetes.py
+-rw-r--r--   0        0        0     1718 2024-05-10 08:39:47.395381 krkn_lib-2.1.3/src/krkn_lib/tests/test_krkn_kubernetes_models.py
+-rw-r--r--   0        0        0     5233 2024-05-10 08:39:47.395381 krkn_lib-2.1.3/src/krkn_lib/tests/test_krkn_kubernetes_pods_monitor_pool.py
+-rw-r--r--   0        0        0     4020 2024-05-10 08:39:47.395381 krkn_lib-2.1.3/src/krkn_lib/tests/test_krkn_openshift.py
+-rw-r--r--   0        0        0     8807 2024-05-10 08:39:47.395381 krkn_lib-2.1.3/src/krkn_lib/tests/test_krkn_prometheus.py
+-rw-r--r--   0        0        0    13447 2024-05-10 08:39:47.395381 krkn_lib-2.1.3/src/krkn_lib/tests/test_krkn_telemetry_kubernetes.py
+-rw-r--r--   0        0        0     8348 2024-05-10 08:39:47.395381 krkn_lib-2.1.3/src/krkn_lib/tests/test_krkn_telemetry_models.py
+-rw-r--r--   0        0        0     1961 2024-05-10 08:39:47.395381 krkn_lib-2.1.3/src/krkn_lib/tests/test_krkn_telemetry_openshift.py
+-rw-r--r--   0        0        0     9874 2024-05-10 08:39:47.395381 krkn_lib-2.1.3/src/krkn_lib/tests/test_utils.py
+-rw-r--r--   0        0        0       68 2024-05-10 08:39:47.399381 krkn_lib-2.1.3/src/krkn_lib/utils/__init__.py
+-rw-r--r--   0        0        0    13066 2024-05-10 08:39:47.399381 krkn_lib-2.1.3/src/krkn_lib/utils/functions.py
+-rw-r--r--   0        0        0     3687 2024-05-10 08:39:47.399381 krkn_lib-2.1.3/src/krkn_lib/utils/safe_logger.py
+-rw-r--r--   0        0        0     2543 1970-01-01 00:00:00.000000 krkn_lib-2.1.3/PKG-INFO
```

### Comparing `krkn_lib-2.1.2/LICENSE` & `krkn_lib-2.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `krkn_lib-2.1.2/README.md` & `krkn_lib-2.1.3/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 ![action](https://github.com/krkn-chaos/krkn-lib/actions/workflows/build.yaml/badge.svg)
-![coverage](https://redhat-chaos.github.io/krkn-lib-docs/coverage_badge.svg)
+![coverage](https://krkn-chaos.github.io/krkn-lib-docs/coverage_badge.svg)
 ![PyPI](https://img.shields.io/pypi/v/krkn-lib?label=PyPi)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/krkn-lib)
 # krkn-lib
 ## Krkn Chaos and resiliency testing tool Foundation Library
 
 ### Contents
 The Library contains Classes, Models and helper functions used in [Kraken](https://github.com/redhat-chaos/krkn) to interact with
```

### Comparing `krkn_lib-2.1.2/pyproject.toml` & `krkn_lib-2.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "krkn-lib"
-version = "v2.1.2"
+version = "v2.1.3"
 description = "Foundation library for Kraken"
 authors = ["Red Hat Chaos Team"]
 license = "Apache-2.0"
 readme = "README.md"
 homepage = "https://github.com/redhat-chaos/krkn"
 #packages = [{include= "src/krkn_lib"}]
```

### Comparing `krkn_lib-2.1.2/src/krkn_lib/k8s/krkn_kubernetes.py` & `krkn_lib-2.1.3/src/krkn_lib/k8s/krkn_kubernetes.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import tempfile
 import threading
 import time
 import warnings
 from concurrent.futures import ThreadPoolExecutor, wait
 from functools import partial
 from queue import Queue
-from typing import Dict, List, Optional
+from typing import Any, Dict, List, Optional
 
 import arcaflow_lib_kubernetes
 import kubernetes
 import urllib3
 import yaml
 from jinja2 import Environment, PackageLoader
 from kubeconfig import KubeConfig
@@ -32,19 +32,20 @@
     ChaosEngine,
     ChaosResult,
     Container,
     LitmusChaosObject,
     Pod,
     PodsMonitorThread,
     PodsStatus,
+    ServiceHijacking,
     Volume,
     VolumeMount,
 )
 from krkn_lib.models.telemetry import NodeInfo, Taint
-from krkn_lib.utils import filter_dictionary
+from krkn_lib.utils import filter_dictionary, get_random_string
 from krkn_lib.utils.safe_logger import SafeLogger
 
 SERVICE_TOKEN_FILENAME = "/var/run/secrets/k8s.io/serviceaccount/token"
 SERVICE_CERT_FILENAME = "/var/run/secrets/k8s.io/serviceaccount/ca.crt"
 
 
 class KrknKubernetes:
@@ -2993,7 +2994,201 @@
         pod = AffectedPod(
             pod_name=pod_name,
             namespace=namespace,
         )
         if not event.is_set():
             pod.pod_readiness_time = end_time - start_time
         return pod
+
+    def replace_service_selector(
+        self, new_selectors: list[str], service_name: str, namespace: str
+    ) -> Optional[dict[Any]]:
+        """
+        Replaces a service selector with one or more new selectors
+        Patching the target service
+
+        :param new_selectors: a list of selectors in the format "key=value"
+        :param service_name: the service name that needs to be patched
+        :param namespace: the namespace of the service
+
+        :return: the original service spec
+            (useful to restore it after the scenario)
+            returns None if self.api_client hasn't been initialized
+        """
+
+        if self.api_client:
+            try:
+                service = self.cli.read_namespaced_service(
+                    service_name, namespace
+                )
+            except ApiException:
+                logging.error(f"{service_name} not found in {namespace}")
+                return None
+            original_service = self.api_client.sanitize_for_serialization(
+                service
+            )
+
+            splitted_selectors = [
+                s.split("=") for s in new_selectors if len(s.split("=")) == 2
+            ]
+            selectors = {}
+            for selector in splitted_selectors:
+                selectors[selector[0]] = selector[1]
+
+            if len(splitted_selectors) == 0:
+                return None
+            try:
+                body = [
+                    {
+                        "op": "replace",
+                        "path": "/spec/selector",
+                        "value": selectors,
+                    }
+                ]
+                path_params: Dict[str, str] = {}
+                query_params: List[str] = []
+                header_params: Dict[str, str] = {}
+                auth_settings = ["BearerToken"]
+                header_params["Accept"] = self.api_client.select_header_accept(
+                    ["application/json"]
+                )
+                header_params["Content-Type"] = (
+                    self.api_client.select_header_accept(
+                        ["application/json-patch+json"]
+                    )
+                )
+
+                path = (
+                    f"/api/v1/namespaces/{namespace}/services/"
+                    f"{service_name}"
+                )
+                self.api_client.call_api(
+                    path,
+                    "PATCH",
+                    path_params,
+                    query_params,
+                    header_params,
+                    body=body,
+                    response_type="str",
+                    auth_settings=auth_settings,
+                )
+
+            except ApiException as e:
+                logging.error(
+                    f"Failed to patch service, "
+                    f"Kubernetes Api Exception: {str(e)}"
+                )
+                raise e
+            if "status" in original_service:
+                original_service.pop("status")
+            if "managedFields" in original_service["metadata"]:
+                original_service["metadata"].pop("managedFields")
+            if "annotations" in original_service["metadata"]:
+                original_service["metadata"].pop("annotations")
+            if "creationTimestamp" in original_service["metadata"]:
+                original_service["metadata"].pop("creationTimestamp")
+            if "resourceVersion" in original_service["metadata"]:
+                original_service["metadata"].pop("resourceVersion")
+            if "uid" in original_service["metadata"]:
+                original_service["metadata"].pop("uid")
+            return original_service
+
+        else:
+            return None
+
+    def deploy_service_hijacking(
+        self,
+        namespace: str,
+        plan: dict[any],
+        image: str,
+        port_number: int = 5000,
+        port_name: str = "flask",
+        stats_route: str = "/stats",
+    ) -> ServiceHijacking:
+        """
+        Deploys a pod running the service-hijacking webservice
+        along with the test plan deployed in krkn stored in a
+        ConfigMap and bound as a file to the container
+
+        :param namespace: The namespace where the Pod and the
+            ConfigMap will be deployed
+        :param plan: the dictionary converted test plan to be
+            executed in the service
+        :param image: the image container image of the service
+        :param port_number: the port where the pod will be listening
+            default 5000
+        :param port_name: the port name if the Service is pointing to
+            a string name instead of a port number
+        :param stats_route: overrides the defautl route where the stats
+            action will be mapped, change it only if you have a /stats
+            route in your test_plan
+        :return: a structure containing all the infos of the
+            Pod and the ConfigMap deployment
+        """
+        pod_name = f"service-hijacking-pod-{get_random_string(5)}"
+        config_map_name = f"service-hijacking-cm-{get_random_string(5)}"
+        selector_key = "service-hijacking"
+        selector_value = f"sh-{get_random_string(5)}"
+
+        file_loader = PackageLoader("krkn_lib.k8s", "templates")
+        env = Environment(loader=file_loader, autoescape=True)
+        config_map_template = env.get_template(
+            "service_hijacking_config_map.j2"
+        )
+        plan_dump = yaml.dump(plan)
+        cm_body = yaml.safe_load(
+            config_map_template.render(
+                name=config_map_name, namespace=namespace, plan=plan_dump
+            )
+        )
+        self.cli.create_namespaced_config_map(
+            namespace=namespace, body=cm_body
+        )
+
+        pod_template = env.get_template("service_hijacking_pod.j2")
+        pod_body = yaml.safe_load(
+            pod_template.render(
+                name=pod_name,
+                namespace=namespace,
+                selector_key=selector_key,
+                selector_value=selector_value,
+                image=image,
+                port_name=port_name,
+                config_map_name=config_map_name,
+                port_number=port_number,
+                stats_route=stats_route,
+            )
+        )
+
+        self.create_pod(namespace=namespace, body=pod_body)
+
+        return ServiceHijacking(
+            pod_name=pod_name,
+            namespace=namespace,
+            selector="=".join([selector_key, selector_value]),
+            config_map_name=config_map_name,
+        )
+
+    def undeploy_service_hijacking(self, service_infos: ServiceHijacking):
+        """
+        Undeploys the resource created for the ServiceHijacking Scenario
+
+        :param service_infos: the structure returned by the
+            deploy_service_hijacking method
+        """
+        self.delete_pod(service_infos.pod_name, service_infos.namespace)
+        self.cli.delete_namespaced_config_map(
+            service_infos.config_map_name, service_infos.namespace
+        )
+
+    def service_exists(self, service_name: str, namespace: str) -> bool:
+        """
+        Checks wheter a kubernetes Service exist or not
+        :param service_name: the name of the service to check
+        :param namespace: the namespace where the service should exist
+        :return: True if the service exists, False if not
+        """
+        try:
+            _ = self.cli.read_namespaced_service(service_name, namespace)
+            return True
+        except ApiException:
+            return False
```

### Comparing `krkn_lib-2.1.2/src/krkn_lib/k8s/pods_monitor_pool.py` & `krkn_lib-2.1.3/src/krkn_lib/k8s/pods_monitor_pool.py`

 * *Files identical despite different names*

### Comparing `krkn_lib-2.1.2/src/krkn_lib/models/k8s/models.py` & `krkn_lib-2.1.3/src/krkn_lib/models/k8s/models.py`

 * *Files 4% similar despite different names*

```diff
@@ -296,7 +296,26 @@
         except Exception as e:
             pods_status = PodsStatus()
             pods_status.error = Exception(
                 f"Thread pool did not shutdown correctly,"
                 f"aborting.\nException: {e}"
             )
             return pods_status
+
+
+class ServiceHijacking:
+    pod_name: str
+    namespace: str
+    selector: str
+    config_map_name: str
+
+    def __init__(
+        self,
+        pod_name: str,
+        namespace: str,
+        selector: str,
+        config_map_name: str,
+    ):
+        self.pod_name = pod_name
+        self.namespace = namespace
+        self.selector = selector
+        self.config_map_name = config_map_name
```

### Comparing `krkn_lib-2.1.2/src/krkn_lib/models/krkn/models.py` & `krkn_lib-2.1.3/src/krkn_lib/models/krkn/models.py`

 * *Files identical despite different names*

### Comparing `krkn_lib-2.1.2/src/krkn_lib/models/telemetry/models.py` & `krkn_lib-2.1.3/src/krkn_lib/models/telemetry/models.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import base64
 import json
 from dataclasses import dataclass
+from datetime import datetime, timezone
 
 import yaml
 
 from krkn_lib.models.k8s import PodsStatus
 
 
 @dataclass(order=False)
@@ -194,39 +195,51 @@
     """
     Number of all kind of nodes in the target cluster
     """
     cloud_infrastructure: str = "Unknown"
     """
     Cloud infrastructure (if available) of the target cluster
     """
+    cloud_type: str = "self-managed"
+    """
+    Cloud Type (if available) of the target cluster: self-managed, rosa, etc
+    """
     run_uuid: str = ""
     """
     Run uuid generated by Krkn for the Run
     """
+    timestamp: str = ""
+    """
+    Current time stamp of run
+    """
 
     affected_pods: PodsStatus = PodsStatus()
 
     def __init__(self, json_object: any = None):
         self.scenarios = list[ScenarioTelemetry]()
         self.node_summary_infos = list[NodeInfo]()
         self.node_taints = list[Taint]()
         self.kubernetes_objects_count = dict[str, int]()
         self.network_plugins = ["Unknown"]
+        self.timestamp = datetime.now(timezone.utc).strftime(
+            "%Y-%m-%dT%H:%M:%SZ"
+        )
         if json_object is not None:
             scenarios = json_object.get("scenarios")
             if scenarios is None or isinstance(scenarios, list) is False:
                 raise Exception("scenarios param must be a list of object")
             for scenario in scenarios:
                 scenario_telemetry = ScenarioTelemetry(scenario)
                 self.scenarios.append(scenario_telemetry)
 
             self.node_summary_infos = json_object.get("node_summary_infos")
             self.node_taints = json_object.get("node_taints")
             self.total_node_count = json_object.get("total_node_count")
             self.cloud_infrastructure = json_object.get("cloud_infrastructure")
+            self.cloud_type = json_object.get("cloud_type")
             self.kubernetes_objects_count = json_object.get(
                 "kubernetes_objects_count"
             )
             self.network_plugins = json_object.get("network_plugins")
             self.run_uuid = json_object.get("run_uuid")
 
     def to_json(self) -> str:
```

### Comparing `krkn_lib-2.1.2/src/krkn_lib/ocp/krkn_openshift.py` & `krkn_lib-2.1.3/src/krkn_lib/ocp/krkn_openshift.py`

 * *Files 10% similar despite different names*

```diff
@@ -50,14 +50,72 @@
             return ""
         except client.exceptions.ApiException as e:
             if e.status == 404:
                 return ""
             else:
                 raise e
 
+    def get_cluster_type(self) -> str:
+        """
+        Get the cluster Cloud infrastructure type when available
+        status:
+            platformStatus:
+                aws:
+                region: us-west-2
+                resourceTags:
+                - key: prowci
+                    value: ci-rosa-**
+                - key: red-hat-clustertype
+                    value: rosa
+                - key: red-hat-managed
+                    value: "true"
+                type: AWS
+
+        :return: the cluster type (ex. rosa) or `self-managed` when unavailable
+        """
+        api_client = self.api_client
+        if api_client:
+            try:
+                path_params: dict[str, str] = {}
+                query_params: list[str] = []
+                header_params: dict[str, str] = {}
+                auth_settings = ["BearerToken"]
+                header_params["Accept"] = api_client.select_header_accept(
+                    ["application/json"]
+                )
+
+                path = "/apis/config.openshift.io/v1/infrastructures/cluster"
+                (data) = api_client.call_api(
+                    path,
+                    "GET",
+                    path_params,
+                    query_params,
+                    header_params,
+                    response_type="str",
+                    auth_settings=auth_settings,
+                )
+                json_obj = ast.literal_eval(data[0])
+                platform = json_obj["status"]["platform"].lower()
+                if (
+                    "resourceTags"
+                    in json_obj["status"]["platformStatus"][platform]
+                ):
+                    resource_tags = json_obj["status"]["platformStatus"][
+                        platform
+                    ]["resourceTags"]
+                    for rt in resource_tags:
+                        if rt["key"] == "red-hat-clustertype":
+                            return rt["value"]
+                return "self-managed"
+            except Exception as e:
+                logging.warning("V1ApiException -> %s", str(e))
+                return "self-managed"
+
+        return None
+
     def get_cloud_infrastructure(self) -> str:
         """
         Get the cluster Cloud infrastructure name when available
 
         :return: the cluster infrastructure name or `Unknown` when unavailable
         """
         api_client = self.api_client
```

### Comparing `krkn_lib-2.1.2/src/krkn_lib/prometheus/krkn_prometheus.py` & `krkn_lib-2.1.3/src/krkn_lib/prometheus/krkn_prometheus.py`

 * *Files identical despite different names*

### Comparing `krkn_lib-2.1.2/src/krkn_lib/telemetry/elastic.py` & `krkn_lib-2.1.3/src/krkn_lib/telemetry/elastic.py`

 * *Files identical despite different names*

### Comparing `krkn_lib-2.1.2/src/krkn_lib/telemetry/k8s/krkn_telemetry_kubernetes.py` & `krkn_lib-2.1.3/src/krkn_lib/telemetry/k8s/krkn_telemetry_kubernetes.py`

 * *Files identical despite different names*

### Comparing `krkn_lib-2.1.2/src/krkn_lib/telemetry/ocp/krkn_telemetry_openshift.py` & `krkn_lib-2.1.3/src/krkn_lib/telemetry/ocp/krkn_telemetry_openshift.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,14 +43,15 @@
         )
 
     def collect_cluster_metadata(self, chaos_telemetry: ChaosRunTelemetry):
         super().collect_cluster_metadata(chaos_telemetry)
         chaos_telemetry.cloud_infrastructure = (
             self.ocpcli.get_cloud_infrastructure()
         )
+        chaos_telemetry.cloud_type = self.ocpcli.get_cluster_type()
         chaos_telemetry.network_plugins = (
             self.ocpcli.get_cluster_network_plugins()
         )
 
     def put_ocp_logs(
         self,
         request_id: str,
```

### Comparing `krkn_lib-2.1.2/src/krkn_lib/tests/base_test.py` & `krkn_lib-2.1.3/src/krkn_lib/tests/base_test.py`

 * *Files identical despite different names*

### Comparing `krkn_lib-2.1.2/src/krkn_lib/tests/test_krkn_elastic.py` & `krkn_lib-2.1.3/src/krkn_lib/tests/test_krkn_elastic.py`

 * *Files identical despite different names*

### Comparing `krkn_lib-2.1.2/src/krkn_lib/tests/test_krkn_kubernetes.py` & `krkn_lib-2.1.3/src/krkn_lib/tests/test_krkn_kubernetes.py`

 * *Files 2% similar despite different names*

```diff
@@ -1193,10 +1193,111 @@
         self.background_delete_pod(delayed_3, namespace)
         self.background_delete_pod(delayed_respawn_1, namespace)
         self.background_delete_pod(delayed_respawn_2, namespace)
         self.assertIsNotNone(result.error)
         self.assertEqual(len(result.unrecovered), 0)
         self.assertEqual(len(result.recovered), 0)
 
+    def test_replace_service_selector(self):
+        namespace = "test-" + self.get_random_string(10)
+        name = "test-" + self.get_random_string(10)
+        self.deploy_namespace(namespace, [])
+        self.deploy_service(name, namespace)
+        self.lib_k8s.replace_service_selector(
+            ["app=selector", "test=replace"], name, namespace
+        )
+
+        service = self.lib_k8s.cli.read_namespaced_service(name, namespace)
+        sanitized_service = self.lib_k8s.api_client.sanitize_for_serialization(
+            service
+        )
+        self.assertEqual(len(sanitized_service["spec"]["selector"].keys()), 2)
+        self.assertTrue("app" in sanitized_service["spec"]["selector"])
+        self.assertEqual(
+            sanitized_service["spec"]["selector"]["app"], "selector"
+        )
+        self.assertTrue("test" in sanitized_service["spec"]["selector"])
+        self.assertEqual(
+            sanitized_service["spec"]["selector"]["test"], "replace"
+        )
+
+        # test None result with non-existent service
+
+        none_result = self.lib_k8s.replace_service_selector(
+            ["app=selector"], "doesnotexist", "doesnotexist"
+        )
+        self.assertIsNone(none_result)
+
+        # test None result with empty selector list
+        none_result = self.lib_k8s.replace_service_selector(
+            [], name, namespace
+        )
+        self.assertIsNone(none_result)
+
+        # test selector validation (bad_selector will be ignored)
+        self.lib_k8s.replace_service_selector(
+            ["bad_selector", "good=selector"], name, namespace
+        )
+        service = self.lib_k8s.cli.read_namespaced_service(name, namespace)
+        sanitized_service = self.lib_k8s.api_client.sanitize_for_serialization(
+            service
+        )
+        self.assertEqual(len(sanitized_service["spec"]["selector"].keys()), 1)
+        self.assertTrue("good" in sanitized_service["spec"]["selector"])
+        self.assertEqual(
+            sanitized_service["spec"]["selector"]["good"], "selector"
+        )
+
+    def test_deploy_undeploy_service_hijacking(self):
+        # test deploy
+        namespace = "test-" + self.get_random_string(10)
+        self.deploy_namespace(namespace, [])
+        with open("src/testdata/service_hijacking_test_plan.yaml") as stream:
+            plan = yaml.safe_load(stream)
+
+        service_infos = self.lib_k8s.deploy_service_hijacking(
+            namespace,
+            plan,
+            "quay.io/redhat-chaos/krkn-service-hijacking:v0.1.0",
+        )
+
+        self.assertIsNotNone(service_infos)
+        self.assertIsNotNone(service_infos.config_map_name)
+        self.assertIsNotNone(service_infos.selector)
+        self.assertIsNotNone(service_infos.pod_name)
+        self.assertIsNotNone(service_infos.namespace)
+
+        pod_infos = self.lib_k8s.get_pod_info(
+            service_infos.pod_name, service_infos.namespace
+        )
+        config_map_infos = self.lib_k8s.cli.read_namespaced_config_map(
+            service_infos.config_map_name, service_infos.namespace
+        )
+        self.assertIsNotNone(pod_infos)
+        self.assertIsNotNone(config_map_infos)
+
+        # test undeploy
+        self.lib_k8s.undeploy_service_hijacking(service_infos)
+
+        pod_infos = self.lib_k8s.get_pod_info(
+            service_infos.pod_name, service_infos.namespace
+        )
+
+        self.assertIsNone(pod_infos)
+        with self.assertRaises(ApiException):
+            self.lib_k8s.cli.read_namespaced_config_map(
+                service_infos.config_map_name, service_infos.namespace
+            )
+
+    def test_service_exists(self):
+        namespace = "test-" + self.get_random_string(10)
+        name = "test-" + self.get_random_string(10)
+        self.deploy_namespace(namespace, [])
+        self.deploy_service(name, namespace)
+        self.assertTrue(self.lib_k8s.service_exists(name, namespace))
+        self.assertFalse(
+            self.lib_k8s.service_exists("doesnotexist", "doesnotexist")
+        )
+
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `krkn_lib-2.1.2/src/krkn_lib/tests/test_krkn_kubernetes_models.py` & `krkn_lib-2.1.3/src/krkn_lib/tests/test_krkn_kubernetes_models.py`

 * *Files identical despite different names*

### Comparing `krkn_lib-2.1.2/src/krkn_lib/tests/test_krkn_kubernetes_pods_monitor_pool.py` & `krkn_lib-2.1.3/src/krkn_lib/tests/test_krkn_kubernetes_pods_monitor_pool.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import time
 
 from krkn_lib.k8s.pods_monitor_pool import PodsMonitorPool
 from krkn_lib.tests import BaseTest
 
 
 class TestKrknKubernetesPodsMonitorPool(BaseTest):
-
     def test_pods_monitor_pool(self):
         namespace_1 = "test-pool-ns-0-" + self.get_random_string(10)
         label_1 = "readiness-1"
         delayed_1 = "delayed-pool-0-1-" + self.get_random_string(10)
         delayed_2 = "delayed-pool-0-2-" + self.get_random_string(10)
 
         delayed_1_respawn = "delayed-pool-0-r-2-" + self.get_random_string(10)
```

### Comparing `krkn_lib-2.1.2/src/krkn_lib/tests/test_krkn_openshift.py` & `krkn_lib-2.1.3/src/krkn_lib/tests/test_krkn_openshift.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,14 +12,19 @@
         self.assertIsNotNone(result)
 
     def test_get_cluster_network_plugins(self):
         resp = self.lib_ocp.get_cluster_network_plugins()
         self.assertTrue(len(resp) > 0)
         self.assertEqual(resp[0], "Unknown")
 
+    def test_get_cluster_type(self):
+        resp = self.lib_ocp.get_cluster_type()
+        self.assertTrue(resp)
+        self.assertEqual(resp, "self-managed")
+
     def test_get_cloud_infrastructure(self):
         resp = self.lib_ocp.get_cloud_infrastructure()
         self.assertTrue(resp)
         self.assertEqual(resp, "Unknown")
 
     def test_filter_must_gather_ocp_log_folder(self):
         # 1694473200 12 Sep 2023 01:00 AM GMT+2
```

### Comparing `krkn_lib-2.1.2/src/krkn_lib/tests/test_krkn_prometheus.py` & `krkn_lib-2.1.3/src/krkn_lib/tests/test_krkn_prometheus.py`

 * *Files identical despite different names*

### Comparing `krkn_lib-2.1.2/src/krkn_lib/tests/test_krkn_telemetry_kubernetes.py` & `krkn_lib-2.1.3/src/krkn_lib/tests/test_krkn_telemetry_kubernetes.py`

 * *Files identical despite different names*

### Comparing `krkn_lib-2.1.2/src/krkn_lib/tests/test_krkn_telemetry_models.py` & `krkn_lib-2.1.3/src/krkn_lib/tests/test_krkn_telemetry_models.py`

 * *Files identical despite different names*

### Comparing `krkn_lib-2.1.2/src/krkn_lib/tests/test_krkn_telemetry_openshift.py` & `krkn_lib-2.1.3/src/krkn_lib/tests/test_krkn_telemetry_openshift.py`

 * *Files identical despite different names*

### Comparing `krkn_lib-2.1.2/src/krkn_lib/tests/test_utils.py` & `krkn_lib-2.1.3/src/krkn_lib/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `krkn_lib-2.1.2/src/krkn_lib/utils/functions.py` & `krkn_lib-2.1.3/src/krkn_lib/utils/functions.py`

 * *Files identical despite different names*

### Comparing `krkn_lib-2.1.2/src/krkn_lib/utils/safe_logger.py` & `krkn_lib-2.1.3/src/krkn_lib/utils/safe_logger.py`

 * *Files identical despite different names*

### Comparing `krkn_lib-2.1.2/PKG-INFO` & `krkn_lib-2.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: krkn-lib
-Version: 2.1.2
+Version: 2.1.3
 Summary: Foundation library for Kraken
 Home-page: https://github.com/redhat-chaos/krkn
 License: Apache-2.0
 Author: Red Hat Chaos Team
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
@@ -25,15 +25,15 @@
 Requires-Dist: sphinx-rtd-theme (>=1.2.2,<2.0.0)
 Requires-Dist: sphinxnotes-markdown-builder (>=0.5.6,<0.6.0)
 Requires-Dist: tzlocal (==5.1)
 Requires-Dist: wheel (>=0.42.0,<0.43.0)
 Description-Content-Type: text/markdown
 
 ![action](https://github.com/krkn-chaos/krkn-lib/actions/workflows/build.yaml/badge.svg)
-![coverage](https://redhat-chaos.github.io/krkn-lib-docs/coverage_badge.svg)
+![coverage](https://krkn-chaos.github.io/krkn-lib-docs/coverage_badge.svg)
 ![PyPI](https://img.shields.io/pypi/v/krkn-lib?label=PyPi)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/krkn-lib)
 # krkn-lib
 ## Krkn Chaos and resiliency testing tool Foundation Library
 
 ### Contents
 The Library contains Classes, Models and helper functions used in [Kraken](https://github.com/redhat-chaos/krkn) to interact with
```

