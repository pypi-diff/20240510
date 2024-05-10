# Comparing `tmp/orca_nw_lib-1.3.6.tar.gz` & `tmp/orca_nw_lib-1.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "orca_nw_lib-1.3.6.tar", max compression
+gzip compressed data, was "orca_nw_lib-1.3.7.tar", max compression
```

## Comparing `orca_nw_lib-1.3.6.tar` & `orca_nw_lib-1.3.7.tar`

### file list

```diff
@@ -1,44 +1,44 @@
--rw-r--r--   0        0        0      626 2024-03-20 08:52:27.929603 orca_nw_lib-1.3.6/LICENSE
--rw-r--r--   0        0        0      373 2024-03-20 08:52:27.929603 orca_nw_lib-1.3.6/orca_nw_lib/__init__.py
--rw-r--r--   0        0        0    13119 2024-03-20 08:52:27.929603 orca_nw_lib-1.3.6/orca_nw_lib/bgp.py
--rw-r--r--   0        0        0     8802 2024-03-20 08:52:27.929603 orca_nw_lib-1.3.6/orca_nw_lib/bgp_db.py
--rw-r--r--   0        0        0    11419 2024-03-20 08:52:27.929603 orca_nw_lib-1.3.6/orca_nw_lib/bgp_gnmi.py
--rw-r--r--   0        0        0     1531 2024-03-20 08:52:27.929603 orca_nw_lib-1.3.6/orca_nw_lib/common.py
--rw-r--r--   0        0        0      226 2024-03-20 08:52:27.929603 orca_nw_lib-1.3.6/orca_nw_lib/constants.py
--rw-r--r--   0        0        0     1938 2024-03-20 08:52:27.929603 orca_nw_lib-1.3.6/orca_nw_lib/device.py
--rw-r--r--   0        0        0      743 2024-03-20 08:52:27.929603 orca_nw_lib-1.3.6/orca_nw_lib/device_db.py
--rw-r--r--   0        0        0     4613 2024-03-20 08:52:27.929603 orca_nw_lib-1.3.6/orca_nw_lib/device_gnmi.py
--rw-r--r--   0        0        0     6464 2024-03-20 08:52:27.929603 orca_nw_lib-1.3.6/orca_nw_lib/discovery.py
--rw-r--r--   0        0        0     4276 2024-03-20 08:52:27.929603 orca_nw_lib-1.3.6/orca_nw_lib/generate_code.py
--rw-r--r--   0        0        0     2677 2024-03-20 08:52:27.929603 orca_nw_lib-1.3.6/orca_nw_lib/github/com/openconfig/gnmi/proto/gnmi_ext/gnmi_ext_pb2.py
--rw-r--r--   0        0        0     2711 2024-03-20 08:52:27.929603 orca_nw_lib-1.3.6/orca_nw_lib/github/com/openconfig/gnmi/proto/gnmi_ext/gnmi_ext_pb2.pyi
--rw-r--r--   0        0        0      159 2024-03-20 08:52:27.929603 orca_nw_lib-1.3.6/orca_nw_lib/github.com/openconfig/gnmi/proto/gnmi_ext/gnmi_ext_pb2_grpc.py
--rw-r--r--   0        0        0    12062 2024-03-20 08:52:27.929603 orca_nw_lib-1.3.6/orca_nw_lib/gnmi_pb2.py
--rw-r--r--   0        0        0    16347 2024-03-20 08:52:27.929603 orca_nw_lib-1.3.6/orca_nw_lib/gnmi_pb2.pyi
--rw-r--r--   0        0        0     7757 2024-03-20 08:52:27.929603 orca_nw_lib-1.3.6/orca_nw_lib/gnmi_pb2_grpc.py
--rw-r--r--   0        0        0    13499 2024-03-20 08:52:27.929603 orca_nw_lib-1.3.6/orca_nw_lib/gnmi_sub.py
--rw-r--r--   0        0        0     5191 2024-03-20 08:52:27.929603 orca_nw_lib-1.3.6/orca_nw_lib/gnmi_util.py
--rw-r--r--   0        0        0     7594 2024-03-20 08:52:27.929603 orca_nw_lib-1.3.6/orca_nw_lib/graph_db_models.py
--rw-r--r--   0        0        0    10762 2024-03-20 08:52:27.929603 orca_nw_lib-1.3.6/orca_nw_lib/interface.py
--rw-r--r--   0        0        0     8327 2024-03-20 08:52:27.929603 orca_nw_lib-1.3.6/orca_nw_lib/interface_db.py
--rw-r--r--   0        0        0    15109 2024-03-20 08:52:27.929603 orca_nw_lib-1.3.6/orca_nw_lib/interface_gnmi.py
--rw-r--r--   0        0        0     7190 2024-03-20 08:52:27.929603 orca_nw_lib-1.3.6/orca_nw_lib/lldp.py
--rw-r--r--   0        0        0    12716 2024-03-20 08:52:27.929603 orca_nw_lib-1.3.6/orca_nw_lib/mclag.py
--rw-r--r--   0        0        0    11774 2024-03-20 08:52:27.929603 orca_nw_lib-1.3.6/orca_nw_lib/mclag_db.py
--rw-r--r--   0        0        0     7836 2024-03-20 08:52:27.929603 orca_nw_lib-1.3.6/orca_nw_lib/mclag_gnmi.py
--rw-r--r--   0        0        0       75 2024-03-20 08:52:27.929603 orca_nw_lib-1.3.6/orca_nw_lib/orca_exceptions.py
--rw-r--r--   0        0        0      777 2024-03-20 08:52:27.929603 orca_nw_lib-1.3.6/orca_nw_lib/orca_nw_lib.yml
--rw-r--r--   0        0        0      578 2024-03-20 08:52:27.929603 orca_nw_lib-1.3.6/orca_nw_lib/orca_nw_lib_logging.yml
--rw-r--r--   0        0        0     8967 2024-03-20 08:52:27.933603 orca_nw_lib-1.3.6/orca_nw_lib/port_chnl.py
--rw-r--r--   0        0        0     5712 2024-03-20 08:52:27.933603 orca_nw_lib-1.3.6/orca_nw_lib/port_chnl_db.py
--rw-r--r--   0        0        0     9590 2024-03-20 08:52:27.933603 orca_nw_lib-1.3.6/orca_nw_lib/port_chnl_gnmi.py
--rw-r--r--   0        0        0     5578 2024-03-20 08:52:27.933603 orca_nw_lib-1.3.6/orca_nw_lib/portgroup.py
--rw-r--r--   0        0        0     4539 2024-03-20 08:52:27.933603 orca_nw_lib-1.3.6/orca_nw_lib/portgroup_db.py
--rw-r--r--   0        0        0     3959 2024-03-20 08:52:27.933603 orca_nw_lib-1.3.6/orca_nw_lib/portgroup_gnmi.py
--rw-r--r--   0        0        0     4086 2024-03-20 08:52:27.933603 orca_nw_lib-1.3.6/orca_nw_lib/utils.py
--rw-r--r--   0        0        0     7619 2024-03-20 08:52:27.933603 orca_nw_lib-1.3.6/orca_nw_lib/vlan.py
--rw-r--r--   0        0        0     4269 2024-03-20 08:52:27.933603 orca_nw_lib-1.3.6/orca_nw_lib/vlan_db.py
--rw-r--r--   0        0        0     7687 2024-03-20 08:52:27.933603 orca_nw_lib-1.3.6/orca_nw_lib/vlan_gnmi.py
--rw-r--r--   0        0        0      508 2024-03-20 08:52:27.933603 orca_nw_lib-1.3.6/pyproject.toml
--rw-r--r--   0        0        0     7034 2024-03-20 08:52:27.933603 orca_nw_lib-1.3.6/readme.md
--rw-r--r--   0        0        0     7908 1970-01-01 00:00:00.000000 orca_nw_lib-1.3.6/PKG-INFO
+-rw-r--r--   0        0        0      626 2024-05-10 11:33:55.161769 orca_nw_lib-1.3.7/LICENSE
+-rw-r--r--   0        0        0      373 2024-05-10 11:33:55.161769 orca_nw_lib-1.3.7/orca_nw_lib/__init__.py
+-rw-r--r--   0        0        0    13119 2024-05-10 11:33:55.161769 orca_nw_lib-1.3.7/orca_nw_lib/bgp.py
+-rw-r--r--   0        0        0     8802 2024-05-10 11:33:55.161769 orca_nw_lib-1.3.7/orca_nw_lib/bgp_db.py
+-rw-r--r--   0        0        0    11382 2024-05-10 11:33:55.161769 orca_nw_lib-1.3.7/orca_nw_lib/bgp_gnmi.py
+-rw-r--r--   0        0        0     2466 2024-05-10 11:33:55.161769 orca_nw_lib-1.3.7/orca_nw_lib/common.py
+-rw-r--r--   0        0        0      226 2024-05-10 11:33:55.161769 orca_nw_lib-1.3.7/orca_nw_lib/constants.py
+-rw-r--r--   0        0        0     1938 2024-05-10 11:33:55.161769 orca_nw_lib-1.3.7/orca_nw_lib/device.py
+-rw-r--r--   0        0        0      743 2024-05-10 11:33:55.161769 orca_nw_lib-1.3.7/orca_nw_lib/device_db.py
+-rw-r--r--   0        0        0     4613 2024-05-10 11:33:55.161769 orca_nw_lib-1.3.7/orca_nw_lib/device_gnmi.py
+-rw-r--r--   0        0        0     6464 2024-05-10 11:33:55.161769 orca_nw_lib-1.3.7/orca_nw_lib/discovery.py
+-rw-r--r--   0        0        0     4276 2024-05-10 11:33:55.161769 orca_nw_lib-1.3.7/orca_nw_lib/generate_code.py
+-rw-r--r--   0        0        0     2677 2024-05-10 11:33:55.161769 orca_nw_lib-1.3.7/orca_nw_lib/github/com/openconfig/gnmi/proto/gnmi_ext/gnmi_ext_pb2.py
+-rw-r--r--   0        0        0     2711 2024-05-10 11:33:55.161769 orca_nw_lib-1.3.7/orca_nw_lib/github/com/openconfig/gnmi/proto/gnmi_ext/gnmi_ext_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-10 11:33:55.161769 orca_nw_lib-1.3.7/orca_nw_lib/github.com/openconfig/gnmi/proto/gnmi_ext/gnmi_ext_pb2_grpc.py
+-rw-r--r--   0        0        0    12062 2024-05-10 11:33:55.161769 orca_nw_lib-1.3.7/orca_nw_lib/gnmi_pb2.py
+-rw-r--r--   0        0        0    16347 2024-05-10 11:33:55.161769 orca_nw_lib-1.3.7/orca_nw_lib/gnmi_pb2.pyi
+-rw-r--r--   0        0        0     7757 2024-05-10 11:33:55.165768 orca_nw_lib-1.3.7/orca_nw_lib/gnmi_pb2_grpc.py
+-rw-r--r--   0        0        0    13499 2024-05-10 11:33:55.165768 orca_nw_lib-1.3.7/orca_nw_lib/gnmi_sub.py
+-rw-r--r--   0        0        0     5522 2024-05-10 11:33:55.165768 orca_nw_lib-1.3.7/orca_nw_lib/gnmi_util.py
+-rw-r--r--   0        0        0     7666 2024-05-10 11:33:55.165768 orca_nw_lib-1.3.7/orca_nw_lib/graph_db_models.py
+-rw-r--r--   0        0        0    12476 2024-05-10 11:33:55.165768 orca_nw_lib-1.3.7/orca_nw_lib/interface.py
+-rw-r--r--   0        0        0     8327 2024-05-10 11:33:55.165768 orca_nw_lib-1.3.7/orca_nw_lib/interface_db.py
+-rw-r--r--   0        0        0    18809 2024-05-10 11:33:55.165768 orca_nw_lib-1.3.7/orca_nw_lib/interface_gnmi.py
+-rw-r--r--   0        0        0     7190 2024-05-10 11:33:55.165768 orca_nw_lib-1.3.7/orca_nw_lib/lldp.py
+-rw-r--r--   0        0        0    12716 2024-05-10 11:33:55.165768 orca_nw_lib-1.3.7/orca_nw_lib/mclag.py
+-rw-r--r--   0        0        0    11774 2024-05-10 11:33:55.165768 orca_nw_lib-1.3.7/orca_nw_lib/mclag_db.py
+-rw-r--r--   0        0        0     7836 2024-05-10 11:33:55.165768 orca_nw_lib-1.3.7/orca_nw_lib/mclag_gnmi.py
+-rw-r--r--   0        0        0       75 2024-05-10 11:33:55.165768 orca_nw_lib-1.3.7/orca_nw_lib/orca_exceptions.py
+-rw-r--r--   0        0        0      777 2024-05-10 11:33:55.165768 orca_nw_lib-1.3.7/orca_nw_lib/orca_nw_lib.yml
+-rw-r--r--   0        0        0      577 2024-05-10 11:33:55.165768 orca_nw_lib-1.3.7/orca_nw_lib/orca_nw_lib_logging.yml
+-rw-r--r--   0        0        0     8967 2024-05-10 11:33:55.165768 orca_nw_lib-1.3.7/orca_nw_lib/port_chnl.py
+-rw-r--r--   0        0        0     5712 2024-05-10 11:33:55.165768 orca_nw_lib-1.3.7/orca_nw_lib/port_chnl_db.py
+-rw-r--r--   0        0        0     9590 2024-05-10 11:33:55.165768 orca_nw_lib-1.3.7/orca_nw_lib/port_chnl_gnmi.py
+-rw-r--r--   0        0        0     5578 2024-05-10 11:33:55.165768 orca_nw_lib-1.3.7/orca_nw_lib/portgroup.py
+-rw-r--r--   0        0        0     4539 2024-05-10 11:33:55.165768 orca_nw_lib-1.3.7/orca_nw_lib/portgroup_db.py
+-rw-r--r--   0        0        0     3959 2024-05-10 11:33:55.165768 orca_nw_lib-1.3.7/orca_nw_lib/portgroup_gnmi.py
+-rw-r--r--   0        0        0     4030 2024-05-10 11:33:55.165768 orca_nw_lib-1.3.7/orca_nw_lib/utils.py
+-rw-r--r--   0        0        0     9628 2024-05-10 11:33:55.165768 orca_nw_lib-1.3.7/orca_nw_lib/vlan.py
+-rw-r--r--   0        0        0     4455 2024-05-10 11:33:55.165768 orca_nw_lib-1.3.7/orca_nw_lib/vlan_db.py
+-rw-r--r--   0        0        0    13314 2024-05-10 11:33:55.165768 orca_nw_lib-1.3.7/orca_nw_lib/vlan_gnmi.py
+-rw-r--r--   0        0        0      508 2024-05-10 11:33:55.165768 orca_nw_lib-1.3.7/pyproject.toml
+-rw-r--r--   0        0        0     7034 2024-05-10 11:33:55.165768 orca_nw_lib-1.3.7/readme.md
+-rw-r--r--   0        0        0     7908 1970-01-01 00:00:00.000000 orca_nw_lib-1.3.7/PKG-INFO
```

### Comparing `orca_nw_lib-1.3.6/LICENSE` & `orca_nw_lib-1.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `orca_nw_lib-1.3.6/orca_nw_lib/bgp.py` & `orca_nw_lib-1.3.7/orca_nw_lib/bgp.py`

 * *Files identical despite different names*

### Comparing `orca_nw_lib-1.3.6/orca_nw_lib/bgp_db.py` & `orca_nw_lib-1.3.7/orca_nw_lib/bgp_db.py`

 * *Files identical despite different names*

### Comparing `orca_nw_lib-1.3.6/orca_nw_lib/bgp_gnmi.py` & `orca_nw_lib-1.3.7/orca_nw_lib/bgp_gnmi.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 from .gnmi_util import (
     create_gnmi_update,
     create_req_for_update,
     get_gnmi_del_req,
     send_gnmi_get,
     send_gnmi_set,
 )
-from .gnmi_pb2 import Path, PathElem
 
 
 def get_bgp_neighbor_base_path() -> Path:
     """
     Generates the base path for the BGP neighbor in the OpenConfig model.
 
     Returns:
```

### Comparing `orca_nw_lib-1.3.6/orca_nw_lib/common.py` & `orca_nw_lib-1.3.7/orca_nw_lib/common.py`

 * *Files 13% similar despite different names*

```diff
@@ -61,7 +61,48 @@
         return NotImplemented
 
     def __hash__(self):
         return hash(self.name)
 
     def __str__(self) -> str:
         return self.name
+
+
+class IFMode(str, Enum):
+    TRUNK = auto()
+    ACCESS = auto()
+
+
+    @staticmethod
+    def get_enum_from_str(name: str):
+        return IFMode[name] if name in IFMode.__members__ else None
+    
+    def __eq__(self, other):
+        if isinstance(other, self.__class__):
+            return self.name == other.name
+        return NotImplemented
+
+    def __hash__(self):
+        return hash(self.name)
+
+    def __str__(self) -> str:
+        return self.name
+
+class VlanAutoState(str, Enum):
+    enable = auto()
+    disable = auto()
+
+
+    @staticmethod
+    def get_enum_from_str(name: str):
+        return VlanAutoState[name] if name in VlanAutoState.__members__ else None
+    
+    def __eq__(self, other):
+        if isinstance(other, self.__class__):
+            return self.name == other.name
+        return NotImplemented
+
+    def __hash__(self):
+        return hash(self.name)
+
+    def __str__(self) -> str:
+        return self.name
```

### Comparing `orca_nw_lib-1.3.6/orca_nw_lib/device.py` & `orca_nw_lib-1.3.7/orca_nw_lib/device.py`

 * *Files identical despite different names*

### Comparing `orca_nw_lib-1.3.6/orca_nw_lib/device_db.py` & `orca_nw_lib-1.3.7/orca_nw_lib/device_db.py`

 * *Files identical despite different names*

### Comparing `orca_nw_lib-1.3.6/orca_nw_lib/device_gnmi.py` & `orca_nw_lib-1.3.7/orca_nw_lib/device_gnmi.py`

 * *Files identical despite different names*

### Comparing `orca_nw_lib-1.3.6/orca_nw_lib/discovery.py` & `orca_nw_lib-1.3.7/orca_nw_lib/discovery.py`

 * *Files identical despite different names*

### Comparing `orca_nw_lib-1.3.6/orca_nw_lib/generate_code.py` & `orca_nw_lib-1.3.7/orca_nw_lib/generate_code.py`

 * *Files identical despite different names*

### Comparing `orca_nw_lib-1.3.6/orca_nw_lib/github/com/openconfig/gnmi/proto/gnmi_ext/gnmi_ext_pb2.py` & `orca_nw_lib-1.3.7/orca_nw_lib/github/com/openconfig/gnmi/proto/gnmi_ext/gnmi_ext_pb2.py`

 * *Files identical despite different names*

### Comparing `orca_nw_lib-1.3.6/orca_nw_lib/github/com/openconfig/gnmi/proto/gnmi_ext/gnmi_ext_pb2.pyi` & `orca_nw_lib-1.3.7/orca_nw_lib/github/com/openconfig/gnmi/proto/gnmi_ext/gnmi_ext_pb2.pyi`

 * *Files identical despite different names*

### Comparing `orca_nw_lib-1.3.6/orca_nw_lib/gnmi_pb2.py` & `orca_nw_lib-1.3.7/orca_nw_lib/gnmi_pb2.py`

 * *Files identical despite different names*

### Comparing `orca_nw_lib-1.3.6/orca_nw_lib/gnmi_pb2.pyi` & `orca_nw_lib-1.3.7/orca_nw_lib/gnmi_pb2.pyi`

 * *Files identical despite different names*

### Comparing `orca_nw_lib-1.3.6/orca_nw_lib/gnmi_pb2_grpc.py` & `orca_nw_lib-1.3.7/orca_nw_lib/gnmi_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `orca_nw_lib-1.3.6/orca_nw_lib/gnmi_sub.py` & `orca_nw_lib-1.3.7/orca_nw_lib/gnmi_sub.py`

 * *Files identical despite different names*

### Comparing `orca_nw_lib-1.3.6/orca_nw_lib/gnmi_util.py` & `orca_nw_lib-1.3.7/orca_nw_lib/gnmi_util.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,31 @@
 import json
-import re
 import ssl
-import sys
 from typing import List
 import grpc
-from .gnmi_pb2 import JSON_IETF, GetRequest, Path, SetRequest, TypedValue, Update
+from .gnmi_pb2 import (
+    JSON_IETF,
+    GetRequest,
+    Path,
+    PathElem,
+    SetRequest,
+    TypedValue,
+    Update,
+)
 from .gnmi_pb2_grpc import gNMIStub
-
+import ast
 from .utils import (
     get_conn_timeout,
     get_logging,
     ping_ok,
     get_device_grpc_port,
     get_device_username,
     get_device_password,
 )
+import re
 
 _logger = get_logging().getLogger(__name__)
 
 stubs = {}
 
 
 def getGrpcStubs(device_ip):
@@ -120,38 +127,47 @@
         else:
             _logger.error(f"no gnmi stub found for device {device_ip}")
     except Exception as e:
         _logger.debug(f"{e} \n on device_ip : {device_ip} \n set request : {req}")
         raise
 
 
-def create_gnmi_path(path_arr: List[str]) -> List[Path]:
-    """Returns a list of gnmi path object create from string formated path array"""
-    paths = []
-    for path in path_arr:
-        gnmi_path = Path()
-
-        path_elements = path.split("/")
-        print(path_elements)
-
-        for pe_entry in path_elements:
-            if not re.match(".+?:.+?", pe_entry) and len(path_elements) == 1:
-                sys.exit(
-                    f"You haven't specified either YANG module or the top-level container in '{pe_entry}'."
-                )
-
-            elif re.match(".+?:.+?", pe_entry):
-                gnmi_path.origin = pe_entry.split(":")[0]
-                gnmi_path.elem.add(name=pe_entry.split(":")[1])
-
-            elif re.match(".+?\[.+?\]", pe_entry):
-                gnmi_path.elem.add(
-                    name=pe_entry.split("[")[0],
-                    key={
-                        f'{pe_entry.split("[")[1].split("=")[0]}': f'{re.sub("]", "", pe_entry.split("[")[1].split("=")[1])}'
-                    },
-                )
-
-            else:
-                gnmi_path.elem.add(name=pe_entry)
-            paths.append(gnmi_path)
-    return paths
+def get_gnmi_path(path: str) -> Path:
+    """
+    Generates a function comment for the given function body in a markdown code block with the correct language syntax.
+
+    Args:
+        path (str): The path to be processed.
+        Example : openconfig-interfaces:interfaces/interface[name=Vlan1]/openconfig-if-ethernet:ethernet/
+
+    Returns:
+        Path: The generated gnmi path.
+
+    """
+    path = path.strip()
+    path_elements = path.split("/")
+    gnmi_path = Path(
+        target="openconfig",
+    )
+    for pe_entry in path_elements:
+        if pe_entry in ["", "restconf", "data"]:
+            continue
+        ## When filter key is given
+        if "[" in pe_entry and "]" in pe_entry and "=" in pe_entry:
+            match = re.search(r"\[(.*?)\]", pe_entry)
+            if match:
+                key_val = match.group(1)
+                try:
+                    gnmi_path.elem.append(
+                        PathElem(
+                            name=pe_entry[: match.start()],
+                            key={key_val.split("=")[0]: key_val.split("=")[1]},
+                        )
+                    )
+                except ValueError as ve:
+                    _logger.error(
+                        f"Invalid property identifier {pe_entry} : {ve} , filter arg should be a dict-> propertykey:value"
+                    )
+                    raise
+        else:
+            gnmi_path.elem.append(PathElem(name=pe_entry))
+    return gnmi_path
```

### Comparing `orca_nw_lib-1.3.6/orca_nw_lib/graph_db_models.py` & `orca_nw_lib-1.3.7/orca_nw_lib/graph_db_models.py`

 * *Files 1% similar despite different names*

```diff
@@ -274,14 +274,16 @@
 
     vlanid = IntegerProperty()
     name = StringProperty()
     mtu = IntegerProperty()
     admin_status = StringProperty()
     oper_status = StringProperty()
     autostate = StringProperty()
+    ip_address = StringProperty()
+    sag_ip_address = StringProperty()
 
     memberInterfaces = RelationshipTo("Interface", "MEMBER_IF", model=VlanMemRel)
 
     def __eq__(self, other):
         if isinstance(other, self.__class__):
             return self.vlanid == other.vlanid
         return NotImplemented
```

### Comparing `orca_nw_lib-1.3.6/orca_nw_lib/interface.py` & `orca_nw_lib-1.3.7/orca_nw_lib/interface.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 import datetime
 from typing import Dict, List
 import pytz
 
-from .common import Speed, PortFec
+from .common import IFMode, Speed, PortFec
 from .device_db import get_device_db_obj
 from .gnmi_sub import ready_to_receive_subscription_response
 from .graph_db_models import Interface, SubInterface
 from .interface_db import (
     get_all_interfaces_of_device_from_db,
     get_interface_of_device_from_db,
     get_sub_interface_of_intfc_from_db,
     insert_device_interfaces_in_db,
 )
 from .interface_gnmi import (
     del_all_subinterfaces_of_all_interfaces_from_device,
     del_all_subinterfaces_of_interface_from_device,
     get_interface_from_device,
+    set_vlan_if_mode_on_device,
     set_interface_config_on_device,
+    remove_vlan_from_if_from_device,
 )
 from .portgroup import discover_port_groups
 from .portgroup_db import (
     get_port_group_id_of_device_interface_from_db,
     get_port_group_of_if_from_db,
 )
 from .utils import get_logging
@@ -182,15 +184,15 @@
     except Exception as e:
         _logger.error(
             f"Configuring interface {if_name} on device {device_ip} failed, Reason: {e}"
         )
         raise
     finally:
         ## discover the interface esp. the subinterfaces if there is a request to set IP
-        # on the interface because currently there are no gNMI subscription available 
+        # on the interface because currently there are no gNMI subscription available
         # for subinterface updates.
         if kwargs.get("ip"):
             discover_interfaces(device_ip, if_name)
 
 
 def del_ip_from_intf(device_ip: str, intfc_name: str):
     """
@@ -303,7 +305,56 @@
     except Exception as e:
         _logger.error(
             f"Deleting all subinterfaces of all interfaces failed, Reason: {e}"
         )
         raise
     finally:
         discover_interfaces(device_ip)
+
+
+def remove_vlan(device_ip: str, intfc_name: str, if_mode: IFMode = None):
+    """
+    Removes the VLAN from an interface.
+
+    Args:
+        device_ip (str): The IP address of the device.
+        intfc_name (str): The name of the interface.
+        if_mode (IFMode): The interface mode to remove. Defaults to None. When None is passed, All the trunk and access VLANs are removed from Interface.
+
+    Returns:
+        None
+    """
+    _logger.info(f"Removing interface mode {if_mode} from interface {intfc_name}.")
+    try:
+        remove_vlan_from_if_from_device(device_ip, intfc_name, if_mode)
+    except Exception as e:
+        _logger.error(
+            f"Removing interface mode {if_mode} from interface {intfc_name} on device {device_ip} failed, Reason: {e}"
+        )
+        raise
+    finally:
+        discover_interfaces(device_ip, intfc_name)
+
+
+def set_if_mode(device_ip: str, if_name: str, if_mode: IFMode, vlan_id: int):
+    """
+    Sets the interface mode on a device.
+
+    Args:
+        device_ip (str): The IP address of the device.
+        if_name (str): The name of the interface.
+        if_mode (IFMode): The interface mode to set.
+        vlan_id (int): The VLAN ID to set.
+
+    Returns:
+        None
+    """
+    _logger.info(f"Setting interface mode {if_mode} on interface {if_name}.")
+    try:
+        set_vlan_if_mode_on_device(device_ip, if_name, if_mode, vlan_id)
+    except Exception as e:
+        _logger.error(
+            f"Setting interface mode {if_mode} on interface {if_name} on device {device_ip} failed, Reason: {e}"
+        )
+        raise
+    finally:
+        discover_interfaces(device_ip, if_name)
```

### Comparing `orca_nw_lib-1.3.6/orca_nw_lib/interface_db.py` & `orca_nw_lib-1.3.7/orca_nw_lib/interface_db.py`

 * *Files identical despite different names*

### Comparing `orca_nw_lib-1.3.6/orca_nw_lib/interface_gnmi.py` & `orca_nw_lib-1.3.7/orca_nw_lib/interface_gnmi.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,15 @@
-from orca_nw_lib.common import PortFec, Speed
+from orca_nw_lib.common import IFMode, PortFec, Speed
 from orca_nw_lib.gnmi_pb2 import Path, PathElem
 from orca_nw_lib.interface_db import get_all_interfaces_name_of_device_from_db
 from orca_nw_lib.gnmi_util import (
     create_gnmi_update,
     create_req_for_update,
     get_gnmi_del_req,
+    get_gnmi_path,
     send_gnmi_get,
     send_gnmi_set,
     get_logging,
 )
 import orca_nw_lib.portgroup_db
 import orca_nw_lib.portgroup_gnmi
 
@@ -238,14 +239,16 @@
     mtu: int = None,
     description: str = None,
     speed: Speed = None,
     ip: str = None,
     ip_prefix_len: int = 0,
     index: int = 0,
     fec: PortFec = None,
+    if_mode: IFMode = None,
+    vlan_id: int = None,
 ):
     """
     Set the interface configuration on a device.
 
     Args:
         device_ip (str): The IP address of the device.
         if_name (str): The name of the interface.
@@ -253,15 +256,16 @@
         mtu (int, optional): The maximum transmission unit (MTU) size. Defaults to None.
         description (str, optional): The interface description. Defaults to None.
         speed (Speed, optional): The interface speed. Defaults to None.
         ip (str, optional): The IP address of the subinterface. Defaults to None.
         ip_prefix_len (int, optional): The prefix length of the IP address. Defaults to 0.
         index (int, optional): The index of the subinterface. Defaults to 0.
         fec (bool, optional): Whether to enable forward error correction. Defaults to None.
-
+        if_mode (IFMode, optional): The interface mode. Defaults to None.
+        vlan_id (int, optional): The VLAN ID of the interface. Defaults to None.
 
     Returns:
         None: If no updates were made.
         str: The response from sending the GNMI set request.
 
     """
     updates = []
@@ -358,15 +362,16 @@
         }
         updates.append(
             create_gnmi_update(
                 get_sub_interface_path(if_name),
                 ip_payload,
             )
         )
-
+    if if_mode and vlan_id:
+        updates.append(get_if_mode_req(vlan_id, if_name, if_mode))
     if updates:
         return send_gnmi_set(
             create_req_for_update(updates),
             device_ip,
         )
     else:
         return None
@@ -521,7 +526,119 @@
         intfc_name (str): The name of the interface.
 
     Returns:
         The result of the GNMI get operation for the subinterface path.
     """
 
     return send_gnmi_get(device_ip=device_ip, path=[get_sub_interface_path(intfc_name)])
+
+
+def remove_vlan_from_if_from_device(
+    device_ip: str, intfc_name: str, if_mode: IFMode = None
+):
+    """
+    Removes the interface mode from a device.
+
+    Args:
+        device_ip (str): The IP address of the device.
+        intfc_name (str): The name of the interface.
+        if_mode (IFMode): The interface mode. Defaults to None. When None is passed, All the trunk and access VLANs are removed from Interface.
+
+    Returns:
+        The result of the gNMI delete operation.
+    """
+    path = None
+    if if_mode == IFMode.ACCESS:
+        path = get_gnmi_path(
+            f"/openconfig-interfaces:interfaces/interface[name={intfc_name}]/openconfig-if-ethernet:ethernet/openconfig-vlan:switched-vlan/config/access-vlan"
+        )
+    elif if_mode == IFMode.TRUNK:
+        path = get_gnmi_path(
+            f"/openconfig-interfaces:interfaces/interface[name={intfc_name}]/openconfig-if-ethernet:ethernet/openconfig-vlan:switched-vlan/config/trunk-vlans"
+        )
+    else:
+        path = get_gnmi_path(
+            f"/openconfig-interfaces:interfaces/interface[name={intfc_name}]/openconfig-if-ethernet:ethernet/openconfig-vlan:switched-vlan"
+        )
+
+    return send_gnmi_set(
+        get_gnmi_del_req(path),
+        device_ip,
+    )
+
+
+def get_if_mode_from_device(device_ip: str, intfc_name: str):
+    """
+    Retrieves the interface mode from a device.
+
+    Args:
+        device_ip (str): The IP address of the device.
+        intfc_name (str): The name of the interface.
+
+    Returns:
+        The interface mode as a string.
+    """
+
+    return send_gnmi_get(
+        device_ip=device_ip,
+        path=[
+            get_gnmi_path(
+                f"/openconfig-interfaces:interfaces/interface[name={intfc_name}]/openconfig-if-ethernet:ethernet/openconfig-vlan:switched-vlan/config/interface-mode"
+            )
+        ],
+    )
+
+
+def get_if_mode_req(vlan_id: int, if_name: str, if_mode: IFMode):
+    """
+    Creates a GNMI update request for the interface mode.
+
+    Args:
+        vlan_id (int): The VLAN ID.
+        if_name (str): The name of the interface.
+        if_mode (IFMode): The interface mode.
+
+    Returns:
+        The GNMI update request.
+    """
+    return create_gnmi_update(
+        get_gnmi_path(
+            f"openconfig-interfaces:interfaces/interface[name={if_name}]/openconfig-if-ethernet:ethernet/openconfig-vlan:switched-vlan/config"
+        ),
+        (
+            {
+                "openconfig-vlan:config": {
+                    "interface-mode": str(if_mode),
+                    "access-vlan": vlan_id,
+                }
+            }
+            if if_mode == IFMode.ACCESS
+            else {
+                "openconfig-vlan:config": {
+                    "interface-mode": str(if_mode),
+                    "trunk-vlans": [vlan_id],
+                }
+            }
+        ),
+    )
+
+
+def set_vlan_if_mode_on_device(
+    device_ip: str, if_name: str, if_mode: IFMode, vlan_id: int
+):
+    """
+    Sets the interface mode on a device.
+
+    Args:
+        device_ip (str): The IP address of the device.
+        if_name (str): The name of the interface.
+        if_mode (IFMode): The interface mode.
+        vlan_id (int): The VLAN ID.
+
+    Returns:
+        The result of the GNMI set operation.
+    """
+
+    return send_gnmi_set(
+        create_req_for_update([get_if_mode_req(vlan_id, if_name, if_mode)]),
+        device_ip,
+    )
```

### Comparing `orca_nw_lib-1.3.6/orca_nw_lib/lldp.py` & `orca_nw_lib-1.3.7/orca_nw_lib/lldp.py`

 * *Files identical despite different names*

### Comparing `orca_nw_lib-1.3.6/orca_nw_lib/mclag.py` & `orca_nw_lib-1.3.7/orca_nw_lib/mclag.py`

 * *Files identical despite different names*

### Comparing `orca_nw_lib-1.3.6/orca_nw_lib/mclag_db.py` & `orca_nw_lib-1.3.7/orca_nw_lib/mclag_db.py`

 * *Files identical despite different names*

### Comparing `orca_nw_lib-1.3.6/orca_nw_lib/mclag_gnmi.py` & `orca_nw_lib-1.3.7/orca_nw_lib/mclag_gnmi.py`

 * *Files identical despite different names*

### Comparing `orca_nw_lib-1.3.6/orca_nw_lib/orca_nw_lib.yml` & `orca_nw_lib-1.3.7/orca_nw_lib/orca_nw_lib.yml`

 * *Files identical despite different names*

### Comparing `orca_nw_lib-1.3.6/orca_nw_lib/orca_nw_lib_logging.yml` & `orca_nw_lib-1.3.7/orca_nw_lib/orca_nw_lib_logging.yml`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
         formatter: format_1
         filename: ./orca_nw_lib.log
         maxBytes: 10485760 #10MB
         backupCount: 5
         level: INFO
     console:
         class: logging.StreamHandler
-        level: DEBUG
+        level: INFO
         formatter: format_1
         #args: (sys.stdout,)
 
 formatters:
     format_1: 
         format: "[%(asctime)s][%(levelname)s][%(filename)s:%(lineno)d][%(threadName)s] %(message)s"
```

### Comparing `orca_nw_lib-1.3.6/orca_nw_lib/port_chnl.py` & `orca_nw_lib-1.3.7/orca_nw_lib/port_chnl.py`

 * *Files identical despite different names*

### Comparing `orca_nw_lib-1.3.6/orca_nw_lib/port_chnl_db.py` & `orca_nw_lib-1.3.7/orca_nw_lib/port_chnl_db.py`

 * *Files identical despite different names*

### Comparing `orca_nw_lib-1.3.6/orca_nw_lib/port_chnl_gnmi.py` & `orca_nw_lib-1.3.7/orca_nw_lib/port_chnl_gnmi.py`

 * *Files identical despite different names*

### Comparing `orca_nw_lib-1.3.6/orca_nw_lib/portgroup.py` & `orca_nw_lib-1.3.7/orca_nw_lib/portgroup.py`

 * *Files identical despite different names*

### Comparing `orca_nw_lib-1.3.6/orca_nw_lib/portgroup_db.py` & `orca_nw_lib-1.3.7/orca_nw_lib/portgroup_db.py`

 * *Files identical despite different names*

### Comparing `orca_nw_lib-1.3.6/orca_nw_lib/portgroup_gnmi.py` & `orca_nw_lib-1.3.7/orca_nw_lib/portgroup_gnmi.py`

 * *Files identical despite different names*

### Comparing `orca_nw_lib-1.3.6/orca_nw_lib/utils.py` & `orca_nw_lib-1.3.7/orca_nw_lib/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -107,14 +107,15 @@
 
 
 import socket
 import time
 
 _logger = get_logging().getLogger(__name__)
 
+
 def ping_ok(host, max_retries=1):
     retry = 0
     status = False
     port = get_device_grpc_port()
     while retry < max_retries:
         # Create a TCP socket object
         sock = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
@@ -129,22 +130,15 @@
             status = False
             time.sleep(1)  # Wait before retrying
         finally:
             sock.close()
             return status
 
 
-def validate_ipv4_address(ip):
-    """
-    Validates an IPv4 address.
-
-    Args:
-        ip (str): The IPv4 address to be validated.
-
-    Returns:
-        bool: True if the address is a valid IPv4 address, False otherwise.
-    """
+
+def validate_and_get_ip_prefix(ip_address):
     try:
-        ipaddress.IPv4Address(ip)
-        return True
-    except ipaddress.AddressValueError:
-        return False
+        ip_network = ipaddress.ip_network(ip_address,strict=False)
+        return str(ip_network.network_address), ip_network.prefixlen
+    except ValueError:
+        _logger.error(f"Invalid IP address: {ip_address}")
+        return None, None
```

### Comparing `orca_nw_lib-1.3.6/orca_nw_lib/vlan.py` & `orca_nw_lib-1.3.7/orca_nw_lib/vlan.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 from orca_nw_lib.graph_db_models import Vlan
 from orca_nw_lib.vlan_gnmi import get_vlan_details_from_device
 
-from .common import VlanTagMode
+from .common import IFMode, VlanAutoState
 
 from .device_db import get_device_db_obj
 from .vlan_db import (
     get_vlan_obj_from_db,
     get_vlan_mem_ifcs_from_db,
     insert_vlan_in_db,
 )
 from .vlan_gnmi import (
     add_vlan_mem_interface_on_device,
     config_vlan_on_device,
-    config_vlan_tagging_mode_on_device,
     del_vlan_from_device,
     del_vlan_mem_interface_on_device,
+    get_vlan_ip_details_from_device,
+    remove_anycast_addr_from_vlan_on_device,
+    remove_ip_from_vlan_on_device,
 )
 from .utils import get_logging
 from .graph_db_models import Vlan
 
 _logger = get_logging().getLogger(__name__)
 
 
@@ -37,18 +39,40 @@
               administrative status, operational status, and autostate.
               {<vlan_db_obj>: {'ifname': 'Ethernet64', 'name': 'Vlan1', 'tagging_mode': 'tagged'}}
     """
 
     vlan_details = get_vlan_details_from_device(device_ip, vlan_name)
     vlans = []
     for vlan in vlan_details.get("sonic-vlan:VLAN_LIST") or []:
+        v_name = vlan.get("name")
+        ip_details = get_vlan_ip_details_from_device(device_ip, v_name).get(
+            "openconfig-if-ip:ipv4", {}
+        )
+        ipv4_addresses = ip_details.get("addresses", {}).get("address", [])
+        sag_ipv4_addresses = (
+            ip_details.get("openconfig-interfaces-ext:sag-ipv4", {})
+            .get("config", {})
+            .get("static-anycast-gateway", [])
+        )
+
+        ipv4_addr = None
+        for ipv4 in ipv4_addresses:
+            if (ip := ipv4.get("config", {}).get("ip", "")) and (
+                pfx := ipv4.get("config", {}).get("prefix-length", "")
+            ):
+                ipv4_addr = f"{ip}/{pfx}"
+                break
+
         vlans.append(
             Vlan(
                 vlanid=vlan.get("vlanid"),
-                name=vlan.get("name"),
+                name=v_name,
+                ip_address=ipv4_addr,
+                sag_ip_address=sag_ipv4_addresses[0] if sag_ipv4_addresses else None,
+                autostate=vlan.get("autostate", str(VlanAutoState.disable)),
             )
         )
 
     for vlan in vlan_details.get("sonic-vlan:VLAN_TABLE_LIST") or []:
         for v in vlans:
             if v.name == vlan.get("name"):
                 v.mtu = vlan.get("mtu")
@@ -92,15 +116,15 @@
 
     if isinstance(vlans, list):
         return [_getJson(device_ip, v) for v in vlans]
 
     return _getJson(device_ip, vlans)
 
 
-def del_vlan(device_ip, vlan_name:str=None):
+def del_vlan(device_ip, vlan_name: str):
     """
     Deletes a VLAN from a device.
 
     Args:
         device_ip (str): The IP address of the device.
         vlan_name (str): The name of the VLAN to be deleted.
 
@@ -113,120 +137,153 @@
     except Exception as e:
         _logger.error(f"VLAN deletion failed on device {device_ip}, Reason: {e}")
         raise
     finally:
         discover_vlan(device_ip)
 
 
-def config_vlan(
-    device_ip: str, vlan_name: str, vlan_id: int, mem_ifs: dict[str:VlanTagMode] = None
-):
+def remove_ip_from_vlan(device_ip: str, vlan_name: str, ip_address: str = None):
     """
-    Configures a VLAN on a network device.
+    Removes an IP address from a VLAN on a specific device.
 
     Args:
         device_ip (str): The IP address of the device.
         vlan_name (str): The name of the VLAN.
-        vlan_id (int): The ID of the VLAN.
-        mem_ifs (dict[str:VlanTagMode], optional): A dictionary mapping interface names to VLAN tag modes.
+        ip_address (str, optional): The IP address to be removed from the VLAN. Defaults to None.
+
+    Raises:
+        Exception: If there is an error while removing the IP address from the VLAN on the device.
 
     Returns:
         None
     """
+
     try:
-        config_vlan_on_device(device_ip, vlan_name, vlan_id, mem_ifs)
+        remove_ip_from_vlan_on_device(device_ip, vlan_name, ip_address)
     except Exception as e:
-        _logger.error(f"VLAN configuration failed on device {device_ip}, Reason: {e}")
+        _logger.error(f"VLAN IP removal failed on device {device_ip}, Reason: {e}")
         raise
     finally:
         discover_vlan(device_ip)
 
 
-def add_vlan_mem(device_ip: str, vlan_name: str, mem_ifs: dict[str:VlanTagMode]):
+def remove_anycast_ip_from_vlan(device_ip: str, vlan_name: str, anycast_ip: str = None):
     """
-    Adds the specified VLAN as a member on the given device.
+    Removes an anycast IP address from a VLAN on a specific device.
 
     Args:
         device_ip (str): The IP address of the device.
         vlan_name (str): The name of the VLAN.
-        mem_ifs (dict[str:VlanTagMode]): A dictionary mapping interface names to VLAN tag modes.
+        anycast_ip (str, optional): The anycast IP address to be removed from the VLAN. Defaults to None.
+
+    Raises:
+        Exception: If there is an error while removing the anycast IP address from the VLAN on the device.
 
     Returns:
         None
     """
+
     try:
-        add_vlan_mem_interface_on_device(device_ip, vlan_name, mem_ifs)
+        remove_anycast_addr_from_vlan_on_device(device_ip, vlan_name, anycast_ip)
     except Exception as e:
-        _logger.error(f"VLAN member addition failed on device {device_ip}, Reason: {e}")
+        _logger.error(
+            f"VLAN Anycast IP removal failed on device {device_ip}, Reason: {e}"
+        )
         raise
     finally:
         discover_vlan(device_ip)
 
 
-def get_vlan_members(device_ip, vlan_name: str):
+def config_vlan(device_ip: str, vlan_name: str, vlan_id: int, **kwargs):
     """
-    Retrieves the members of a VLAN on a specific device.
+    Configures a VLAN on a device.
 
     Args:
         device_ip (str): The IP address of the device.
         vlan_name (str): The name of the VLAN.
+        vlan_id (int): The ID of the VLAN.
+        **kwargs: Additional keyword arguments to be passed to the `config_vlan_on_device` function.
+
+    Raises:
+        Exception: If there is an error while configuring the VLAN on the device.
 
     Returns:
-        dict: A dictionary mapping member interface names to their corresponding tagging mode.
+        None
     """
-    members = get_vlan_mem_ifcs_from_db(device_ip, vlan_name)
-    mem_intf_vs_tagging_mode = {}
-    for mem in members or []:
-        mem_rel = get_vlan_obj_from_db(
-            device_ip, vlan_name
-        ).memberInterfaces.relationship(mem)
-        mem_intf_vs_tagging_mode[mem.name] = mem_rel.tagging_mode
-    return mem_intf_vs_tagging_mode
+    try:
+        config_vlan_on_device(device_ip, vlan_name, vlan_id, **kwargs)
+    except Exception as e:
+        _logger.error(f"VLAN configuration failed on device {device_ip}, Reason: {e}")
+        raise
+    finally:
+        discover_vlan(device_ip)
 
 
-def config_vlan_mem_tagging(
-    device_ip: str, vlan_name: str, if_name: str, tagging_mode: VlanTagMode
-):
+def add_vlan_mem(device_ip: str, vlan_id: int, mem_ifs: dict[str:IFMode]):
     """
-    Configures VLAN member tagging on a network device.
+    Adds VLAN members to a device.
 
     Args:
-        device_ip (str): The IP address of the network device.
-        vlan_name (str): The name of the VLAN.
-        if_name (str): The name of the interface.
-        tagging_mode (VlanTagMode): The tagging mode to be configured.
+        device_ip (str): The IP address of the device.
+        vlan_id (int): The ID of the VLAN.
+        mem_ifs (dict[str:IFMode]): A dictionary mapping interface names to their IFMode.
+
+    Raises:
+        Exception: If there is an error while adding VLAN members to the device.
 
     Returns:
         None
     """
+
     try:
-        config_vlan_tagging_mode_on_device(device_ip, vlan_name, if_name, tagging_mode)
+        add_vlan_mem_interface_on_device(device_ip, vlan_id, mem_ifs)
     except Exception as e:
-        _logger.error(
-            f"VLAN member tagging configuration failed on device {device_ip}, Reason: {e}"
-        )
+        _logger.error(f"VLAN member addition failed on device {device_ip}, Reason: {e}")
         raise
     finally:
         discover_vlan(device_ip)
 
 
-def del_vlan_mem(device_ip: str, vlan_name: str, if_name: str = None):
+def get_vlan_members(device_ip, vlan_name: str):
     """
-    Deletes a VLAN member from a device.
+    Retrieves the members of a VLAN on a specific device.
 
     Args:
         device_ip (str): The IP address of the device.
         vlan_name (str): The name of the VLAN.
-        if_name (str, optional): The name of the interface. Defaults to None.
+
+    Returns:
+        dict: A dictionary mapping member interface names to their corresponding tagging mode.
+    """
+    members = get_vlan_mem_ifcs_from_db(device_ip, vlan_name)
+    mem_intf_vs_tagging_mode = {}
+    for mem in members or []:
+        mem_rel = get_vlan_obj_from_db(
+            device_ip, vlan_name
+        ).memberInterfaces.relationship(mem)
+        mem_intf_vs_tagging_mode[mem.name] = mem_rel.tagging_mode
+    return mem_intf_vs_tagging_mode
+
+
+def del_vlan_mem(device_ip: str, vlan_id: int, if_name: str, if_mode: IFMode):
+    """
+    Deletes a VLAN member from a device.
+
+    Args:
+        device_ip (str): The IP address of the device.
+        vlan_id (int): The ID of the VLAN.
+        if_name (str): The name of the interface to be removed from the VLAN.
+        if_mode (IFMode): The mode of the interface to be removed from the VLAN.
 
     Returns:
         None
     """
-    try:
-        del_vlan_mem_interface_on_device(device_ip, vlan_name, if_name)
+    
+    try: 
+        del_vlan_mem_interface_on_device(device_ip, vlan_id, if_name, if_mode)
     except Exception as e:
         _logger.error(f"VLAN member deletion failed on device {device_ip}, Reason: {e}")
         raise
     finally:
         discover_vlan(device_ip)
```

### Comparing `orca_nw_lib-1.3.6/orca_nw_lib/vlan_db.py` & `orca_nw_lib-1.3.7/orca_nw_lib/vlan_db.py`

 * *Files 4% similar despite different names*

```diff
@@ -73,14 +73,17 @@
         None
     """
     target_vlan_obj.vlanid = source_vlan_obj.vlanid
     target_vlan_obj.name = source_vlan_obj.name
     target_vlan_obj.mtu = source_vlan_obj.mtu
     target_vlan_obj.admin_status = source_vlan_obj.admin_status
     target_vlan_obj.oper_status = source_vlan_obj.oper_status
+    target_vlan_obj.autostate = source_vlan_obj.autostate
+    target_vlan_obj.ip_address = source_vlan_obj.ip_address
+    target_vlan_obj.sag_ip_address = source_vlan_obj.sag_ip_address
 
 
 def insert_vlan_in_db(device: Device, vlans_obj_vs_mem):
     """
     Inserts VLAN information into the database.
 
     Args:
```

### Comparing `orca_nw_lib-1.3.6/readme.md` & `orca_nw_lib-1.3.7/readme.md`

 * *Files identical despite different names*

### Comparing `orca_nw_lib-1.3.6/PKG-INFO` & `orca_nw_lib-1.3.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: orca_nw_lib
-Version: 1.3.6
+Version: 1.3.7
 Summary: APIs to interact with SONiC NW
 Author: Kamal Krishna Bhatt
 Author-email: kamal.bhatt@stordis.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

