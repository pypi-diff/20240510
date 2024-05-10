# Comparing `tmp/eg_wakeonlan-1.1.tar.gz` & `tmp/eg_wakeonlan-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eg_wakeonlan-1.1.tar", last modified: Sun Apr 28 06:26:35 2024, max compression
+gzip compressed data, was "eg_wakeonlan-1.2.tar", last modified: Fri May 10 06:07:14 2024, max compression
```

## Comparing `eg_wakeonlan-1.1.tar` & `eg_wakeonlan-1.2.tar`

### file list

```diff
@@ -1,20 +1,22 @@
-drwxr-xr-x   0 eugene     (501) wheel        (0)        0 2024-04-28 06:26:35.024249 eg_wakeonlan-1.1/
--rw-r--r--   0 eugene     (501) wheel        (0)     1493 2024-04-28 06:13:06.000000 eg_wakeonlan-1.1/LICENSE.txt
--rw-r--r--   0 eugene     (501) wheel        (0)     3018 2024-04-28 06:26:35.023806 eg_wakeonlan-1.1/PKG-INFO
--rw-r--r--   0 eugene     (501) wheel        (0)     1808 2024-04-28 06:13:06.000000 eg_wakeonlan-1.1/README.md
--rw-r--r--   0 eugene     (501) wheel        (0)     1672 2024-04-28 06:13:06.000000 eg_wakeonlan-1.1/pyproject.toml
--rw-r--r--   0 eugene     (501) wheel        (0)       38 2024-04-28 06:26:35.024343 eg_wakeonlan-1.1/setup.cfg
-drwxr-xr-x   0 eugene     (501) wheel        (0)        0 2024-04-28 06:26:35.017258 eg_wakeonlan-1.1/src/
-drwxr-xr-x   0 eugene     (501) wheel        (0)        0 2024-04-28 06:26:35.023335 eg_wakeonlan-1.1/src/eg.wakeonlan.egg-info/
--rw-r--r--   0 eugene     (501) wheel        (0)     3018 2024-04-28 06:26:35.000000 eg_wakeonlan-1.1/src/eg.wakeonlan.egg-info/PKG-INFO
--rw-r--r--   0 eugene     (501) wheel        (0)      365 2024-04-28 06:26:35.000000 eg_wakeonlan-1.1/src/eg.wakeonlan.egg-info/SOURCES.txt
--rw-r--r--   0 eugene     (501) wheel        (0)        1 2024-04-28 06:26:35.000000 eg_wakeonlan-1.1/src/eg.wakeonlan.egg-info/dependency_links.txt
--rw-r--r--   0 eugene     (501) wheel        (0)       55 2024-04-28 06:26:35.000000 eg_wakeonlan-1.1/src/eg.wakeonlan.egg-info/entry_points.txt
--rw-r--r--   0 eugene     (501) wheel        (0)       10 2024-04-28 06:26:35.000000 eg_wakeonlan-1.1/src/eg.wakeonlan.egg-info/top_level.txt
-drwxr-xr-x   0 eugene     (501) wheel        (0)        0 2024-04-28 06:26:35.022194 eg_wakeonlan-1.1/src/wakeonlan/
--rw-r--r--   0 eugene     (501) wheel        (0)      321 2024-04-28 06:13:06.000000 eg_wakeonlan-1.1/src/wakeonlan/__init__.py
--rw-r--r--   0 eugene     (501) wheel        (0)      254 2024-04-28 06:13:06.000000 eg_wakeonlan-1.1/src/wakeonlan/__main__.py
--rw-r--r--   0 eugene     (501) wheel        (0)        0 2024-04-28 06:13:06.000000 eg_wakeonlan-1.1/src/wakeonlan/py.typed
--rw-r--r--   0 eugene     (501) wheel        (0)     9945 2024-04-28 06:26:21.000000 eg_wakeonlan-1.1/src/wakeonlan/wakeonlan.py
-drwxr-xr-x   0 eugene     (501) wheel        (0)        0 2024-04-28 06:26:35.022800 eg_wakeonlan-1.1/tests/
--rw-r--r--   0 eugene     (501) wheel        (0)      455 2024-04-28 06:13:06.000000 eg_wakeonlan-1.1/tests/test_wakeonlan.py
+drwxr-xr-x   0 eugene     (501) wheel        (0)        0 2024-05-10 06:07:14.965866 eg_wakeonlan-1.2/
+-rw-r--r--   0 eugene     (501) wheel        (0)      618 2024-05-10 06:07:05.000000 eg_wakeonlan-1.2/CHANGELOG.md
+-rw-r--r--   0 eugene     (501) wheel        (0)     1493 2024-04-28 06:13:06.000000 eg_wakeonlan-1.2/LICENSE.txt
+-rw-r--r--   0 eugene     (501) wheel        (0)      117 2024-05-10 05:21:53.000000 eg_wakeonlan-1.2/MANIFEST.in
+-rw-r--r--   0 eugene     (501) wheel        (0)     5534 2024-05-10 06:07:14.965324 eg_wakeonlan-1.2/PKG-INFO
+-rw-r--r--   0 eugene     (501) wheel        (0)     4324 2024-05-10 05:57:41.000000 eg_wakeonlan-1.2/README.md
+-rw-r--r--   0 eugene     (501) wheel        (0)     1671 2024-05-09 01:40:21.000000 eg_wakeonlan-1.2/pyproject.toml
+-rw-r--r--   0 eugene     (501) wheel        (0)       38 2024-05-10 06:07:14.966151 eg_wakeonlan-1.2/setup.cfg
+drwxr-xr-x   0 eugene     (501) wheel        (0)        0 2024-05-10 06:07:14.956198 eg_wakeonlan-1.2/src/
+drwxr-xr-x   0 eugene     (501) wheel        (0)        0 2024-05-10 06:07:14.964665 eg_wakeonlan-1.2/src/eg.wakeonlan.egg-info/
+-rw-r--r--   0 eugene     (501) wheel        (0)     5534 2024-05-10 06:07:14.000000 eg_wakeonlan-1.2/src/eg.wakeonlan.egg-info/PKG-INFO
+-rw-r--r--   0 eugene     (501) wheel        (0)      427 2024-05-10 06:07:14.000000 eg_wakeonlan-1.2/src/eg.wakeonlan.egg-info/SOURCES.txt
+-rw-r--r--   0 eugene     (501) wheel        (0)        1 2024-05-10 06:07:14.000000 eg_wakeonlan-1.2/src/eg.wakeonlan.egg-info/dependency_links.txt
+-rw-r--r--   0 eugene     (501) wheel        (0)       55 2024-05-10 06:07:14.000000 eg_wakeonlan-1.2/src/eg.wakeonlan.egg-info/entry_points.txt
+-rw-r--r--   0 eugene     (501) wheel        (0)       10 2024-05-10 06:07:14.000000 eg_wakeonlan-1.2/src/eg.wakeonlan.egg-info/top_level.txt
+drwxr-xr-x   0 eugene     (501) wheel        (0)        0 2024-05-10 06:07:14.964071 eg_wakeonlan-1.2/src/wakeonlan/
+-rw-r--r--   0 eugene     (501) wheel        (0)      321 2024-04-28 06:13:06.000000 eg_wakeonlan-1.2/src/wakeonlan/__init__.py
+-rw-r--r--   0 eugene     (501) wheel        (0)      254 2024-05-08 03:47:11.000000 eg_wakeonlan-1.2/src/wakeonlan/__main__.py
+-rw-r--r--   0 eugene     (501) wheel        (0)     1069 2024-05-10 05:21:53.000000 eg_wakeonlan-1.2/src/wakeonlan/autocomplete.ps1
+-rw-r--r--   0 eugene     (501) wheel        (0)     1931 2024-05-09 02:15:05.000000 eg_wakeonlan-1.2/src/wakeonlan/autocomplete.sh
+-rw-r--r--   0 eugene     (501) wheel        (0)        0 2024-04-28 06:13:06.000000 eg_wakeonlan-1.2/src/wakeonlan/py.typed
+-rw-r--r--   0 eugene     (501) wheel        (0)    12010 2024-05-10 06:07:05.000000 eg_wakeonlan-1.2/src/wakeonlan/wakeonlan.py
```

### Comparing `eg_wakeonlan-1.1/LICENSE.txt` & `eg_wakeonlan-1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `eg_wakeonlan-1.1/pyproject.toml` & `eg_wakeonlan-1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [build-system]
 requires = [
     "setuptools>=61"
 ]
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools]
-include-package-data = false
+include-package-data = true
 
 [tool.setuptools.dynamic]
 version = {attr = "wakeonlan.__version__"}
 
 [tool.setuptools.packages.find]
 where = ["src"]
```

### Comparing `eg_wakeonlan-1.1/src/wakeonlan/wakeonlan.py` & `eg_wakeonlan-1.2/src/wakeonlan/wakeonlan.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,28 +7,30 @@
 import os
 import socket
 import argparse
 import re
 import json
 import shutil
 from pathlib import Path
-from typing import Any, Dict, Sequence, Tuple, Union
+from typing import Any, Dict, Sequence, Tuple, Union, Optional
 
-VERSION = '1.1'
+VERSION = '1.2'
 
 PROG = 'wakeonlan'
 
 DESCRIPTION = 'Send Wake-On-Lan packet to a given machine'
 
 USAGE = r'''
 %(prog)s MAC [-a IPADDR] [-p PORT]
 %(prog)s NAME
 %(prog)s --save NAME MAC [-a IPADDR] [-p PORT]
 %(prog)s --delete NAME
 %(prog)s --list
+%(prog)s --names
+%(prog)s --autocomplete-source
 %(prog)s --version
 %(prog)s --help
 '''
 
 
 DEFAULT_IP = '255.255.255.255'
 DEFAULT_PORT = 9
@@ -40,53 +42,55 @@
      
 
 WAKE_CMD            = 1
 WAKE_BY_NAME_CMD    = 2
 SAVE_CMD            = 3
 DELETE_CMD          = 4
 LIST_CMD            = 5
+NAMES_CMD           = 6
+AUTOC_SOURCE        = 7
 
 MacAddress = Sequence[int]
 IPAddress = str
 Port = int
 SocketAddress = Union[Tuple[Any, ...], str, Any] #see socket._Address
 HostRecord = Tuple[MacAddress, Tuple[IPAddress, Port]] 
 
 class WakeOnLanError(Exception):
-    def __init__(self, message):
+    def __init__(self, message: str):
         super().__init__(message)
 
-def splitMac(mac):
+def splitMac(mac: str):
     return [int(x, 16) for x in mac.split(':')]
 
-def joinMac(macItems):
+def joinMac(macItems: MacAddress):
     return ':'.join([f'{x:02X}' for x in macItems])
 
 def parseArgs():
 
-    def mac_address_or_name(string):
+    def mac_address_or_name(string: str):
         if MAC_PATTERN.match(string):
             return splitMac(string)
         return string
     
-    def ip_address(string):
+    def ip_address(string: str):
         if not IP_PATTERN.match(string):
             raise argparse.ArgumentTypeError('invalid IPv4 address ' + string)
         return string
 
-    def port(string):
+    def port(string: str):
         try:
             val = int(string)
             if val < 0 or val >= 65535:
                 raise argparse.ArgumentTypeError('invalid port ' + string)
             return val
         except ValueError:
             raise argparse.ArgumentTypeError('invalid port ' + string)
 
-    def exitWithMessage(parser, message):
+    def exitWithMessage(parser: argparse.ArgumentParser, message: str):
         print(message, file=sys.stderr)
         parser.print_usage()
         sys.exit(1)
 
     parser = argparse.ArgumentParser(description=DESCRIPTION, usage=USAGE, add_help=False,
                                      prog=PROG)
     argsGroup = parser.add_argument_group('arguments')
@@ -99,16 +103,20 @@
     flagsGroup.add_argument('-p', dest='port', type=port, 
                             help='Wake-On-Lan port')
     manageGroud = flagsGroup.add_mutually_exclusive_group()
     manageGroud.add_argument('--save', '-s', type=str, dest='saveName', metavar='NAME', 
                              help='Save wake arguments as NAME')
     manageGroud.add_argument('--delete', '-d', type=str, dest='deleteName', metavar='NAME', 
                              help='Delete saved NAME')
-    manageGroud.add_argument('--list', '-l', action='store_true', dest='listNames', 
+    manageGroud.add_argument('--list', '-l', action='store_true', dest='listDefinitions', 
+                             help='List saved definitions')
+    manageGroud.add_argument('--names', '-n', action='store_true', dest='listNames', 
                              help='List saved names')
+    manageGroud.add_argument('--autocomplete-source', action='store_true', dest='autocompleteSource', 
+                             help='Print out path to a script suitable for sourcing into a shell to set up auto-complete')
     flagsGroup.add_argument('--version', action='version', version=f'%(prog)s {VERSION}')
     flagsGroup.add_argument('--help', '-h', action='help',
                             help='show this help message and exit')
     parser.set_defaults(cmd=0)
 
     args = parser.parse_args()
 
@@ -120,27 +128,44 @@
         if not args.macOrName is None:
             exitWithMessage(parser, 'parameter MAC_OR_NAME: not allowed with --delete/-d')
         if not args.ipaddr is None:
             exitWithMessage(parser, 'argument -a: not allowed with argument with --delete/-d')
         if not args.port is None:
             exitWithMessage(parser, 'argument -p: not allowed with argument with --delete/-d')
         args.cmd = DELETE_CMD
-    elif args.listNames:
+    elif args.listDefinitions:
         if not args.macOrName is None:
             exitWithMessage(parser, 'parameter MAC_OR_NAME: not allowed with --list/-l')
         if not args.ipaddr is None:
             exitWithMessage(parser, 'argument -a: not allowed with argument with --list/-l')
         if not args.port is None:
             exitWithMessage(parser, 'argument -p: not allowed with argument with --list/-l')
         args.cmd = LIST_CMD
+    elif args.listNames:
+        if not args.macOrName is None:
+            exitWithMessage(parser, 'parameter MAC_OR_NAME: not allowed with --names/-n')
+        if not args.ipaddr is None:
+            exitWithMessage(parser, 'argument -a: not allowed with argument with --names/-n')
+        if not args.port is None:
+            exitWithMessage(parser, 'argument -p: not allowed with argument with --names/-n')
+        args.cmd = NAMES_CMD
+    elif args.autocompleteSource:
+        if not args.macOrName is None:
+            exitWithMessage(parser, 'parameter MAC_OR_NAME: not allowed with --autocomplete-source')
+        if not args.ipaddr is None:
+            exitWithMessage(parser, 'argument -a: not allowed with argument with --autocomplete-source')
+        if not args.port is None:
+            exitWithMessage(parser, 'argument -p: not allowed with argument with --autocomplete-source')
+        args.cmd = AUTOC_SOURCE
+
 
     if args.cmd == 0:
-        if args.macOrName is None:
+        if args.macOrName is None: # type: ignore
             exitWithMessage(parser, 'MAC or name is required')
-        if type(args.macOrName) is list:
+        if type(args.macOrName) is list: # type: ignore
             args.cmd = WAKE_CMD
         else:
             if not args.ipaddr is None:
                 exitWithMessage(parser, 'Cannot specify broadcast address with name')
             if not args.port is None:
                 exitWithMessage(parser, 'Cannot specify port with name')
             args.cmd = WAKE_BY_NAME_CMD
@@ -159,42 +184,42 @@
     for i in range(6):
         payload[i] = 0xFF
     for i in range(6, len(payload), 6):
         payload[i:] = mac
 
     sock.sendto(payload, addr)
 
-def loadConfig():
+def loadConfig() -> Dict[Any, Any]:
     try:
         with open(CONFIG_PATH, 'rt') as config:
             config = json.load(config)
             if type(config) != dict:
                 raise WakeOnLanError(f'{CONFIG_PATH} is malformed')
-            return config
+            return config # type: ignore
     except json.JSONDecodeError:
         raise WakeOnLanError(f'{CONFIG_PATH} is malformed')
     except OSError:
         pass
     return {'names':{}}
 
-def saveConfig(config):
+def saveConfig(config: Dict[Any, Any]):
     try:
         with open(CONFIG_TMP_PATH, 'wt') as tempfile:
             json.dump(config, tempfile, indent=2)
         shutil.move(CONFIG_TMP_PATH, CONFIG_PATH)
     except OSError as err:
         raise WakeOnLanError(f'Unable to save: {err.strerror}')
 
-def getNamesDict(config):
+def getNamesDict(config: Dict[Any, Any]) -> Dict[Any, Any]:
     names = config.get('names')
     if type(names) != dict:
         raise WakeOnLanError(f'`names` not found in {CONFIG_PATH}')
-    return names
+    return names # type: ignore
 
-def parseNameRecord(name, nameRecord):
+def parseNameRecord(name: str, nameRecord: Dict[Any, Any]) -> HostRecord:
     if type(nameRecord) != dict:
         raise WakeOnLanError(f'`{name}` entry in {CONFIG_PATH} is malformed')
     mac = nameRecord.get('mac')
     if type(mac) != str or not MAC_PATTERN.match(mac):
         raise WakeOnLanError(f'mac address in `{name}` entry in {CONFIG_PATH} is missing or malformed')
     mac = splitMac(mac)
     ip = nameRecord.get('ip', DEFAULT_IP)
@@ -202,26 +227,26 @@
         raise WakeOnLanError(f'ip address in `{name}` entry in {CONFIG_PATH} is malformed')
     port = nameRecord.get('port', DEFAULT_PORT)
     if type(port) != int or port < 0 or port > 65535:
         raise WakeOnLanError(f'port address in `{name}` entry in {CONFIG_PATH} is malformed')
     
     return (mac, (ip, port))
 
-def getNameRecord(name: str) -> Union[HostRecord, None]:
+def getNameRecord(name: str) -> Optional[HostRecord]:
     config = loadConfig()
     names = getNamesDict(config)
     nameRecord = names.get(name)
     if nameRecord is None:
         return None
     return parseNameRecord(name, nameRecord)
 
 def getNames() -> Dict[str, HostRecord] :
     config = loadConfig()
     names = getNamesDict(config)
-    ret = {}
+    ret: Dict[str, HostRecord] = {}
     for name, nameRecord in names.items():
         ret[name] = parseNameRecord(name, nameRecord)
     return ret
 
 
 def saveName(name: str, mac: MacAddress, ipaddr: IPAddress, port: Port) -> None :
     config = loadConfig()
@@ -238,15 +263,15 @@
 
 def deleteName(name: str) -> None :
     config = loadConfig()
     names = getNamesDict(config)
     names.pop(name, None)
     saveConfig(config)
 
-def main():
+def main() -> int:
     args = parseArgs()
 
     try:
 
         if args.cmd == WAKE_CMD:
             print(f'wake: {args.macOrName}, {args.ipaddr}, {args.port}')
             wake(args.macOrName, (args.ipaddr, args.port))
@@ -265,11 +290,20 @@
             print(f'Name {args.deleteName} deleted')
         elif args.cmd == LIST_CMD:
             names = getNames()
             for name, nameRecord in names.items():
                 mac, addr = nameRecord
                 mac = joinMac(mac)
                 print(f'{name} - {mac}, {addr[0]}, {addr[1]}')
+        elif args.cmd == NAMES_CMD:
+            names = getNames()
+            for name in names.keys():
+                print(name)
+        elif args.cmd == AUTOC_SOURCE:
+            if not os.environ.get('PSMODULEPATH') is None:
+                print(str(Path(__file__).parent / 'autocomplete.ps1'))
+            else:
+                print(str(Path(__file__).parent / 'autocomplete.sh'))
         return 0
     except WakeOnLanError as ex:
         print(ex, file=sys.stderr)
         return 1
```

