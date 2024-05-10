# Comparing `tmp/plush-fabric-0.5.9.tar.gz` & `tmp/plush_fabric-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plush-fabric-0.5.9.tar", last modified: Wed Apr  5 22:12:30 2023, max compression
+gzip compressed data, was "plush_fabric-1.0.0.tar", last modified: Fri May 10 21:31:34 2024, max compression
```

## Comparing `plush-fabric-0.5.9.tar` & `plush_fabric-1.0.0.tar`

### file list

```diff
@@ -1,24 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-04-05 22:12:30.814624 plush-fabric-0.5.9/
--rw-rw-rw-   0        0        0     1088 2019-11-22 18:46:33.000000 plush-fabric-0.5.9/LICENSE.TXT
--rw-rw-rw-   0        0        0       40 2022-06-02 02:26:43.000000 plush-fabric-0.5.9/MANIFEST.in
--rw-rw-rw-   0        0        0     2438 2023-04-05 22:12:30.814624 plush-fabric-0.5.9/PKG-INFO
--rw-rw-rw-   0        0        0     1539 2022-06-02 02:26:43.000000 plush-fabric-0.5.9/README.md
-drwxrwxrwx   0        0        0        0 2023-04-05 22:12:30.778824 plush-fabric-0.5.9/plush/
--rw-rw-rw-   0        0        0        0 2017-05-24 00:51:53.000000 plush-fabric-0.5.9/plush/__init__.py
--rw-rw-rw-   0        0        0     1514 2022-06-01 22:10:39.000000 plush-fabric-0.5.9/plush/console.py
-drwxrwxrwx   0        0        0        0 2023-04-05 22:12:30.784377 plush-fabric-0.5.9/plush/fabric_commands/
--rw-rw-rw-   0        0        0     3148 2022-06-01 22:10:39.000000 plush-fabric-0.5.9/plush/fabric_commands/__init__.py
--rw-rw-rw-   0        0        0      615 2022-06-01 22:10:39.000000 plush-fabric-0.5.9/plush/fabric_commands/git.py
--rw-rw-rw-   0        0        0     1825 2023-01-03 04:13:04.000000 plush-fabric-0.5.9/plush/fabric_commands/permissions.py
--rw-rw-rw-   0        0        0      938 2022-06-01 22:10:39.000000 plush-fabric-0.5.9/plush/fabric_commands/ssh_key.py
--rw-rw-rw-   0        0        0     1989 2022-06-01 22:10:39.000000 plush-fabric-0.5.9/plush/oauth_flow.py
--rw-rw-rw-   0        0        0     1311 2022-06-01 22:10:39.000000 plush-fabric-0.5.9/plush/repo_keys.py
-drwxrwxrwx   0        0        0        0 2023-04-05 22:12:30.813624 plush-fabric-0.5.9/plush_fabric.egg-info/
--rw-rw-rw-   0        0        0     2438 2023-04-05 22:12:30.000000 plush-fabric-0.5.9/plush_fabric.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      477 2023-04-05 22:12:30.000000 plush-fabric-0.5.9/plush_fabric.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-05 22:12:30.000000 plush-fabric-0.5.9/plush_fabric.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       91 2023-04-05 22:12:30.000000 plush-fabric-0.5.9/plush_fabric.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      139 2023-04-05 22:12:30.000000 plush-fabric-0.5.9/plush_fabric.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-04-05 22:12:30.000000 plush-fabric-0.5.9/plush_fabric.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1209 2023-04-05 22:12:30.816629 plush-fabric-0.5.9/setup.cfg
--rw-rw-rw-   0        0        0       41 2022-06-02 02:26:43.000000 plush-fabric-0.5.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 21:31:34.976415 plush_fabric-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-05-10 21:31:25.000000 plush_fabric-1.0.0/LICENSE.TXT
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-10 21:31:25.000000 plush_fabric-1.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2666 2024-05-10 21:31:34.976415 plush_fabric-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1539 2024-05-10 21:31:25.000000 plush_fabric-1.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 21:31:34.972416 plush_fabric-1.0.0/plush/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 21:31:25.000000 plush_fabric-1.0.0/plush/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-05-10 21:31:25.000000 plush_fabric-1.0.0/plush/console.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 21:31:34.972416 plush_fabric-1.0.0/plush/fabric_commands/
+-rw-r--r--   0 runner    (1001) docker     (127)     3148 2024-05-10 21:31:25.000000 plush_fabric-1.0.0/plush/fabric_commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      615 2024-05-10 21:31:25.000000 plush_fabric-1.0.0/plush/fabric_commands/git.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1831 2024-05-10 21:31:25.000000 plush_fabric-1.0.0/plush/fabric_commands/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      938 2024-05-10 21:31:25.000000 plush_fabric-1.0.0/plush/fabric_commands/ssh_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1989 2024-05-10 21:31:25.000000 plush_fabric-1.0.0/plush/oauth_flow.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 21:31:34.976415 plush_fabric-1.0.0/plush/patchwork/
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-05-10 21:31:25.000000 plush_fabric-1.0.0/plush/patchwork/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5009 2024-05-10 21:31:25.000000 plush_fabric-1.0.0/plush/patchwork/files.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6581 2024-05-10 21:31:25.000000 plush_fabric-1.0.0/plush/patchwork/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1311 2024-05-10 21:31:25.000000 plush_fabric-1.0.0/plush/repo_keys.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 21:31:34.976415 plush_fabric-1.0.0/plush_fabric.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2666 2024-05-10 21:31:34.000000 plush_fabric-1.0.0/plush_fabric.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-05-10 21:31:34.000000 plush_fabric-1.0.0/plush_fabric.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 21:31:34.000000 plush_fabric-1.0.0/plush_fabric.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-10 21:31:34.000000 plush_fabric-1.0.0/plush_fabric.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-10 21:31:34.000000 plush_fabric-1.0.0/plush_fabric.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-10 21:31:34.000000 plush_fabric-1.0.0/plush_fabric.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-05-10 21:31:34.976415 plush_fabric-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-10 21:31:25.000000 plush_fabric-1.0.0/setup.py
```

### Comparing `plush-fabric-0.5.9/LICENSE.TXT` & `plush_fabric-1.0.0/LICENSE.TXT`

 * *Files identical despite different names*

### Comparing `plush-fabric-0.5.9/PKG-INFO` & `plush_fabric-1.0.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,50 +1,58 @@
-Metadata-Version: 2.1
-Name: plush-fabric
-Version: 0.5.9
-Summary: Helper library for Fabric to simplify creating and managing GitHub deploy keys when deploying GitHub-hosted repositories
-Home-page: https://github.com/kbarnes3/Plush
-Author: Kevin Barnes
-Author-email: kbarnes3@gmail.com
-Project-URL: Bug Tracker, https://github.com/kbarnes3/Plush/issues
-Keywords: Fabric,GitHub,deployment
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-Provides-Extra: test
-Provides-Extra: publish
-License-File: LICENSE.TXT
-
-Plush
-=====
-
-A helper library for [Fabric](https://www.fabfile.org) to simplify creating and managing GitHub deploy keys when deploying your GitHub-hosted
-repository. Currently, Plush is only tested on Ubuntu 22.04 LTS.
-
-Plush aims to make deployments easier by:
-- Using OAuth flows to securely connect to the GitHub API on your behalf
-(while supporting 2 factor auth and never handling your username/password)
-- Generating SSH deploy keys on your target server/computer
-- Registering these deploy keys with your GitHub repo programmatically
-- Configuring your new clone to use the appropriate deploy key while not conflicting with other 
-SSH keys used elsewhere on your server
-- ACL'ing these keys so they can be reused by people to fetch/deploy on your behalf
-(and not readable by anyone else on the server)
-- Example PowerShell scripts are provided that give tab completion around fab.exe
-
-To see this project in action, follow the directions in Setup-Dev-Environment.md. You will need access to an Ubuntu 18.04 machine (ideally a VM).
-
-Usage
-
-This project is intended to be used by projects that use or are considering [Fabric](https://www.fabfile.org) for their deployments. Plush expects Fabric 2.0 or greater.
-In a project that uses Fabric, install Plush by running:
-
-`pip install plush-fabric`
-
-To get started, see the `fabfile.py` in the [GitHub repo](https://github.com/kbarnes3/Plush) for a minimal usage of Plush.
-For a more complete example, see my [BaseDjangoAngular template](https://github.com/kbarnes3/BaseDjangoAngular).
+Metadata-Version: 2.1
+Name: plush-fabric
+Version: 1.0.0
+Summary: Helper library for Fabric to simplify creating and managing GitHub deploy keys when deploying GitHub-hosted repositories
+Home-page: https://github.com/kbarnes3/Plush
+Author: Kevin Barnes
+Author-email: kbarnes3@gmail.com
+Project-URL: Bug Tracker, https://github.com/kbarnes3/Plush/issues
+Keywords: Fabric,GitHub,deployment
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.12
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers
+Classifier: Topic :: Software Development
+Requires-Python: >=3.12
+Description-Content-Type: text/markdown
+License-File: LICENSE.TXT
+Requires-Dist: oauth2client>=4.1.3
+Requires-Dist: PyGithub>=2.3.0
+Requires-Dist: keyring>=25.2.0
+Requires-Dist: fabric>=3.2.2
+Requires-Dist: colorama>=0.4.6
+Provides-Extra: test
+Requires-Dist: pylint; extra == "test"
+Provides-Extra: publish
+Requires-Dist: build; extra == "publish"
+Requires-Dist: twine; extra == "publish"
+
+Plush
+==============
+
+A helper library for [Fabric](https://www.fabfile.org) to simplify creating and managing GitHub deploy keys when deploying your GitHub-hosted
+repository. Currently, Plush is only tested on Ubuntu 24.04 LTS.
+
+Plush aims to make deployments easier by:
+- Using OAuth flows to securely connect to the GitHub API on your behalf
+(while supporting 2 factor auth and never handling your username/password)
+- Generating SSH deploy keys on your target server/computer
+- Registering these deploy keys with your GitHub repo programmatically
+- Configuring your new clone to use the appropriate deploy key while not conflicting with other 
+SSH keys used elsewhere on your server
+- ACL'ing these keys so they can be reused by people to fetch/deploy on your behalf
+(and not readable by anyone else on the server)
+- Example PowerShell scripts are provided that give tab completion around fab.exe
+
+To see this project in action, follow the directions in Setup-Dev-Environment.md. You will need access to an Ubuntu 24.04 machine (ideally a VM).
+
+## Usage
+
+This project is intended to be used by projects that use or are considering [Fabric](https://www.fabfile.org) for their deployments. Plush versions 1.0 and greater expect Fabric 3.2.2 and greater. In a project that uses Fabric, install Plush by running:
+
+```
+pip install plush-fabric
+```
+
+To get started, see the fabfile.py in this repo for a minimal usage of Plush. For a more complete example, see my [BaseDjangoAngular template](https://github.com/kbarnes3/BaseDjangoAngular).
```

### Comparing `plush-fabric-0.5.9/README.md` & `plush_fabric-1.0.0/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 Plush
-=====
+==============
 
 A helper library for [Fabric](https://www.fabfile.org) to simplify creating and managing GitHub deploy keys when deploying your GitHub-hosted
-repository. Currently, Plush is only tested on Ubuntu 22.04 LTS.
+repository. Currently, Plush is only tested on Ubuntu 24.04 LTS.
 
 Plush aims to make deployments easier by:
 - Using OAuth flows to securely connect to the GitHub API on your behalf
 (while supporting 2 factor auth and never handling your username/password)
 - Generating SSH deploy keys on your target server/computer
 - Registering these deploy keys with your GitHub repo programmatically
 - Configuring your new clone to use the appropriate deploy key while not conflicting with other 
 SSH keys used elsewhere on your server
 - ACL'ing these keys so they can be reused by people to fetch/deploy on your behalf
 (and not readable by anyone else on the server)
 - Example PowerShell scripts are provided that give tab completion around fab.exe
 
-To see this project in action, follow the directions in Setup-Dev-Environment.md. You will need access to an Ubuntu 18.04 machine (ideally a VM).
+To see this project in action, follow the directions in Setup-Dev-Environment.md. You will need access to an Ubuntu 24.04 machine (ideally a VM).
 
-Usage
+## Usage
 
-This project is intended to be used by projects that use or are considering [Fabric](https://www.fabfile.org) for their deployments. Plush expects Fabric 2.0 or greater.
-In a project that uses Fabric, install Plush by running:
+This project is intended to be used by projects that use or are considering [Fabric](https://www.fabfile.org) for their deployments. Plush versions 1.0 and greater expect Fabric 3.2.2 and greater. In a project that uses Fabric, install Plush by running:
 
-`pip install plush-fabric`
+```
+pip install plush-fabric
+```
 
-To get started, see the `fabfile.py` in the [GitHub repo](https://github.com/kbarnes3/Plush) for a minimal usage of Plush.
-For a more complete example, see my [BaseDjangoAngular template](https://github.com/kbarnes3/BaseDjangoAngular).
+To get started, see the fabfile.py in this repo for a minimal usage of Plush. For a more complete example, see my [BaseDjangoAngular template](https://github.com/kbarnes3/BaseDjangoAngular).
```

### Comparing `plush-fabric-0.5.9/plush/console.py` & `plush_fabric-1.0.0/plush/console.py`

 * *Files identical despite different names*

### Comparing `plush-fabric-0.5.9/plush/fabric_commands/__init__.py` & `plush_fabric-1.0.0/plush/fabric_commands/__init__.py`

 * *Files identical despite different names*

### Comparing `plush-fabric-0.5.9/plush/fabric_commands/git.py` & `plush_fabric-1.0.0/plush/fabric_commands/git.py`

 * *Files identical despite different names*

### Comparing `plush-fabric-0.5.9/plush/fabric_commands/permissions.py` & `plush_fabric-1.0.0/plush/fabric_commands/permissions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Optional
 from fabric.connection import Connection
-from patchwork.files import exists as patchwork_exists
+from plush.patchwork.files import exists as patchwork_exists
 
 
 def _exists(conn: Connection, path: str, sudo: bool=False) -> bool:
     # pylint doesn't understand the @set_runner decorator
     # create a wrapper so we only have to suppress the error once
     return patchwork_exists(conn, path, sudo=sudo) # pylint: disable=E1120
```

### Comparing `plush-fabric-0.5.9/plush/fabric_commands/ssh_key.py` & `plush_fabric-1.0.0/plush/fabric_commands/ssh_key.py`

 * *Files identical despite different names*

### Comparing `plush-fabric-0.5.9/plush/oauth_flow.py` & `plush_fabric-1.0.0/plush/oauth_flow.py`

 * *Files identical despite different names*

### Comparing `plush-fabric-0.5.9/plush/repo_keys.py` & `plush_fabric-1.0.0/plush/repo_keys.py`

 * *Files identical despite different names*

### Comparing `plush-fabric-0.5.9/plush_fabric.egg-info/PKG-INFO` & `plush_fabric-1.0.0/plush_fabric.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,50 +1,58 @@
-Metadata-Version: 2.1
-Name: plush-fabric
-Version: 0.5.9
-Summary: Helper library for Fabric to simplify creating and managing GitHub deploy keys when deploying GitHub-hosted repositories
-Home-page: https://github.com/kbarnes3/Plush
-Author: Kevin Barnes
-Author-email: kbarnes3@gmail.com
-Project-URL: Bug Tracker, https://github.com/kbarnes3/Plush/issues
-Keywords: Fabric,GitHub,deployment
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-Provides-Extra: test
-Provides-Extra: publish
-License-File: LICENSE.TXT
-
-Plush
-=====
-
-A helper library for [Fabric](https://www.fabfile.org) to simplify creating and managing GitHub deploy keys when deploying your GitHub-hosted
-repository. Currently, Plush is only tested on Ubuntu 22.04 LTS.
-
-Plush aims to make deployments easier by:
-- Using OAuth flows to securely connect to the GitHub API on your behalf
-(while supporting 2 factor auth and never handling your username/password)
-- Generating SSH deploy keys on your target server/computer
-- Registering these deploy keys with your GitHub repo programmatically
-- Configuring your new clone to use the appropriate deploy key while not conflicting with other 
-SSH keys used elsewhere on your server
-- ACL'ing these keys so they can be reused by people to fetch/deploy on your behalf
-(and not readable by anyone else on the server)
-- Example PowerShell scripts are provided that give tab completion around fab.exe
-
-To see this project in action, follow the directions in Setup-Dev-Environment.md. You will need access to an Ubuntu 18.04 machine (ideally a VM).
-
-Usage
-
-This project is intended to be used by projects that use or are considering [Fabric](https://www.fabfile.org) for their deployments. Plush expects Fabric 2.0 or greater.
-In a project that uses Fabric, install Plush by running:
-
-`pip install plush-fabric`
-
-To get started, see the `fabfile.py` in the [GitHub repo](https://github.com/kbarnes3/Plush) for a minimal usage of Plush.
-For a more complete example, see my [BaseDjangoAngular template](https://github.com/kbarnes3/BaseDjangoAngular).
+Metadata-Version: 2.1
+Name: plush-fabric
+Version: 1.0.0
+Summary: Helper library for Fabric to simplify creating and managing GitHub deploy keys when deploying GitHub-hosted repositories
+Home-page: https://github.com/kbarnes3/Plush
+Author: Kevin Barnes
+Author-email: kbarnes3@gmail.com
+Project-URL: Bug Tracker, https://github.com/kbarnes3/Plush/issues
+Keywords: Fabric,GitHub,deployment
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.12
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers
+Classifier: Topic :: Software Development
+Requires-Python: >=3.12
+Description-Content-Type: text/markdown
+License-File: LICENSE.TXT
+Requires-Dist: oauth2client>=4.1.3
+Requires-Dist: PyGithub>=2.3.0
+Requires-Dist: keyring>=25.2.0
+Requires-Dist: fabric>=3.2.2
+Requires-Dist: colorama>=0.4.6
+Provides-Extra: test
+Requires-Dist: pylint; extra == "test"
+Provides-Extra: publish
+Requires-Dist: build; extra == "publish"
+Requires-Dist: twine; extra == "publish"
+
+Plush
+==============
+
+A helper library for [Fabric](https://www.fabfile.org) to simplify creating and managing GitHub deploy keys when deploying your GitHub-hosted
+repository. Currently, Plush is only tested on Ubuntu 24.04 LTS.
+
+Plush aims to make deployments easier by:
+- Using OAuth flows to securely connect to the GitHub API on your behalf
+(while supporting 2 factor auth and never handling your username/password)
+- Generating SSH deploy keys on your target server/computer
+- Registering these deploy keys with your GitHub repo programmatically
+- Configuring your new clone to use the appropriate deploy key while not conflicting with other 
+SSH keys used elsewhere on your server
+- ACL'ing these keys so they can be reused by people to fetch/deploy on your behalf
+(and not readable by anyone else on the server)
+- Example PowerShell scripts are provided that give tab completion around fab.exe
+
+To see this project in action, follow the directions in Setup-Dev-Environment.md. You will need access to an Ubuntu 24.04 machine (ideally a VM).
+
+## Usage
+
+This project is intended to be used by projects that use or are considering [Fabric](https://www.fabfile.org) for their deployments. Plush versions 1.0 and greater expect Fabric 3.2.2 and greater. In a project that uses Fabric, install Plush by running:
+
+```
+pip install plush-fabric
+```
+
+To get started, see the fabfile.py in this repo for a minimal usage of Plush. For a more complete example, see my [BaseDjangoAngular template](https://github.com/kbarnes3/BaseDjangoAngular).
```

### Comparing `plush-fabric-0.5.9/setup.cfg` & `plush_fabric-1.0.0/setup.cfg`

 * *Files 20% similar despite different names*

```diff
@@ -1,76 +1,73 @@
-00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
-00000010: 203d 2070 6c75 7368 2d66 6162 7269 630d   = plush-fabric.
-00000020: 0a76 6572 7369 6f6e 203d 2030 2e35 2e39  .version = 0.5.9
-00000030: 0d0a 6175 7468 6f72 203d 204b 6576 696e  ..author = Kevin
-00000040: 2042 6172 6e65 730d 0a61 7574 686f 725f   Barnes..author_
-00000050: 656d 6169 6c20 3d20 6b62 6172 6e65 7333  email = kbarnes3
-00000060: 4067 6d61 696c 2e63 6f6d 0d0a 6465 7363  @gmail.com..desc
-00000070: 7269 7074 696f 6e20 3d20 4865 6c70 6572  ription = Helper
-00000080: 206c 6962 7261 7279 2066 6f72 2046 6162   library for Fab
-00000090: 7269 6320 746f 2073 696d 706c 6966 7920  ric to simplify 
-000000a0: 6372 6561 7469 6e67 2061 6e64 206d 616e  creating and man
-000000b0: 6167 696e 6720 4769 7448 7562 2064 6570  aging GitHub dep
-000000c0: 6c6f 7920 6b65 7973 2077 6865 6e20 6465  loy keys when de
-000000d0: 706c 6f79 696e 6720 4769 7448 7562 2d68  ploying GitHub-h
-000000e0: 6f73 7465 6420 7265 706f 7369 746f 7269  osted repositori
-000000f0: 6573 0d0a 6c6f 6e67 5f64 6573 6372 6970  es..long_descrip
-00000100: 7469 6f6e 203d 2066 696c 653a 2052 4541  tion = file: REA
-00000110: 444d 452e 6d64 0d0a 6c6f 6e67 5f64 6573  DME.md..long_des
-00000120: 6372 6970 7469 6f6e 5f63 6f6e 7465 6e74  cription_content
-00000130: 5f74 7970 6520 3d20 7465 7874 2f6d 6172  _type = text/mar
-00000140: 6b64 6f77 6e0d 0a75 726c 203d 2068 7474  kdown..url = htt
-00000150: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00000160: 6b62 6172 6e65 7333 2f50 6c75 7368 0d0a  kbarnes3/Plush..
-00000170: 7072 6f6a 6563 745f 7572 6c73 203d 200d  project_urls = .
-00000180: 0a09 4275 6720 5472 6163 6b65 7220 3d20  ..Bug Tracker = 
-00000190: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-000001a0: 6f6d 2f6b 6261 726e 6573 332f 506c 7573  om/kbarnes3/Plus
-000001b0: 682f 6973 7375 6573 0d0a 636c 6173 7369  h/issues..classi
-000001c0: 6669 6572 7320 3d20 0d0a 0950 726f 6772  fiers = ...Progr
-000001d0: 616d 6d69 6e67 204c 616e 6775 6167 6520  amming Language 
-000001e0: 3a3a 2050 7974 686f 6e20 3a3a 2033 0d0a  :: Python :: 3..
-000001f0: 0950 726f 6772 616d 6d69 6e67 204c 616e  .Programming Lan
-00000200: 6775 6167 6520 3a3a 2050 7974 686f 6e20  guage :: Python 
-00000210: 3a3a 2033 2e31 300d 0a09 4c69 6365 6e73  :: 3.10...Licens
-00000220: 6520 3a3a 204f 5349 2041 7070 726f 7665  e :: OSI Approve
-00000230: 6420 3a3a 204d 4954 204c 6963 656e 7365  d :: MIT License
-00000240: 0d0a 094f 7065 7261 7469 6e67 2053 7973  ...Operating Sys
-00000250: 7465 6d20 3a3a 204f 5320 496e 6465 7065  tem :: OS Indepe
-00000260: 6e64 656e 740d 0a09 4465 7665 6c6f 706d  ndent...Developm
-00000270: 656e 7420 5374 6174 7573 203a 3a20 3420  ent Status :: 4 
-00000280: 2d20 4265 7461 0d0a 0949 6e74 656e 6465  - Beta...Intende
-00000290: 6420 4175 6469 656e 6365 203a 3a20 4465  d Audience :: De
-000002a0: 7665 6c6f 7065 7273 0d0a 0954 6f70 6963  velopers...Topic
-000002b0: 203a 3a20 536f 6674 7761 7265 2044 6576   :: Software Dev
-000002c0: 656c 6f70 6d65 6e74 0d0a 6b65 7977 6f72  elopment..keywor
-000002d0: 6473 203d 2046 6162 7269 632c 2047 6974  ds = Fabric, Git
-000002e0: 4875 622c 2064 6570 6c6f 796d 656e 740d  Hub, deployment.
-000002f0: 0a0d 0a5b 6f70 7469 6f6e 735d 0d0a 7061  ...[options]..pa
-00000300: 636b 6167 6573 203d 200d 0a09 706c 7573  ckages = ...plus
-00000310: 680d 0a09 706c 7573 682e 6661 6272 6963  h...plush.fabric
-00000320: 5f63 6f6d 6d61 6e64 730d 0a70 7974 686f  _commands..pytho
-00000330: 6e5f 7265 7175 6972 6573 203d 203e 3d33  n_requires = >=3
-00000340: 2e31 300d 0a69 6e73 7461 6c6c 5f72 6571  .10..install_req
-00000350: 7569 7265 7320 3d20 0d0a 096f 6175 7468  uires = ...oauth
-00000360: 3263 6c69 656e 743e 3d34 2e31 2e33 0d0a  2client>=4.1.3..
-00000370: 0950 7947 6974 6875 623e 3d31 2e35 382e  .PyGithub>=1.58.
-00000380: 310d 0a09 6b65 7972 696e 673e 3d32 332e  1...keyring>=23.
-00000390: 3133 2e31 0d0a 0966 6162 7269 633e 3d32  13.1...fabric>=2
-000003a0: 2e37 2e31 0d0a 0970 6174 6368 776f 726b  .7.1...patchwork
-000003b0: 3e3d 312e 302e 310d 0a09 636f 6c6f 7261  >=1.0.1...colora
-000003c0: 6d61 3e3d 302e 342e 360d 0a0d 0a5b 6f70  ma>=0.4.6....[op
-000003d0: 7469 6f6e 732e 656e 7472 795f 706f 696e  tions.entry_poin
-000003e0: 7473 5d0d 0a63 6f6e 736f 6c65 5f73 6372  ts]..console_scr
-000003f0: 6970 7473 203d 200d 0a09 6175 7468 203d  ipts = ...auth =
-00000400: 2070 6c75 7368 2e63 6f6e 736f 6c65 3a61   plush.console:a
-00000410: 7574 685f 656e 7472 790d 0a09 6c69 7374  uth_entry...list
-00000420: 6b65 7973 203d 2070 6c75 7368 2e63 6f6e  keys = plush.con
-00000430: 736f 6c65 3a6c 6973 745f 6b65 7973 5f65  sole:list_keys_e
-00000440: 6e74 7279 0d0a 0d0a 5b6f 7074 696f 6e73  ntry....[options
-00000450: 2e65 7874 7261 735f 7265 7175 6972 655d  .extras_require]
-00000460: 0d0a 7465 7374 203d 2070 796c 696e 740d  ..test = pylint.
-00000470: 0a70 7562 6c69 7368 203d 200d 0a09 6275  .publish = ...bu
-00000480: 696c 640d 0a09 7477 696e 650d 0a0d 0a5b  ild...twine....[
-00000490: 6567 675f 696e 666f 5d0d 0a74 6167 5f62  egg_info]..tag_b
-000004a0: 7569 6c64 203d 200d 0a74 6167 5f64 6174  uild = ..tag_dat
-000004b0: 6520 3d20 300d 0a0d 0a                   e = 0....
+00000000: 5b6d 6574 6164 6174 615d 0a6e 616d 6520  [metadata].name 
+00000010: 3d20 706c 7573 682d 6661 6272 6963 0a76  = plush-fabric.v
+00000020: 6572 7369 6f6e 203d 2031 2e30 2e30 0a61  ersion = 1.0.0.a
+00000030: 7574 686f 7220 3d20 4b65 7669 6e20 4261  uthor = Kevin Ba
+00000040: 726e 6573 0a61 7574 686f 725f 656d 6169  rnes.author_emai
+00000050: 6c20 3d20 6b62 6172 6e65 7333 4067 6d61  l = kbarnes3@gma
+00000060: 696c 2e63 6f6d 0a64 6573 6372 6970 7469  il.com.descripti
+00000070: 6f6e 203d 2048 656c 7065 7220 6c69 6272  on = Helper libr
+00000080: 6172 7920 666f 7220 4661 6272 6963 2074  ary for Fabric t
+00000090: 6f20 7369 6d70 6c69 6679 2063 7265 6174  o simplify creat
+000000a0: 696e 6720 616e 6420 6d61 6e61 6769 6e67  ing and managing
+000000b0: 2047 6974 4875 6220 6465 706c 6f79 206b   GitHub deploy k
+000000c0: 6579 7320 7768 656e 2064 6570 6c6f 7969  eys when deployi
+000000d0: 6e67 2047 6974 4875 622d 686f 7374 6564  ng GitHub-hosted
+000000e0: 2072 6570 6f73 6974 6f72 6965 730a 6c6f   repositories.lo
+000000f0: 6e67 5f64 6573 6372 6970 7469 6f6e 203d  ng_description =
+00000100: 2066 696c 653a 2052 4541 444d 452e 6d64   file: README.md
+00000110: 0a6c 6f6e 675f 6465 7363 7269 7074 696f  .long_descriptio
+00000120: 6e5f 636f 6e74 656e 745f 7479 7065 203d  n_content_type =
+00000130: 2074 6578 742f 6d61 726b 646f 776e 0a75   text/markdown.u
+00000140: 726c 203d 2068 7474 7073 3a2f 2f67 6974  rl = https://git
+00000150: 6875 622e 636f 6d2f 6b62 6172 6e65 7333  hub.com/kbarnes3
+00000160: 2f50 6c75 7368 0a70 726f 6a65 6374 5f75  /Plush.project_u
+00000170: 726c 7320 3d20 0a09 4275 6720 5472 6163  rls = ..Bug Trac
+00000180: 6b65 7220 3d20 6874 7470 733a 2f2f 6769  ker = https://gi
+00000190: 7468 7562 2e63 6f6d 2f6b 6261 726e 6573  thub.com/kbarnes
+000001a0: 332f 506c 7573 682f 6973 7375 6573 0a63  3/Plush/issues.c
+000001b0: 6c61 7373 6966 6965 7273 203d 200a 0950  lassifiers = ..P
+000001c0: 726f 6772 616d 6d69 6e67 204c 616e 6775  rogramming Langu
+000001d0: 6167 6520 3a3a 2050 7974 686f 6e20 3a3a  age :: Python ::
+000001e0: 2033 0a09 5072 6f67 7261 6d6d 696e 6720   3..Programming 
+000001f0: 4c61 6e67 7561 6765 203a 3a20 5079 7468  Language :: Pyth
+00000200: 6f6e 203a 3a20 332e 3132 0a09 4c69 6365  on :: 3.12..Lice
+00000210: 6e73 6520 3a3a 204f 5349 2041 7070 726f  nse :: OSI Appro
+00000220: 7665 6420 3a3a 204d 4954 204c 6963 656e  ved :: MIT Licen
+00000230: 7365 0a09 4f70 6572 6174 696e 6720 5379  se..Operating Sy
+00000240: 7374 656d 203a 3a20 4f53 2049 6e64 6570  stem :: OS Indep
+00000250: 656e 6465 6e74 0a09 4465 7665 6c6f 706d  endent..Developm
+00000260: 656e 7420 5374 6174 7573 203a 3a20 3420  ent Status :: 4 
+00000270: 2d20 4265 7461 0a09 496e 7465 6e64 6564  - Beta..Intended
+00000280: 2041 7564 6965 6e63 6520 3a3a 2044 6576   Audience :: Dev
+00000290: 656c 6f70 6572 730a 0954 6f70 6963 203a  elopers..Topic :
+000002a0: 3a20 536f 6674 7761 7265 2044 6576 656c  : Software Devel
+000002b0: 6f70 6d65 6e74 0a6b 6579 776f 7264 7320  opment.keywords 
+000002c0: 3d20 4661 6272 6963 2c20 4769 7448 7562  = Fabric, GitHub
+000002d0: 2c20 6465 706c 6f79 6d65 6e74 0a0a 5b6f  , deployment..[o
+000002e0: 7074 696f 6e73 5d0a 7061 636b 6167 6573  ptions].packages
+000002f0: 203d 200a 0970 6c75 7368 0a09 706c 7573   = ..plush..plus
+00000300: 682e 6661 6272 6963 5f63 6f6d 6d61 6e64  h.fabric_command
+00000310: 730a 0970 6c75 7368 2e70 6174 6368 776f  s..plush.patchwo
+00000320: 726b 0a70 7974 686f 6e5f 7265 7175 6972  rk.python_requir
+00000330: 6573 203d 203e 3d33 2e31 320a 696e 7374  es = >=3.12.inst
+00000340: 616c 6c5f 7265 7175 6972 6573 203d 200a  all_requires = .
+00000350: 096f 6175 7468 3263 6c69 656e 743e 3d34  .oauth2client>=4
+00000360: 2e31 2e33 0a09 5079 4769 7468 7562 3e3d  .1.3..PyGithub>=
+00000370: 322e 332e 300a 096b 6579 7269 6e67 3e3d  2.3.0..keyring>=
+00000380: 3235 2e32 2e30 0a09 6661 6272 6963 3e3d  25.2.0..fabric>=
+00000390: 332e 322e 320a 0963 6f6c 6f72 616d 613e  3.2.2..colorama>
+000003a0: 3d30 2e34 2e36 0a0a 5b6f 7074 696f 6e73  =0.4.6..[options
+000003b0: 2e65 6e74 7279 5f70 6f69 6e74 735d 0a63  .entry_points].c
+000003c0: 6f6e 736f 6c65 5f73 6372 6970 7473 203d  onsole_scripts =
+000003d0: 200a 0961 7574 6820 3d20 706c 7573 682e   ..auth = plush.
+000003e0: 636f 6e73 6f6c 653a 6175 7468 5f65 6e74  console:auth_ent
+000003f0: 7279 0a09 6c69 7374 6b65 7973 203d 2070  ry..listkeys = p
+00000400: 6c75 7368 2e63 6f6e 736f 6c65 3a6c 6973  lush.console:lis
+00000410: 745f 6b65 7973 5f65 6e74 7279 0a0a 5b6f  t_keys_entry..[o
+00000420: 7074 696f 6e73 2e65 7874 7261 735f 7265  ptions.extras_re
+00000430: 7175 6972 655d 0a74 6573 7420 3d20 7079  quire].test = py
+00000440: 6c69 6e74 0a70 7562 6c69 7368 203d 200a  lint.publish = .
+00000450: 0962 7569 6c64 0a09 7477 696e 650a 0a5b  .build..twine..[
+00000460: 6567 675f 696e 666f 5d0a 7461 675f 6275  egg_info].tag_bu
+00000470: 696c 6420 3d20 0a74 6167 5f64 6174 6520  ild = .tag_date 
+00000480: 3d20 300a 0a                             = 0..
```

