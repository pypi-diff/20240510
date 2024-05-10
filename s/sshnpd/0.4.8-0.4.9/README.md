# Comparing `tmp/sshnpd-0.4.8.tar.gz` & `tmp/sshnpd-0.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sshnpd-0.4.8.tar", max compression
+gzip compressed data, was "sshnpd-0.4.9.tar", max compression
```

## Comparing `sshnpd-0.4.8.tar` & `sshnpd-0.4.9.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1529 2024-05-09 08:45:09.433183 sshnpd-0.4.8/LICENSE
--rw-r--r--   0        0        0     1416 2024-05-09 08:45:09.433183 sshnpd-0.4.8/README.PyPI.md
--rw-r--r--   0        0        0      484 2024-05-09 08:45:09.433183 sshnpd-0.4.8/pyproject.toml
--rwxr-xr-x   0        0        0    13417 2024-05-09 08:45:09.433183 sshnpd-0.4.8/sshnpd.py
--rw-r--r--   0        0        0     1994 1970-01-01 00:00:00.000000 sshnpd-0.4.8/PKG-INFO
+-rw-r--r--   0        0        0     1529 2024-05-10 14:47:39.666435 sshnpd-0.4.9/LICENSE
+-rw-r--r--   0        0        0     3176 2024-05-10 14:47:52.206473 sshnpd-0.4.9/README.PyPI.md
+-rw-r--r--   0        0        0      484 2024-05-10 14:47:39.666435 sshnpd-0.4.9/pyproject.toml
+-rwxr-xr-x   0        0        0    13417 2024-05-10 14:47:39.666435 sshnpd-0.4.9/sshnpd.py
+-rw-r--r--   0        0        0     3754 1970-01-01 00:00:00.000000 sshnpd-0.4.9/PKG-INFO
```

### Comparing `sshnpd-0.4.8/LICENSE` & `sshnpd-0.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `sshnpd-0.4.8/sshnpd.py` & `sshnpd-0.4.9/sshnpd.py`

 * *Files identical despite different names*

### Comparing `sshnpd-0.4.8/PKG-INFO` & `sshnpd-0.4.9/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 Metadata-Version: 2.1
 Name: sshnpd
-Version: 0.4.8
+Version: 0.4.9
 Summary: Python implementation of SSH No Ports daemon
 Home-page: https://github.com/atsign-foundation/noports
 Author: Xavier Lin
 Author-email: xavier.lin@atsign.com 
 Maintainer: Chris Swan
 Maintainer-email: chris@atsign.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: atsdk (==0.2.13)
+Requires-Dist: atsdk (==0.2.14)
 Description-Content-Type: text/markdown
 
 <h1><img width=250px src="https://atsign.com/wp-content/uploads/2022/05/atsign-logo-horizontal-color2022.svg" alt="The Atsign Foundation"></h1>
 
 [![GitHub License](https://img.shields.io/badge/license-BSD3-blue.svg)](./LICENSE)
+[![PyPI version](https://badge.fury.io/py/sshnpd.svg)](https://badge.fury.io/py/sshnpd)
+[![SLSA 3](https://slsa.dev/images/gh-badge-level3.svg)](https://slsa.dev)
 
-# SSHNPD Python
+# SSHNPD Python (beta)
 
 SSH No Ports provides a way to ssh to a remote linux host/device without that
 device or the client having any open ports (not even 22) on external
 interfaces. All network connectivity is outbound and there is no need to
 know the IP address the device has been given. As long as the device and
 client has an IP address (public or private 1918), DNS and Internet access,
 you will be able to connect to it.
@@ -31,38 +33,104 @@
 This version is SSHNP Daemon written in Python, it is still in its beta
 stage of developement.
 
 ## Prerequisites
 
 SSHNPD Python requires the following:
 
-* 2 atsigns, one for the client and one for the device
-* any machine with sshd running and python3 installed
-* atsdk installed
+* Python 3.10 or later on a system where the following packages containing
+native code are available[1]:
+  * bcrypt
+  * cffi
+  * charset-normalizer
+  * cryptography
+* Two atSigns, one for the client and one for the device
+  * The device atSign keys file should be placed in ~/.atsign/keys
+* An sshd bound to (at least) localhost
+  * Port 22 is the assumed default, but can be overridden
+
+[1] A common problem with installation is that native packages for a given
+architecture or libc aren't available. Pip will then download the source
+and try to compile that, which usually fails because the required toolchain
+isn't present.
 
 ## Installation
 
 This package can be installed from PyPI with:
 
 ```sh
 pip install sshnpd
 ```
 
+Though some systems will need `pip3` rather than `pip`:
+
+```sh
+pip3 install sshnpd
+```
+
+### Python virtual environments (venv)
+
+Recent Linux distributions such as Debian 12 and derivatives (including
+Ubuntu 24.04 and Rapberry Pi OS 'Bookworm') no longer allow the installation
+of packages from PyPI into the system Python. It's therefore necessary to
+use a virtual environment (venv).
+
+First ensure that pip and the venv module are available:
+
+```sh
+sudo apt install -y python3-pip python3-venv
+```
+
+Then create and activate a venv:
+
+```sh
+python3 -m venv sshnpd
+. sshnpd/bin/activate
+```
+
+The daemon can then be installed as before:
+
+```sh
+pip install sshnpd
+```
+
+Just remember to activate the venv first whenever using the daemon.
+
+### Installing from source
+
 Alternatively clone this repo and from the repo root:
 
 ```sh
 cd packages/python/sshnpd
 pip install -r requirements.txt
 pip install .
 ```
 
-## Running the program
+## Running the daemon
+
+```sh
+sshnpd -m @{clientAtsign} -a @{deviceAtsign} -d {deviceName} -u
+```
+
+e.g.
+
+```sh
+sshnpd -m @zaphod -a @heartofgold -d eddie -u
+```
+
+### Connecting to the daemon
+
+The Python version of SSHNPD presently implements v4 functionality, so it's
+a little behind the Dart implementation, and the latest client needs some
+flags to ensure compatibility:
 
 ```sh
-sshnpd -m @{clientAtsign} -a @{deviceAtsign} -d {deviceName}
+sshnp -f @{clientAtsign} -t @{deviceAtsign} -d {deviceName} \
+-r @{rvPoint} -u {user} --no-ad --no-et
 ```
 
-## No Ports SDK Python (experimental)
+e.g.
 
-There is a simple python SDK which allows you to create scripts for common
-administrative patterns via SSH No Ports.
+```sh
+sshnp -f @zaphod -t @heartofgold -d eddie -r @rv_am -u ubuntu --no-ad --no-et
+```
```

