# Comparing `tmp/seam-0.6.0.tar.gz` & `tmp/seam-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seam-0.6.0.tar", max compression
+gzip compressed data, was "seam-0.6.1.tar", max compression
```

## Comparing `seam-0.6.0.tar` & `seam-0.6.1.tar`

### file list

```diff
@@ -1,42 +1,46 @@
--rw-r--r--   0        0        0     1087 2024-05-01 10:54:55.246269 seam-0.6.0/LICENSE.txt
--rw-r--r--   0        0        0     4765 2024-05-01 10:54:55.246269 seam-0.6.0/README.rst
--rw-r--r--   0        0        0      726 2024-05-01 10:54:55.250269 seam-0.6.0/pyproject.toml
--rw-r--r--   0        0        0       97 2024-05-01 10:54:55.250269 seam-0.6.0/seam/__init__.py
--rw-r--r--   0        0        0    11938 2024-05-01 10:54:55.250269 seam-0.6.0/seam/access_codes.py
--rw-r--r--   0        0        0      903 2024-05-01 10:54:55.250269 seam-0.6.0/seam/access_codes_simulate.py
--rw-r--r--   0        0        0     3979 2024-05-01 10:54:55.250269 seam-0.6.0/seam/access_codes_unmanaged.py
--rw-r--r--   0        0        0     1746 2024-05-01 10:54:55.250269 seam-0.6.0/seam/acs.py
--rw-r--r--   0        0        0     2505 2024-05-01 10:54:55.250269 seam-0.6.0/seam/acs_access_groups.py
--rw-r--r--   0        0        0      718 2024-05-01 10:54:55.250269 seam-0.6.0/seam/acs_credential_pools.py
--rw-r--r--   0        0        0     1782 2024-05-01 10:54:55.250269 seam-0.6.0/seam/acs_credential_provisioning_automations.py
--rw-r--r--   0        0        0     4763 2024-05-01 10:54:55.250269 seam-0.6.0/seam/acs_credentials.py
--rw-r--r--   0        0        0     2172 2024-05-01 10:54:55.250269 seam-0.6.0/seam/acs_entrances.py
--rw-r--r--   0        0        0      955 2024-05-01 10:54:55.250269 seam-0.6.0/seam/acs_systems.py
--rw-r--r--   0        0        0     6476 2024-05-01 10:54:55.250269 seam-0.6.0/seam/acs_users.py
--rw-r--r--   0        0        0     3255 2024-05-01 10:54:55.250269 seam-0.6.0/seam/action_attempts.py
--rw-r--r--   0        0        0     5751 2024-05-01 10:54:55.250269 seam-0.6.0/seam/client_sessions.py
--rw-r--r--   0        0        0     3292 2024-05-01 10:54:55.250269 seam-0.6.0/seam/connect_webviews.py
--rw-r--r--   0        0        0     2520 2024-05-01 10:54:55.250269 seam-0.6.0/seam/connected_accounts.py
--rw-r--r--   0        0        0     4761 2024-05-01 10:54:55.250269 seam-0.6.0/seam/devices.py
--rw-r--r--   0        0        0      517 2024-05-01 10:54:55.250269 seam-0.6.0/seam/devices_simulate.py
--rw-r--r--   0        0        0     3323 2024-05-01 10:54:55.250269 seam-0.6.0/seam/devices_unmanaged.py
--rw-r--r--   0        0        0     2385 2024-05-01 10:54:55.250269 seam-0.6.0/seam/events.py
--rw-r--r--   0        0        0     4181 2024-05-01 10:54:55.250269 seam-0.6.0/seam/locks.py
--rw-r--r--   0        0        0      765 2024-05-01 10:54:55.250269 seam-0.6.0/seam/networks.py
--rw-r--r--   0        0        0      714 2024-05-01 10:54:55.250269 seam-0.6.0/seam/noise_sensors.py
--rw-r--r--   0        0        0     4350 2024-05-01 10:54:55.250269 seam-0.6.0/seam/noise_sensors_noise_thresholds.py
--rw-r--r--   0        0        0      594 2024-05-01 10:54:55.250269 seam-0.6.0/seam/noise_sensors_simulate.py
--rw-r--r--   0        0        0     1063 2024-05-01 10:54:55.250269 seam-0.6.0/seam/phones.py
--rw-r--r--   0        0        0     1185 2024-05-01 10:54:55.250269 seam-0.6.0/seam/phones_simulate.py
--rw-r--r--   0        0        0     1535 2024-05-01 10:54:55.250269 seam-0.6.0/seam/routes.py
--rw-r--r--   0        0        0     3175 2024-05-01 10:54:55.250269 seam-0.6.0/seam/seam.py
--rw-r--r--   0        0        0     8926 2024-05-01 10:54:55.250269 seam-0.6.0/seam/thermostats.py
--rw-r--r--   0        0        0     6930 2024-05-01 10:54:55.250269 seam-0.6.0/seam/thermostats_climate_setting_schedules.py
--rw-r--r--   0        0        0    65327 2024-05-01 10:54:55.250269 seam-0.6.0/seam/types.py
--rw-r--r--   0        0        0     6700 2024-05-01 10:54:55.250269 seam-0.6.0/seam/user_identities.py
--rw-r--r--   0        0        0     2903 2024-05-01 10:54:55.250269 seam-0.6.0/seam/user_identities_enrollment_automations.py
--rw-r--r--   0        0        0      851 2024-05-01 10:54:55.250269 seam-0.6.0/seam/utils/action_attempt_errors.py
--rw-r--r--   0        0        0      864 2024-05-01 10:54:55.250269 seam-0.6.0/seam/utils/deep_attr_dict.py
--rw-r--r--   0        0        0     1815 2024-05-01 10:54:55.250269 seam-0.6.0/seam/webhooks.py
--rw-r--r--   0        0        0     2174 2024-05-01 10:54:55.250269 seam-0.6.0/seam/workspaces.py
--rw-r--r--   0        0        0     5515 1970-01-01 00:00:00.000000 seam-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1087 2024-05-09 15:11:34.619220 seam-0.6.1/LICENSE.txt
+-rw-r--r--   0        0        0     8321 2024-05-09 15:11:34.619220 seam-0.6.1/README.rst
+-rw-r--r--   0        0        0      726 2024-05-09 15:11:34.619220 seam-0.6.1/pyproject.toml
+-rw-r--r--   0        0        0      323 2024-05-09 15:11:34.619220 seam-0.6.1/seam/__init__.py
+-rw-r--r--   0        0        0    11938 2024-05-09 15:11:34.619220 seam-0.6.1/seam/access_codes.py
+-rw-r--r--   0        0        0      903 2024-05-09 15:11:34.619220 seam-0.6.1/seam/access_codes_simulate.py
+-rw-r--r--   0        0        0     3979 2024-05-09 15:11:34.619220 seam-0.6.1/seam/access_codes_unmanaged.py
+-rw-r--r--   0        0        0     1746 2024-05-09 15:11:34.619220 seam-0.6.1/seam/acs.py
+-rw-r--r--   0        0        0     2505 2024-05-09 15:11:34.619220 seam-0.6.1/seam/acs_access_groups.py
+-rw-r--r--   0        0        0      718 2024-05-09 15:11:34.619220 seam-0.6.1/seam/acs_credential_pools.py
+-rw-r--r--   0        0        0     1782 2024-05-09 15:11:34.619220 seam-0.6.1/seam/acs_credential_provisioning_automations.py
+-rw-r--r--   0        0        0     4763 2024-05-09 15:11:34.619220 seam-0.6.1/seam/acs_credentials.py
+-rw-r--r--   0        0        0     2172 2024-05-09 15:11:34.619220 seam-0.6.1/seam/acs_entrances.py
+-rw-r--r--   0        0        0      955 2024-05-09 15:11:34.619220 seam-0.6.1/seam/acs_systems.py
+-rw-r--r--   0        0        0     6476 2024-05-09 15:11:34.619220 seam-0.6.1/seam/acs_users.py
+-rw-r--r--   0        0        0     3255 2024-05-09 15:11:34.619220 seam-0.6.1/seam/action_attempts.py
+-rw-r--r--   0        0        0     3156 2024-05-09 15:11:34.619220 seam-0.6.1/seam/auth.py
+-rw-r--r--   0        0        0     5751 2024-05-09 15:11:34.619220 seam-0.6.1/seam/client_sessions.py
+-rw-r--r--   0        0        0     3292 2024-05-09 15:11:34.619220 seam-0.6.1/seam/connect_webviews.py
+-rw-r--r--   0        0        0     2520 2024-05-09 15:11:34.619220 seam-0.6.1/seam/connected_accounts.py
+-rw-r--r--   0        0        0     4761 2024-05-09 15:11:34.619220 seam-0.6.1/seam/devices.py
+-rw-r--r--   0        0        0      517 2024-05-09 15:11:34.619220 seam-0.6.1/seam/devices_simulate.py
+-rw-r--r--   0        0        0     3323 2024-05-09 15:11:34.619220 seam-0.6.1/seam/devices_unmanaged.py
+-rw-r--r--   0        0        0     2385 2024-05-09 15:11:34.619220 seam-0.6.1/seam/events.py
+-rw-r--r--   0        0        0     4181 2024-05-09 15:11:34.619220 seam-0.6.1/seam/locks.py
+-rw-r--r--   0        0        0      765 2024-05-09 15:11:34.619220 seam-0.6.1/seam/networks.py
+-rw-r--r--   0        0        0      714 2024-05-09 15:11:34.619220 seam-0.6.1/seam/noise_sensors.py
+-rw-r--r--   0        0        0     4350 2024-05-09 15:11:34.619220 seam-0.6.1/seam/noise_sensors_noise_thresholds.py
+-rw-r--r--   0        0        0      594 2024-05-09 15:11:34.619220 seam-0.6.1/seam/noise_sensors_simulate.py
+-rw-r--r--   0        0        0     1854 2024-05-09 15:11:34.619220 seam-0.6.1/seam/options.py
+-rw-r--r--   0        0        0      715 2024-05-09 15:11:34.619220 seam-0.6.1/seam/parse_options.py
+-rw-r--r--   0        0        0     1063 2024-05-09 15:11:34.619220 seam-0.6.1/seam/phones.py
+-rw-r--r--   0        0        0     1185 2024-05-09 15:11:34.619220 seam-0.6.1/seam/phones_simulate.py
+-rw-r--r--   0        0        0     1436 2024-05-09 15:11:34.619220 seam-0.6.1/seam/routes.py
+-rw-r--r--   0        0        0     3614 2024-05-09 15:11:34.619220 seam-0.6.1/seam/seam.py
+-rw-r--r--   0        0        0     8926 2024-05-09 15:11:34.619220 seam-0.6.1/seam/thermostats.py
+-rw-r--r--   0        0        0     6930 2024-05-09 15:11:34.619220 seam-0.6.1/seam/thermostats_climate_setting_schedules.py
+-rw-r--r--   0        0        0     1027 2024-05-09 15:11:34.619220 seam-0.6.1/seam/token.py
+-rw-r--r--   0        0        0    66038 2024-05-09 15:11:34.619220 seam-0.6.1/seam/types.py
+-rw-r--r--   0        0        0     6700 2024-05-09 15:11:34.619220 seam-0.6.1/seam/user_identities.py
+-rw-r--r--   0        0        0     2903 2024-05-09 15:11:34.619220 seam-0.6.1/seam/user_identities_enrollment_automations.py
+-rw-r--r--   0        0        0      851 2024-05-09 15:11:34.619220 seam-0.6.1/seam/utils/action_attempt_errors.py
+-rw-r--r--   0        0        0      864 2024-05-09 15:11:34.619220 seam-0.6.1/seam/utils/deep_attr_dict.py
+-rw-r--r--   0        0        0     1815 2024-05-09 15:11:34.619220 seam-0.6.1/seam/webhooks.py
+-rw-r--r--   0        0        0     2174 2024-05-09 15:11:34.619220 seam-0.6.1/seam/workspaces.py
+-rw-r--r--   0        0        0     9071 1970-01-01 00:00:00.000000 seam-0.6.1/PKG-INFO
```

### Comparing `seam-0.6.0/LICENSE.txt` & `seam-0.6.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `seam-0.6.0/pyproject.toml` & `seam-0.6.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "seam"
-version = "0.6.0"
+version = "0.6.1"
 description = "SDK for the Seam API written in Python."
 authors = ["Seam Labs, Inc. <engineering@getseam.com>"]
 license = "MIT"
 readme = "README.rst"
 homepage = "https://github.com/seamapi/python-next"
 repository = "https://github.com/seamapi/python-next"
```

### Comparing `seam-0.6.0/seam/access_codes.py` & `seam-0.6.1/seam/access_codes.py`

 * *Files identical despite different names*

### Comparing `seam-0.6.0/seam/access_codes_simulate.py` & `seam-0.6.1/seam/access_codes_simulate.py`

 * *Files identical despite different names*

### Comparing `seam-0.6.0/seam/access_codes_unmanaged.py` & `seam-0.6.1/seam/access_codes_unmanaged.py`

 * *Files identical despite different names*

### Comparing `seam-0.6.0/seam/acs.py` & `seam-0.6.1/seam/acs.py`

 * *Files identical despite different names*

### Comparing `seam-0.6.0/seam/acs_access_groups.py` & `seam-0.6.1/seam/acs_access_groups.py`

 * *Files identical despite different names*

### Comparing `seam-0.6.0/seam/acs_credential_pools.py` & `seam-0.6.1/seam/acs_credential_pools.py`

 * *Files identical despite different names*

### Comparing `seam-0.6.0/seam/acs_credential_provisioning_automations.py` & `seam-0.6.1/seam/acs_credential_provisioning_automations.py`

 * *Files identical despite different names*

### Comparing `seam-0.6.0/seam/acs_credentials.py` & `seam-0.6.1/seam/acs_credentials.py`

 * *Files identical despite different names*

### Comparing `seam-0.6.0/seam/acs_entrances.py` & `seam-0.6.1/seam/acs_entrances.py`

 * *Files identical despite different names*

### Comparing `seam-0.6.0/seam/acs_systems.py` & `seam-0.6.1/seam/acs_systems.py`

 * *Files identical despite different names*

### Comparing `seam-0.6.0/seam/acs_users.py` & `seam-0.6.1/seam/acs_users.py`

 * *Files identical despite different names*

### Comparing `seam-0.6.0/seam/action_attempts.py` & `seam-0.6.1/seam/action_attempts.py`

 * *Files identical despite different names*

### Comparing `seam-0.6.0/seam/client_sessions.py` & `seam-0.6.1/seam/client_sessions.py`

 * *Files identical despite different names*

### Comparing `seam-0.6.0/seam/connect_webviews.py` & `seam-0.6.1/seam/connect_webviews.py`

 * *Files identical despite different names*

### Comparing `seam-0.6.0/seam/connected_accounts.py` & `seam-0.6.1/seam/connected_accounts.py`

 * *Files identical despite different names*

### Comparing `seam-0.6.0/seam/devices.py` & `seam-0.6.1/seam/devices.py`

 * *Files identical despite different names*

### Comparing `seam-0.6.0/seam/devices_simulate.py` & `seam-0.6.1/seam/devices_simulate.py`

 * *Files identical despite different names*

### Comparing `seam-0.6.0/seam/devices_unmanaged.py` & `seam-0.6.1/seam/devices_unmanaged.py`

 * *Files identical despite different names*

### Comparing `seam-0.6.0/seam/events.py` & `seam-0.6.1/seam/events.py`

 * *Files identical despite different names*

### Comparing `seam-0.6.0/seam/locks.py` & `seam-0.6.1/seam/locks.py`

 * *Files identical despite different names*

### Comparing `seam-0.6.0/seam/networks.py` & `seam-0.6.1/seam/networks.py`

 * *Files identical despite different names*

### Comparing `seam-0.6.0/seam/noise_sensors.py` & `seam-0.6.1/seam/noise_sensors.py`

 * *Files identical despite different names*

### Comparing `seam-0.6.0/seam/noise_sensors_noise_thresholds.py` & `seam-0.6.1/seam/noise_sensors_noise_thresholds.py`

 * *Files identical despite different names*

### Comparing `seam-0.6.0/seam/noise_sensors_simulate.py` & `seam-0.6.1/seam/noise_sensors_simulate.py`

 * *Files identical despite different names*

### Comparing `seam-0.6.0/seam/phones.py` & `seam-0.6.1/seam/phones.py`

 * *Files identical despite different names*

### Comparing `seam-0.6.0/seam/phones_simulate.py` & `seam-0.6.1/seam/phones_simulate.py`

 * *Files identical despite different names*

### Comparing `seam-0.6.0/seam/routes.py` & `seam-0.6.1/seam/routes.py`

 * *Files 17% similar despite different names*

```diff
@@ -31,10 +31,7 @@
         self.networks = Networks(seam=self)
         self.noise_sensors = NoiseSensors(seam=self)
         self.phones = Phones(seam=self)
         self.thermostats = Thermostats(seam=self)
         self.user_identities = UserIdentities(seam=self)
         self.webhooks = Webhooks(seam=self)
         self.workspaces = Workspaces(seam=self)
-
-    def make_request(self, method: str, path: str, **kwargs):
-        raise NotImplementedError()
```

### Comparing `seam-0.6.0/seam/thermostats.py` & `seam-0.6.1/seam/thermostats.py`

 * *Files identical despite different names*

### Comparing `seam-0.6.0/seam/thermostats_climate_setting_schedules.py` & `seam-0.6.1/seam/thermostats_climate_setting_schedules.py`

 * *Files identical despite different names*

### Comparing `seam-0.6.0/seam/types.py` & `seam-0.6.1/seam/types.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from typing import Any, Dict, List, Optional, Union
+from typing_extensions import Self
 import abc
 from dataclasses import dataclass
 from seam.utils.deep_attr_dict import DeepAttrDict
 
 
 @dataclass
 class AccessCode:
@@ -2057,30 +2058,50 @@
     noise_sensors: AbstractNoiseSensors
     phones: AbstractPhones
     thermostats: AbstractThermostats
     user_identities: AbstractUserIdentities
     webhooks: AbstractWebhooks
     workspaces: AbstractWorkspaces
 
-    @abc.abstractmethod
-    def make_request(self, method: str, path: str, **kwargs) -> Any:
-        raise NotImplementedError
-
 
-@dataclass
 class AbstractSeam(AbstractRoutes):
-    api_key: str
-    workspace_id: str
-    api_url: str
     lts_version: str
-    wait_for_action_attempt: bool
 
     @abc.abstractmethod
     def __init__(
         self,
         api_key: Optional[str] = None,
         *,
+        personal_access_token: Optional[str] = None,
         workspace_id: Optional[str] = None,
-        api_url: Optional[str] = None,
-        wait_for_action_attempt: Optional[bool] = False,
+        endpoint: Optional[str] = None,
+        wait_for_action_attempt: Optional[Union[bool, Dict[str, float]]] = False,
     ):
+        self.wait_for_action_attempt = wait_for_action_attempt
+        self.lts_version = AbstractSeam.lts_version
+
+    @abc.abstractmethod
+    def make_request(self, method: str, path: str, **kwargs) -> Any:
+        raise NotImplementedError
+
+    @classmethod
+    @abc.abstractmethod
+    def from_api_key(
+        cls,
+        api_key: str,
+        *,
+        endpoint: Optional[str] = None,
+        wait_for_action_attempt: Optional[Union[bool, Dict[str, float]]] = False,
+    ) -> Self:
+        raise NotImplementedError
+
+    @classmethod
+    @abc.abstractmethod
+    def from_personal_access_token(
+        cls,
+        personal_access_token: str,
+        workspace_id: str,
+        *,
+        endpoint: Optional[str] = None,
+        wait_for_action_attempt: Optional[Union[bool, Dict[str, float]]] = False,
+    ) -> Self:
         raise NotImplementedError
```

### Comparing `seam-0.6.0/seam/user_identities.py` & `seam-0.6.1/seam/user_identities.py`

 * *Files identical despite different names*

### Comparing `seam-0.6.0/seam/user_identities_enrollment_automations.py` & `seam-0.6.1/seam/user_identities_enrollment_automations.py`

 * *Files identical despite different names*

### Comparing `seam-0.6.0/seam/utils/action_attempt_errors.py` & `seam-0.6.1/seam/utils/action_attempt_errors.py`

 * *Files identical despite different names*

### Comparing `seam-0.6.0/seam/utils/deep_attr_dict.py` & `seam-0.6.1/seam/utils/deep_attr_dict.py`

 * *Files identical despite different names*

### Comparing `seam-0.6.0/seam/webhooks.py` & `seam-0.6.1/seam/webhooks.py`

 * *Files identical despite different names*

### Comparing `seam-0.6.0/seam/workspaces.py` & `seam-0.6.1/seam/workspaces.py`

 * *Files identical despite different names*

