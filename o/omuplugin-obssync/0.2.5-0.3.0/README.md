# Comparing `tmp/omuplugin_obssync-0.2.5.tar.gz` & `tmp/omuplugin_obssync-0.3.0.tar.gz`

## Comparing `omuplugin_obssync-0.2.5.tar` & `omuplugin_obssync-0.3.0.tar`

### file list

```diff
@@ -1,7 +1,8 @@
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 omuplugin_obssync-0.2.5/src/omuplugin_obssync/__init__.py
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 omuplugin_obssync-0.2.5/src/omuplugin_obssync/__main__.py
--rw-r--r--   0        0        0     2593 2020-02-02 00:00:00.000000 omuplugin_obssync-0.2.5/src/omuplugin_obssync/plugin.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 omuplugin_obssync-0.2.5/.gitignore
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 omuplugin_obssync-0.2.5/README.md
--rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 omuplugin_obssync-0.2.5/pyproject.toml
--rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 omuplugin_obssync-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 omuplugin_obssync-0.3.0/src/omuplugin_obssync/__init__.py
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 omuplugin_obssync-0.3.0/src/omuplugin_obssync/__main__.py
+-rw-r--r--   0        0        0     2587 2020-02-02 00:00:00.000000 omuplugin_obssync-0.3.0/src/omuplugin_obssync/plugin.py
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 omuplugin_obssync-0.3.0/src/omuplugin_obssync/version.py
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 omuplugin_obssync-0.3.0/.gitignore
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 omuplugin_obssync-0.3.0/README.md
+-rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 omuplugin_obssync-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 omuplugin_obssync-0.3.0/PKG-INFO
```

### Comparing `omuplugin_obssync-0.2.5/src/omuplugin_obssync/plugin.py` & `omuplugin_obssync-0.3.0/src/omuplugin_obssync/plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 from __future__ import annotations
 
 import json
 import os
 import subprocess
 import sys
 from pathlib import Path
-from typing import Any, List, TypedDict
+from typing import Any, TypedDict
 
 import psutil
 from omu.identifier import Identifier
 from omuserver.server import Server
 
 IDENTIFIER = Identifier("cc.omuchat", "plugin-obssync")
 
 
 class obs:
-    launch_command: List[str] | None = None
+    launch_command: list[str] | None = None
     cwd: Path | None = None
 
 
 def kill_obs():
     for proc in psutil.process_iter():
         if proc.name() == "obs":
             obs.launch_command = proc.cmdline()
@@ -33,15 +33,15 @@
 
 
 class ScriptToolJson(TypedDict):
     path: str
     settings: Any
 
 
-ModulesJson = TypedDict("ModulesJson", {"scripts-tool": List[ScriptToolJson]})
+ModulesJson = TypedDict("ModulesJson", {"scripts-tool": list[ScriptToolJson]})
 
 
 def get_launch_command():
     import os
     import sys
 
     return {
```

