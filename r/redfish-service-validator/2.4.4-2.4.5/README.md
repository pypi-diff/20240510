# Comparing `tmp/redfish_service_validator-2.4.4.tar.gz` & `tmp/redfish_service_validator-2.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redfish_service_validator-2.4.4.tar", last modified: Fri May  3 20:42:44 2024, max compression
+gzip compressed data, was "redfish_service_validator-2.4.5.tar", last modified: Fri May 10 19:31:54 2024, max compression
```

## Comparing `redfish_service_validator-2.4.4.tar` & `redfish_service_validator-2.4.5.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 20:42:44.293168 redfish_service_validator-2.4.4/
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-03 20:42:34.000000 redfish_service_validator-2.4.4/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (127)     3311 2024-05-03 20:42:34.000000 redfish_service_validator-2.4.4/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     9512 2024-05-03 20:42:44.293168 redfish_service_validator-2.4.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8837 2024-05-03 20:42:34.000000 redfish_service_validator-2.4.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 20:42:44.293168 redfish_service_validator-2.4.4/redfish_service_validator/
--rw-r--r--   0 runner    (1001) docker     (127)    24264 2024-05-03 20:42:34.000000 redfish_service_validator-2.4.4/redfish_service_validator/RedfishLogo.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    12074 2024-05-03 20:42:34.000000 redfish_service_validator-2.4.4/redfish_service_validator/RedfishServiceValidator.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    16498 2024-05-03 20:42:34.000000 redfish_service_validator-2.4.4/redfish_service_validator/RedfishServiceValidatorGui.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 20:42:34.000000 redfish_service_validator-2.4.4/redfish_service_validator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    50066 2024-05-03 20:42:34.000000 redfish_service_validator-2.4.4/redfish_service_validator/catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     2950 2024-05-03 20:42:34.000000 redfish_service_validator-2.4.4/redfish_service_validator/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     6475 2024-05-03 20:42:34.000000 redfish_service_validator-2.4.4/redfish_service_validator/helper.py
--rw-r--r--   0 runner    (1001) docker     (127)    23130 2024-05-03 20:42:34.000000 redfish_service_validator-2.4.4/redfish_service_validator/metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     2760 2024-05-03 20:42:34.000000 redfish_service_validator-2.4.4/redfish_service_validator/schema_pack.py
--rw-r--r--   0 runner    (1001) docker     (127)    16126 2024-05-03 20:42:34.000000 redfish_service_validator-2.4.4/redfish_service_validator/tohtml.py
--rw-r--r--   0 runner    (1001) docker     (127)    12403 2024-05-03 20:42:34.000000 redfish_service_validator-2.4.4/redfish_service_validator/traverse.py
--rw-r--r--   0 runner    (1001) docker     (127)    30785 2024-05-03 20:42:34.000000 redfish_service_validator-2.4.4/redfish_service_validator/validateRedfish.py
--rw-r--r--   0 runner    (1001) docker     (127)    23324 2024-05-03 20:42:34.000000 redfish_service_validator-2.4.4/redfish_service_validator/validateResource.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 20:42:44.293168 redfish_service_validator-2.4.4/redfish_service_validator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9512 2024-05-03 20:42:44.000000 redfish_service_validator-2.4.4/redfish_service_validator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      899 2024-05-03 20:42:44.000000 redfish_service_validator-2.4.4/redfish_service_validator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 20:42:44.000000 redfish_service_validator-2.4.4/redfish_service_validator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-05-03 20:42:44.000000 redfish_service_validator-2.4.4/redfish_service_validator.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-03 20:42:44.000000 redfish_service_validator-2.4.4/redfish_service_validator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-03 20:42:44.000000 redfish_service_validator-2.4.4/redfish_service_validator.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 20:42:44.293168 redfish_service_validator-2.4.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1351 2024-05-03 20:42:34.000000 redfish_service_validator-2.4.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 20:42:44.293168 redfish_service_validator-2.4.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     7976 2024-05-03 20:42:34.000000 redfish_service_validator-2.4.4/tests/test_catalog.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 19:31:54.909075 redfish_service_validator-2.4.5/
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-10 19:31:42.000000 redfish_service_validator-2.4.5/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3311 2024-05-10 19:31:42.000000 redfish_service_validator-2.4.5/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     9512 2024-05-10 19:31:54.909075 redfish_service_validator-2.4.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8837 2024-05-10 19:31:42.000000 redfish_service_validator-2.4.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 19:31:54.905075 redfish_service_validator-2.4.5/redfish_service_validator/
+-rw-r--r--   0 runner    (1001) docker     (127)    24264 2024-05-10 19:31:42.000000 redfish_service_validator-2.4.5/redfish_service_validator/RedfishLogo.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    12074 2024-05-10 19:31:43.000000 redfish_service_validator-2.4.5/redfish_service_validator/RedfishServiceValidator.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    16498 2024-05-10 19:31:42.000000 redfish_service_validator-2.4.5/redfish_service_validator/RedfishServiceValidatorGui.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 19:31:42.000000 redfish_service_validator-2.4.5/redfish_service_validator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50066 2024-05-10 19:31:42.000000 redfish_service_validator-2.4.5/redfish_service_validator/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2950 2024-05-10 19:31:42.000000 redfish_service_validator-2.4.5/redfish_service_validator/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6475 2024-05-10 19:31:42.000000 redfish_service_validator-2.4.5/redfish_service_validator/helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23130 2024-05-10 19:31:42.000000 redfish_service_validator-2.4.5/redfish_service_validator/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2760 2024-05-10 19:31:42.000000 redfish_service_validator-2.4.5/redfish_service_validator/schema_pack.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16126 2024-05-10 19:31:42.000000 redfish_service_validator-2.4.5/redfish_service_validator/tohtml.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12403 2024-05-10 19:31:42.000000 redfish_service_validator-2.4.5/redfish_service_validator/traverse.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30967 2024-05-10 19:31:42.000000 redfish_service_validator-2.4.5/redfish_service_validator/validateRedfish.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23324 2024-05-10 19:31:42.000000 redfish_service_validator-2.4.5/redfish_service_validator/validateResource.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 19:31:54.905075 redfish_service_validator-2.4.5/redfish_service_validator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9512 2024-05-10 19:31:54.000000 redfish_service_validator-2.4.5/redfish_service_validator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      899 2024-05-10 19:31:54.000000 redfish_service_validator-2.4.5/redfish_service_validator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 19:31:54.000000 redfish_service_validator-2.4.5/redfish_service_validator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-05-10 19:31:54.000000 redfish_service_validator-2.4.5/redfish_service_validator.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-10 19:31:54.000000 redfish_service_validator-2.4.5/redfish_service_validator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-10 19:31:54.000000 redfish_service_validator-2.4.5/redfish_service_validator.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 19:31:54.909075 redfish_service_validator-2.4.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1351 2024-05-10 19:31:43.000000 redfish_service_validator-2.4.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 19:31:54.905075 redfish_service_validator-2.4.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     7976 2024-05-10 19:31:42.000000 redfish_service_validator-2.4.5/tests/test_catalog.py
```

### Comparing `redfish_service_validator-2.4.4/LICENSE.md` & `redfish_service_validator-2.4.5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `redfish_service_validator-2.4.4/PKG-INFO` & `redfish_service_validator-2.4.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redfish_service_validator
-Version: 2.4.4
+Version: 2.4.5
 Summary: Redfish Service Validator
 Home-page: https://github.com/DMTF/Redfish-Protocol-Validator
 Author: DMTF, https://www.dmtf.org/standards/feedback
 License: BSD 3-clause "New" or "Revised License"
 Keywords: Redfish
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `redfish_service_validator-2.4.4/README.md` & `redfish_service_validator-2.4.5/README.md`

 * *Files identical despite different names*

### Comparing `redfish_service_validator-2.4.4/redfish_service_validator/RedfishLogo.py` & `redfish_service_validator-2.4.5/redfish_service_validator/RedfishLogo.py`

 * *Files identical despite different names*

### Comparing `redfish_service_validator-2.4.4/redfish_service_validator/RedfishServiceValidator.py` & `redfish_service_validator-2.4.5/redfish_service_validator/RedfishServiceValidator.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from redfish_service_validator.metadata import getSchemaDetails
 from redfish_service_validator.config import convert_config_to_args, convert_args_to_config
 from redfish_service_validator.validateResource import validateSingleURI, validateURITree
 from redfish_service_validator import tohtml, schema_pack, traverse
 from urllib.parse import urlparse
 from collections import Counter
 
-tool_version = '2.4.4'
+tool_version = '2.4.5'
 
 # Set up the custom debug levels
 VERBOSE1 = logging.INFO-1
 VERBOSE2 = logging.INFO-2
 
 logging.addLevelName(VERBOSE1, "VERBOSE1")
 logging.addLevelName(VERBOSE2, "VERBOSE2")
```

### Comparing `redfish_service_validator-2.4.4/redfish_service_validator/RedfishServiceValidatorGui.py` & `redfish_service_validator-2.4.5/redfish_service_validator/RedfishServiceValidatorGui.py`

 * *Files identical despite different names*

### Comparing `redfish_service_validator-2.4.4/redfish_service_validator/catalog.py` & `redfish_service_validator-2.4.5/redfish_service_validator/catalog.py`

 * *Files identical despite different names*

### Comparing `redfish_service_validator-2.4.4/redfish_service_validator/config.py` & `redfish_service_validator-2.4.5/redfish_service_validator/config.py`

 * *Files identical despite different names*

### Comparing `redfish_service_validator-2.4.4/redfish_service_validator/helper.py` & `redfish_service_validator-2.4.5/redfish_service_validator/helper.py`

 * *Files identical despite different names*

### Comparing `redfish_service_validator-2.4.4/redfish_service_validator/metadata.py` & `redfish_service_validator-2.4.5/redfish_service_validator/metadata.py`

 * *Files identical despite different names*

### Comparing `redfish_service_validator-2.4.4/redfish_service_validator/schema_pack.py` & `redfish_service_validator-2.4.5/redfish_service_validator/schema_pack.py`

 * *Files identical despite different names*

### Comparing `redfish_service_validator-2.4.4/redfish_service_validator/tohtml.py` & `redfish_service_validator-2.4.5/redfish_service_validator/tohtml.py`

 * *Files identical despite different names*

### Comparing `redfish_service_validator-2.4.4/redfish_service_validator/traverse.py` & `redfish_service_validator-2.4.5/redfish_service_validator/traverse.py`

 * *Files identical despite different names*

### Comparing `redfish_service_validator-2.4.4/redfish_service_validator/validateRedfish.py` & `redfish_service_validator-2.4.5/redfish_service_validator/validateRedfish.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,45 +47,47 @@
 
     return True
 
 
 def validateAction(act_fulltype, actionDecoded, all_actions):
     actionMessages, actionCounts = OrderedDict(), Counter()
     act_namespace, act_type = getNamespace(act_fulltype.strip('#')), getType(act_fulltype)
-    actPass = False
+    actPass = True
     if act_type not in all_actions:
         my_logger.error('Action {} does not exist in Namespace {}'.format(act_type, act_namespace))
         actionCounts['errorActionBadName'] += 1
         actionMessages[act_fulltype] = (
                 'Action', '-',
                 'Yes' if actionDecoded != REDFISH_ABSENT else 'No',
                 'FAIL')
     else:
         my_act = all_actions[act_type]
         actOptional = my_act.find('annotation', {'term': 'Redfish.Required'}) is not None
         if actionDecoded == REDFISH_ABSENT:
-            if actOptional:
-                actPass = True
-            else:
-                my_logger.error('{}: Mandatory action missing'.format(act_namespace))
+            if not actOptional:
+                actPass = False
+                my_logger.error('{}: Mandatory action missing'.format(act_fulltype))
                 actionCounts['failMandatoryAction'] += 1
         if actionDecoded != REDFISH_ABSENT:
             # validate target
             target = actionDecoded.get('target')
             if target is None:
-                my_logger.error('{}: target for action is missing'.format(act_namespace))
+                actPass = False
+                my_logger.error('{}: target for action is missing'.format(act_fulltype))
             elif not isinstance(target, str):
-                my_logger.error('{}: target for action is malformed'.format(act_namespace))
-                # check for unexpected properties
+                actPass = False
+                my_logger.error('{}: target for action is malformed'.format(act_fulltype))
+            # check for unexpected properties
             for ap_name in actionDecoded:
                 expected = ['target', 'title', '@Redfish.ActionInfo', '@Redfish.OperationApplyTimeSupport']
-                if ap_name not in expected and '@Redfish.AllowableValues' not in ap_name:
-                    my_logger.error('{}: Property "{}" is not allowed in actions property. \
-                        Allowed properties are "{}", "{}", "{}", "{}" and "{}"'.format(act_namespace, ap_name, *expected, '*@Redfish.AllowableValues'))
-            actPass = True
+                expected_patterns = ['@Redfish.AllowableValues', '@Redfish.AllowableNumbers', '@Redfish.AllowablePattern']
+                if ap_name not in expected and not any(pattern in ap_name for pattern in expected_patterns):
+                    actPass = False
+                    my_logger.error('{}: Property "{}" is not allowed in actions property. ' \
+                        'Allowed properties are {}, {}'.format(act_fulltype, ap_name, ', '.join(expected), ', '.join(expected_patterns)))
         if actOptional and actPass:
             actionCounts['optionalAction'] += 1
         elif actPass:
             actionCounts['passAction'] += 1
         else:
             actionCounts['failAction'] += 1
```

### Comparing `redfish_service_validator-2.4.4/redfish_service_validator/validateResource.py` & `redfish_service_validator-2.4.5/redfish_service_validator/validateResource.py`

 * *Files identical despite different names*

### Comparing `redfish_service_validator-2.4.4/redfish_service_validator.egg-info/PKG-INFO` & `redfish_service_validator-2.4.5/redfish_service_validator.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redfish_service_validator
-Version: 2.4.4
+Version: 2.4.5
 Summary: Redfish Service Validator
 Home-page: https://github.com/DMTF/Redfish-Protocol-Validator
 Author: DMTF, https://www.dmtf.org/standards/feedback
 License: BSD 3-clause "New" or "Revised License"
 Keywords: Redfish
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `redfish_service_validator-2.4.4/redfish_service_validator.egg-info/SOURCES.txt` & `redfish_service_validator-2.4.5/redfish_service_validator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `redfish_service_validator-2.4.4/setup.py` & `redfish_service_validator-2.4.5/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from codecs import open
 
 with open("README.md", "r", "utf-8") as f:
     long_description = f.read()
 
 setup(
     name="redfish_service_validator",
-    version="2.4.4",
+    version="2.4.5",
     description="Redfish Service Validator",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="DMTF, https://www.dmtf.org/standards/feedback",
     license="BSD 3-clause \"New\" or \"Revised License\"",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
```

### Comparing `redfish_service_validator-2.4.4/tests/test_catalog.py` & `redfish_service_validator-2.4.5/tests/test_catalog.py`

 * *Files identical despite different names*

