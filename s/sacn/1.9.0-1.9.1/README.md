# Comparing `tmp/sacn-1.9.0.tar.gz` & `tmp/sacn-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/sacn-1.9.0.tar", last modified: Sun Dec  4 11:31:57 2022, max compression
+gzip compressed data, was "sacn-1.9.1.tar", last modified: Fri May 10 07:36:24 2024, max compression
```

## Comparing `sacn-1.9.0.tar` & `sacn-1.9.1.tar`

### file list

```diff
@@ -1,47 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-04 11:31:57.000000 sacn-1.9.0/
--rw-r--r--   0 runner    (1001) docker     (122)      771 2022-12-04 11:31:41.000000 sacn-1.9.0/setup.py
--rw-r--r--   0 runner    (1001) docker     (122)    15894 2022-12-04 11:31:41.000000 sacn-1.9.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-04 11:31:57.000000 sacn-1.9.0/sacn.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-12-04 11:31:56.000000 sacn-1.9.0/sacn.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        5 2022-12-04 11:31:56.000000 sacn-1.9.0/sacn.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-12-04 11:31:56.000000 sacn-1.9.0/sacn.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)     1150 2022-12-04 11:31:57.000000 sacn-1.9.0/sacn.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)    18413 2022-12-04 11:31:56.000000 sacn-1.9.0/sacn.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    18413 2022-12-04 11:31:57.000000 sacn-1.9.0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-04 11:31:57.000000 sacn-1.9.0/sacn/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-04 11:31:57.000000 sacn-1.9.0/sacn/sending/
--rw-r--r--   0 runner    (1001) docker     (122)     4531 2022-12-04 11:31:41.000000 sacn-1.9.0/sacn/sending/sender_handler.py
--rw-r--r--   0 runner    (1001) docker     (122)     1302 2022-12-04 11:31:41.000000 sacn-1.9.0/sacn/sending/output.py
--rw-r--r--   0 runner    (1001) docker     (122)     1282 2022-12-04 11:31:41.000000 sacn-1.9.0/sacn/sending/sender_socket_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     3891 2022-12-04 11:31:41.000000 sacn-1.9.0/sacn/sending/sender_socket_udp.py
--rw-r--r--   0 runner    (1001) docker     (122)     1096 2022-12-04 11:31:41.000000 sacn-1.9.0/sacn/sending/sender_socket_base.py
--rw-r--r--   0 runner    (1001) docker     (122)     7363 2022-12-04 11:31:41.000000 sacn-1.9.0/sacn/sending/sender_handler_test.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-04 11:31:41.000000 sacn-1.9.0/sacn/sending/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1025 2022-12-04 11:31:41.000000 sacn-1.9.0/sacn/sending/sender_socket_base_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     7442 2022-12-04 11:31:41.000000 sacn-1.9.0/sacn/sender.py
--rw-r--r--   0 runner    (1001) docker     (122)     6746 2022-12-04 11:31:41.000000 sacn-1.9.0/sacn/receiver.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-04 11:31:57.000000 sacn-1.9.0/sacn/messages/
--rw-r--r--   0 runner    (1001) docker     (122)     8380 2022-12-04 11:31:41.000000 sacn-1.9.0/sacn/messages/universe_discovery_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     9987 2022-12-04 11:31:41.000000 sacn-1.9.0/sacn/messages/data_packet_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     3106 2022-12-04 11:31:41.000000 sacn-1.9.0/sacn/messages/sync_packet.py
--rw-r--r--   0 runner    (1001) docker     (122)     3652 2022-12-04 11:31:41.000000 sacn-1.9.0/sacn/messages/root_layer.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-04 11:31:41.000000 sacn-1.9.0/sacn/messages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3857 2022-12-04 11:31:41.000000 sacn-1.9.0/sacn/messages/root_layer_test.py
--rw-r--r--   0 runner    (1001) docker     (122)      871 2022-12-04 11:31:41.000000 sacn-1.9.0/sacn/messages/data_types.py
--rw-r--r--   0 runner    (1001) docker     (122)     4738 2022-12-04 11:31:41.000000 sacn-1.9.0/sacn/messages/sync_packet_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     7975 2022-12-04 11:31:41.000000 sacn-1.9.0/sacn/messages/universe_discovery.py
--rw-r--r--   0 runner    (1001) docker     (122)      536 2022-12-04 11:31:41.000000 sacn-1.9.0/sacn/messages/general_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     2016 2022-12-04 11:31:41.000000 sacn-1.9.0/sacn/messages/data_types_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     9603 2022-12-04 11:31:41.000000 sacn-1.9.0/sacn/messages/data_packet.py
--rw-r--r--   0 runner    (1001) docker     (122)      406 2022-12-04 11:31:41.000000 sacn-1.9.0/sacn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5924 2022-12-04 11:31:41.000000 sacn-1.9.0/sacn/receiver_test.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-04 11:31:57.000000 sacn-1.9.0/sacn/receiving/
--rw-r--r--   0 runner    (1001) docker     (122)     8353 2022-12-04 11:31:41.000000 sacn-1.9.0/sacn/receiving/receiver_handler_test.py
--rw-r--r--   0 runner    (1001) docker     (122)      846 2022-12-04 11:31:41.000000 sacn-1.9.0/sacn/receiving/receiver_socket_base_test.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-04 11:31:41.000000 sacn-1.9.0/sacn/receiving/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1018 2022-12-04 11:31:41.000000 sacn-1.9.0/sacn/receiving/receiver_socket_base.py
--rw-r--r--   0 runner    (1001) docker     (122)     4030 2022-12-04 11:31:41.000000 sacn-1.9.0/sacn/receiving/receiver_socket_udp.py
--rw-r--r--   0 runner    (1001) docker     (122)     7873 2022-12-04 11:31:41.000000 sacn-1.9.0/sacn/receiving/receiver_handler.py
--rw-r--r--   0 runner    (1001) docker     (122)     1071 2022-12-04 11:31:41.000000 sacn-1.9.0/sacn/receiving/receiver_socket_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     8805 2022-12-04 11:31:41.000000 sacn-1.9.0/sacn/sender_test.py
--rw-r--r--   0 runner    (1001) docker     (122)       38 2022-12-04 11:31:57.000000 sacn-1.9.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 07:36:24.043501 sacn-1.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-05-10 07:36:14.000000 sacn-1.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    16637 2024-05-10 07:36:24.043501 sacn-1.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    16119 2024-05-10 07:36:14.000000 sacn-1.9.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 07:36:24.035501 sacn-1.9.1/sacn/
+-rw-r--r--   0 runner    (1001) docker     (127)      406 2024-05-10 07:36:14.000000 sacn-1.9.1/sacn/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 07:36:24.039501 sacn-1.9.1/sacn/messages/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 07:36:14.000000 sacn-1.9.1/sacn/messages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9603 2024-05-10 07:36:14.000000 sacn-1.9.1/sacn/messages/data_packet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9987 2024-05-10 07:36:14.000000 sacn-1.9.1/sacn/messages/data_packet_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      871 2024-05-10 07:36:14.000000 sacn-1.9.1/sacn/messages/data_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2016 2024-05-10 07:36:14.000000 sacn-1.9.1/sacn/messages/data_types_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2024-05-10 07:36:14.000000 sacn-1.9.1/sacn/messages/general_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3652 2024-05-10 07:36:14.000000 sacn-1.9.1/sacn/messages/root_layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3857 2024-05-10 07:36:14.000000 sacn-1.9.1/sacn/messages/root_layer_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3106 2024-05-10 07:36:14.000000 sacn-1.9.1/sacn/messages/sync_packet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4738 2024-05-10 07:36:14.000000 sacn-1.9.1/sacn/messages/sync_packet_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7976 2024-05-10 07:36:14.000000 sacn-1.9.1/sacn/messages/universe_discovery.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8380 2024-05-10 07:36:14.000000 sacn-1.9.1/sacn/messages/universe_discovery_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6746 2024-05-10 07:36:14.000000 sacn-1.9.1/sacn/receiver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5924 2024-05-10 07:36:14.000000 sacn-1.9.1/sacn/receiver_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 07:36:24.043501 sacn-1.9.1/sacn/receiving/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 07:36:14.000000 sacn-1.9.1/sacn/receiving/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7873 2024-05-10 07:36:14.000000 sacn-1.9.1/sacn/receiving/receiver_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8353 2024-05-10 07:36:14.000000 sacn-1.9.1/sacn/receiving/receiver_handler_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1018 2024-05-10 07:36:14.000000 sacn-1.9.1/sacn/receiving/receiver_socket_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      846 2024-05-10 07:36:14.000000 sacn-1.9.1/sacn/receiving/receiver_socket_base_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-10 07:36:14.000000 sacn-1.9.1/sacn/receiving/receiver_socket_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4030 2024-05-10 07:36:14.000000 sacn-1.9.1/sacn/receiving/receiver_socket_udp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7442 2024-05-10 07:36:14.000000 sacn-1.9.1/sacn/sender.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8805 2024-05-10 07:36:14.000000 sacn-1.9.1/sacn/sender_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 07:36:24.043501 sacn-1.9.1/sacn/sending/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 07:36:14.000000 sacn-1.9.1/sacn/sending/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1302 2024-05-10 07:36:14.000000 sacn-1.9.1/sacn/sending/output.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4531 2024-05-10 07:36:14.000000 sacn-1.9.1/sacn/sending/sender_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7363 2024-05-10 07:36:14.000000 sacn-1.9.1/sacn/sending/sender_handler_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-05-10 07:36:14.000000 sacn-1.9.1/sacn/sending/sender_socket_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-05-10 07:36:14.000000 sacn-1.9.1/sacn/sending/sender_socket_base_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-10 07:36:14.000000 sacn-1.9.1/sacn/sending/sender_socket_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3911 2024-05-10 07:36:14.000000 sacn-1.9.1/sacn/sending/sender_socket_udp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 07:36:24.043501 sacn-1.9.1/sacn.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    16637 2024-05-10 07:36:23.000000 sacn-1.9.1/sacn.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-05-10 07:36:24.000000 sacn-1.9.1/sacn.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 07:36:23.000000 sacn-1.9.1/sacn.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 07:36:23.000000 sacn-1.9.1/sacn.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-10 07:36:23.000000 sacn-1.9.1/sacn.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 07:36:24.043501 sacn-1.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      771 2024-05-10 07:36:14.000000 sacn-1.9.1/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `sacn-1.9.0/setup.py` & `sacn-1.9.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='sacn',
-    version='1.9.0',
+    version='1.9.1',
     description='sACN / E1.31 module for easy handling of DMX data over ethernet',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://www.github.com/Hundemeier/sacn',
     author='Hundemeier',
     author_email='hundemeier99@gmail.com',
     license='MIT License',
```

### Comparing `sacn-1.9.0/README.md` & `sacn-1.9.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -133,35 +133,36 @@
 ### Receiving
 To use the receiving functionality you have to use the `sACNreceiver`.
 
 ```python
 import sacn
 import time
 
-# provide an IP-Address to bind to if you want to send multicast packets from a specific interface
+# provide an IP-Address to bind to if you want to receive multicast packets from a specific interface
 receiver = sacn.sACNreceiver()
 receiver.start()  # start the receiving thread
 
 # define a callback function
 @receiver.listen_on('universe', universe=1)  # listens on universe 1
 def callback(packet):  # packet type: sacn.DataPacket
-    print(packet.dmxData)  # print the received DMX data
+    if packet.dmxStartCode == 0x00:  # ignore non-DMX-data packets
+        print(packet.dmxData)  # print the received DMX data
 
 # optional: if multicast is desired, join with the universe number as parameter
 receiver.join_multicast(1)
 
 time.sleep(10)  # receive for 10 seconds
 
 # optional: if multicast was previously joined
 receiver.leave_multicast(1)
 
 receiver.stop()
 ```
 
-The usage of the receiver is way more simple than the sender.
+The usage of the receiver is simpler than the sender.
 The `sACNreceiver` can be initialized with the following parameters:
  * `bind_address: str`: Provide an IP-Address to bind to if you want to receive multicast packets from a specific interface.
  * `bind_port: int`: Default: 5568. It is not recommended to change this value!
  Only use when you are know what you are doing!
 
 Please keep in mind to not use the callbacks for time consuming tasks!
 If you do this, then the receiver can not react fast enough on incoming messages!
@@ -222,14 +223,15 @@
 `pytest` is used for unit testing and can be executed with `pytest` or `python -m pytest` in the root directory of this repository.
 By default, this skips the integration test, which uses real hardware I/O and might not run in every configuration.
 Use the flag `--run-integration-tests` to run the additional tests (e.g. `python -m pytest --run-integration-tests`)
 
 It is useful to check if the test coverage changed with `coverage run -m pytest` and then `coverage html`, which generates a `htmlcov/index.html` file with all the information.
 
 ### Changelog
+ * 1.9.1: When a sACN packet could not be send out, the exception is raised instead of silently dropped. (Thanks to andrewyager! See #48 for more information)
  * 1.9.0: The behavior of multicast sending and receiving is now unified across most operating systems. This means Windows no longer requires to set a `bind_address` to be able to use multicast or universe discovery. (Thanks to mthespian! See #42 for more information)
  * 1.8.1: Calling `stop` on a sender or receiver now closes the underlying socket too. Note: after stopping a sender or receiver, it can not be started again with `start`. (See #39 for more information)
  * 1.8.0: Added function for removing a listener on a receiver by universe. See `sACNreceiver.remove_listener_from_universe(<universe>)` for more information.
  * 1.7.1: Small changes that might improve timing on the sender. (Thanks to mthespian! See #36 for more information)
  * 1.7.0: Added function for removing a listener on a receiver. See `sACNreceiver.remove_listener(<callback>)` for more information.
  * 1.6.4: Functionality related to sending of sACN data is now mostly covered by tests. Removed undocumented parameters for `sACNsender.start()`.
  * 1.6.3: Functionality related to receiving sACN data is now mostly covered by tests. Fixed a bug, where an exception was thrown on the first `DataPacket` when the stream-termination option was set. (Additional thanks to mthespian! See #31 for more information)
```

### Comparing `sacn-1.9.0/sacn.egg-info/SOURCES.txt` & `sacn-1.9.1/sacn.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE
 README.md
 setup.py
 sacn/__init__.py
 sacn/receiver.py
 sacn/receiver_test.py
 sacn/sender.py
 sacn/sender_test.py
```

### Comparing `sacn-1.9.0/sacn.egg-info/PKG-INFO` & `sacn-1.9.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,265 +1,267 @@
 Metadata-Version: 2.1
 Name: sacn
-Version: 1.9.0
+Version: 1.9.1
 Summary: sACN / E1.31 module for easy handling of DMX data over ethernet
 Home-page: https://www.github.com/Hundemeier/sacn
 Author: Hundemeier
 Author-email: hundemeier99@gmail.com
 License: MIT License
-Description: # sACN / E1.31 module
-        
-        This module is a simple sACN library that support the standard DMX message of the protocol.
-        It is based on the [2016][e1.31] version of the official ANSI E1.31 standard.
-        It has support for sending out DMX data and receiving it. Multiple and multicast universes are supported.
-        For full blown DMX support use [OLA](https://www.openlighting.org/ola/).
-        
-        Currently missing features:
-         * discovery messages (receiving)
-         * E1.31 sync feature (on the receiver side)
-         * custom ports (because this is not recommended)
-        
-        Features:
-         * out-of-order packet detection like the [E1.31][e1.31] 6.7.2
-         * multicast
-         * auto flow control (see [The Internals/Sending](#sending))
-         * E1.31 sync feature (see manual_flush)
-        
-        ## Setup
-        This Package is in the [pypi](https://pypi.org/project/sacn/). To install the package use `pip install sacn`. Python 3.6 or newer required!
-        To use the library `import sacn`.
-        If you want to install directly from source, download or clone the repository and execute `pip install .` where the setup.py is located.
-        For more information on pip installation see: https://packaging.python.org/tutorials/installing-packages/#installing-from-a-local-src-tree
-        
-        ## The Internals
-        ### Sending
-        You can create a new `sACNsender` object and provide the necessary information. Then you have to use `start()`.
-        This creates a new thread that is responsible for sending out the data. Do not forget to `stop()` the thread when
-        finished! If the data is not changed, the same DMX data is sent out every second.
-        
-        The thread sends out the data every *1/fps* seconds. This reduces network traffic even if you give the sender new data
-        more often than the *fps*.
-        A simple description would be to say that the data that you give the sACNsender is subsampled by the *fps*.
-        You can tweak this *fps* by simply change it when creating the `sACNsender` object.
-        
-        This function works according to the [E1.31][e1.31]. See 6.6.1 for more information.
-        
-        Note: Since Version 1.4 there is a manual flush feature available. See Usage/Sending for more info.
-        This feature also uses the sync feature of the sACN protocol (see page 36 on [E1.31][e1.31]).
-        Currently this is not implemented like the recommended way (this does not wait before sending out the sync packet), but
-        it should work on a normal local network without too many latency differences.
-        When the `flush()` function is called, all data is send out at the same time and immediately a sync packet is send out.
-        
-        ### Receiving
-        A very simple solution, as you just create a `sACNreceiver` object and use `start()` a new thread that is running in
-        the background and calls the callbacks when new sACN data arrives.
-        
-        ---
-        ## Usage
-        ### Sending
-        To use the sending functionality you have to use the `sACNsender`.
-        
-        ```python
-        import sacn
-        import time
-        
-        sender = sacn.sACNsender()  # provide an IP-Address to bind to if you want to send multicast packets from a specific interface
-        sender.start()  # start the sending thread
-        sender.activate_output(1)  # start sending out data in the 1st universe
-        sender[1].multicast = True  # set multicast to True
-        # sender[1].destination = "192.168.1.20"  # or provide unicast information.
-        # Keep in mind that if multicast is on, unicast is not used
-        sender[1].dmx_data = (1, 2, 3, 4)  # some test DMX data
-        
-        time.sleep(10)  # send the data for 10 seconds
-        sender.stop()  # do not forget to stop the sender
-        ```
-        
-        You can activate an output universe via `activate_output(<universe>)` and then change the attributes of this universe
-        via `sender[<universe>].<attribute>`. To deactivate an output use `deactivate_output(<universe>)`. The output is
-        terminated like the [E1.31][e1.31] describes it on page 14.
-        
-        If you want to flush manually and the sender thread should not send out automatic, use the
-        `sACNsender.manual_flush` option. This is useful when you want to use a fixture that is using more than one universe
-        and all the data on multiple universes should send out at the same time.
-        
-        Tip: you can get the activated outputs with `get_active_outputs()` and you can move an output with all its settings
-        from one universe to another with `move_universe(<from>, <to>)`.
-        
-        Available Attributes for `sender[<universe>].<attribute>` are:
-         * `destination: str`: the unicast destination as string. (eg "192.168.1.150") Default: "127.0.0.1"
-         * `multicast: bool`: set whether to send out via multicast or not. Default: False
-         If True the data is send out via multicast and not unicast.
-         * `ttl: int`: the time-to-live for the packets that are send out via multicast on this universe. Default: 8
-         * `priority: int`: (must be between 0-200) the priority for this universe that is send out. If multiple sources in a
-         network are sending to the same receiver the data with the highest priority wins. Default: 100
-         * `preview_data: bool`: Flag to mark the data as preview data for visualization purposes. Default: False
-         * `dmx_data: tuple`: the DMX data as a tuple. Max length is 512 and for legacy devices all data that is smaller than
-         512 is merged to a 512 length tuple with 0 as filler value. The values in the tuple have to be [0-255]!
-        
-        `sACNsender` Creates a sender object. A sender is used to manage multiple sACN universes and handles their output.
-        DMX data is send out every second, when no data changes. Some changes may be not send out, because the fps
-        setting defines how often packets are send out to prevent network overuse. So if you change the DMX values too
-        often in a second they may not all been send. Vary the fps parameter to your needs (Default=30).
-         * `bind_address: str`: the IP-Address to bind to.
-         Provide an IP-Address to bind to if you want to send multicast packets from a specific interface.
-         * `bind_port: int`: optionally bind to a specific port. Default=5568. It is not recommended to change the port.
-         Change the port number if you have trouble with another program or the sACNreceiver blocking the port
-         * `source_name: str`: the source name used in the sACN packets. See the [standard][e1.31] for more information.
-         * `cid: tuple`: the cid. If not given, a random CID will be generated. See the [standard][e1.31] for more information.
-         * `fps: int` the frames per second. See explanation above. Has to be >0. Default: 30
-         * `universeDiscovery: bool` if true, universe discovery messages are send out via broadcast every 10s. Default: True
-         * `sync_universe: int` set a specific universe used in the sync-packets. Default: 63999
-        
-        When manually flushed, the E1.31 sync feature is used. So all universe data is send out, and after all data was send out
-        a sync packet is send to all receivers and then they are allowed to display the received data. Note that not all
-        receiver implemented this feature of the sACN protocol.
-        
-        Example for the usage of the manual_flush:
-        ```python
-        import sacn
-        import time
-        
-        sender = sacn.sACNsender()
-        sender.start()
-        sender.activate_output(1)
-        sender.activate_output(2)
-        sender[1].multicast = True
-        sender[2].multicast = True
-        
-        sender.manual_flush = True # turning off the automatic sending of packets
-        sender[1].dmx_data = (1, 2, 3, 4)  # some test DMX data
-        sender[2].dmx_data = (5, 6, 7, 8)  # by the time we are here, the above data would be already send out,
-        # if manual_flush would be False. This could cause some jitter
-        # so instead we are flushing manual
-        time.sleep(1) # let the sender initialize itself
-        sender.flush()
-        sender.manual_flush = False # keep manual flush off as long as possible, because if it is on, the automatic
-        # sending of packets is turned off and that is not recommended
-        sender.stop() # stop sending out
-        ```
-        
-        ### Receiving
-        To use the receiving functionality you have to use the `sACNreceiver`.
-        
-        ```python
-        import sacn
-        import time
-        
-        # provide an IP-Address to bind to if you want to send multicast packets from a specific interface
-        receiver = sacn.sACNreceiver()
-        receiver.start()  # start the receiving thread
-        
-        # define a callback function
-        @receiver.listen_on('universe', universe=1)  # listens on universe 1
-        def callback(packet):  # packet type: sacn.DataPacket
-            print(packet.dmxData)  # print the received DMX data
-        
-        # optional: if multicast is desired, join with the universe number as parameter
-        receiver.join_multicast(1)
-        
-        time.sleep(10)  # receive for 10 seconds
-        
-        # optional: if multicast was previously joined
-        receiver.leave_multicast(1)
-        
-        receiver.stop()
-        ```
-        
-        The usage of the receiver is way more simple than the sender.
-        The `sACNreceiver` can be initialized with the following parameters:
-         * `bind_address: str`: Provide an IP-Address to bind to if you want to receive multicast packets from a specific interface.
-         * `bind_port: int`: Default: 5568. It is not recommended to change this value!
-         Only use when you are know what you are doing!
-        
-        Please keep in mind to not use the callbacks for time consuming tasks!
-        If you do this, then the receiver can not react fast enough on incoming messages!
-        
-        Functions:
-         * `join_multicast(<universe>)`: joins the multicast group for the specific universe.
-         * `leave_multicast(<universe>)`: leave the multicast group specified by the universe.
-         * `get_possible_universes()`: Returns a tuple with all universes that have sources that are sending out data and this
-         data is received by this machine
-         * `register_listener(<trigger>, <callback>, **kwargs)`: register a listener for the given trigger.
-         You can also use the decorator `listen_on(<trigger>, **kwargs)`. Possible trigger so far:
-           * `availability`: gets called when there is no data for a universe anymore or there is now data
-           available. This gets also fired if a source terminates a stream via the stream_termination bit.
-           The callback should get two arguments: `callback(universe, changed)`
-             * `universe: int`: is the universe where the action happened
-             * `changed: str`: can be 'timeout' or 'available'
-           * `universe`: registers a listener for the given universe. The callback gets only one parameter, the DataPacket.
-           You can also use the decorator `@listen_on('universe', universe=<universe>)`.
-           The callback should have one argument: `callback(packet)`
-             * `packet: DataPacket`: the received DataPacket with all information
-         * `remove_listener(<callback>)`: removes a previously registered listener regardless of the trigger.
-         This means a listener can only be removed completely, even if it was listening to multiple universes.
-         If the function never was registered, nothing happens.
-         Note: if a function was registered multiple times, this remove function needs to be called only once.
-         * `remove_listener_from_universe(<universe>)`: removes all listeners from the given universe.
-         This does only have effect on the 'universe' listening trigger.
-         If no function was registered for this universe, nothing happens.
-        
-        ### DataPacket
-        This is an abstract representation of an sACN Data packet that carries the DMX data. This class is used internally by
-        the module and is used in the callbacks of the receiver.
-        
-        The DataPacket provides following attributes:
-         * `sourceName: str`: a string that is used to identify the source. Only the first 64 bytes are used.
-         * `priority: int`: the priority used to manage multiple DMX data on one receiver. [1-200] Default: 100
-         * `universe: int`: the universe for the whole message and its DMX data. [1-63999]
-         * `sequence: int`: the sequence number. Should increment for every new message and can be used to check for wrong
-         order of arriving packets.
-         * `option_StreamTerminated: bool`: True if this packet is the last one of the stream for the given universe.
-         * `option_PreviewData: bool`: True if this data is for visualization purposes.
-         * `option_ForceSync: bool`: True if this should only function in a synchronized state.
-         * `dmxStartCode: int`: the start code for the data tuple. [1-255] Default: 0x00 for streaming level data. See
-         [Alternate START Codes](https://tsp.esta.org/tsp/working_groups/CP/DMXAlternateCodes.php) for more information.
-         * `dmxData: tuple`: the DMX data as tuple. Max length is 512 and shorter tuples getting normalized to a length of 512.
-         Filled with 0 for empty spaces.
-        
-        ## Development
-        Some tools are used to help with development of this library. These are [flake8](https://flake8.pycqa.org), [pytest](https://pytest.org) and [coverage.py](https://coverage.readthedocs.io).
-        
-        Install those tools with pip:
-        
-        ```
-        pip install flake8 pytest pytest-timeout coverage
-        ```
-        
-        `flake8` checks for formatting issues and can be run with `flake8` or `python -m flake8` in the root directory of this repository.
-        
-        `pytest` is used for unit testing and can be executed with `pytest` or `python -m pytest` in the root directory of this repository.
-        By default, this skips the integration test, which uses real hardware I/O and might not run in every configuration.
-        Use the flag `--run-integration-tests` to run the additional tests (e.g. `python -m pytest --run-integration-tests`)
-        
-        It is useful to check if the test coverage changed with `coverage run -m pytest` and then `coverage html`, which generates a `htmlcov/index.html` file with all the information.
-        
-        ### Changelog
-         * 1.9.0: The behavior of multicast sending and receiving is now unified across most operating systems. This means Windows no longer requires to set a `bind_address` to be able to use multicast or universe discovery. (Thanks to mthespian! See #42 for more information)
-         * 1.8.1: Calling `stop` on a sender or receiver now closes the underlying socket too. Note: after stopping a sender or receiver, it can not be started again with `start`. (See #39 for more information)
-         * 1.8.0: Added function for removing a listener on a receiver by universe. See `sACNreceiver.remove_listener_from_universe(<universe>)` for more information.
-         * 1.7.1: Small changes that might improve timing on the sender. (Thanks to mthespian! See #36 for more information)
-         * 1.7.0: Added function for removing a listener on a receiver. See `sACNreceiver.remove_listener(<callback>)` for more information.
-         * 1.6.4: Functionality related to sending of sACN data is now mostly covered by tests. Removed undocumented parameters for `sACNsender.start()`.
-         * 1.6.3: Functionality related to receiving sACN data is now mostly covered by tests. Fixed a bug, where an exception was thrown on the first `DataPacket` when the stream-termination option was set. (Additional thanks to mthespian! See #31 for more information)
-         * 1.6.2: Test coverage of sub-module `messages` is now 100%. Fixed a bug where a too long source name did not throw an exception.
-         Fixed a bug where invalid DMX data could be set on the `DataPacket`. (Thanks to mthespian! See #30 for more information)
-         * 1.6.1: Fixed a bug, where the DMX start code was not set on received packets (Thanks to mthespian! See #29 for more information)
-         * 1.6: Added dmxStartCode property to DataPacket (Thanks to mthespian! see #27 for more information)
-         * 1.5: Performance improvement: Deleted debugging statements in hot path of packet sending and receiving (Thanks to shauneccles! See #25 for more information)
-         * 1.4.6: Fix: When creating a DataPacket with invalid DMX start codes (i.e. not `0x00`) an exception is thrown (Thanks to niggiover9000! See #11 for more information)
-         * 1.4.5: When using a manual flush, only a specified list of universes can be flushed (Thanks to CrazyIvan359! See #22 for more information)
-         * 1.4.4: The universe used for the sACN-sync messages can now be set when creating a `sACNsender` (Thanks to CrazyIvan359! See #21 for more information)
-         * 1.4.3: The sequence number of the sync-packet when using manual flush was not increased (Thanks to @BlakeGarner ! See #19 for more information)
-         * 1.4.2: The internal logging of the receiver_thread and output_thread was using the root logger instead of its module-logger. (Thanks to @mje-nz ! See #18 for more information)
-         * 1.4: Added a manual flush feature for sending out all universes at the same time. Thanks to ahodges9 for the idea.
-        
-        
-        [e1.31]: http://tsp.esta.org/tsp/documents/docs/E1-31-2016.pdf
-        
 Keywords: sacn e131 e1.31 dmx
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# sACN / E1.31 module
+
+This module is a simple sACN library that support the standard DMX message of the protocol.
+It is based on the [2016][e1.31] version of the official ANSI E1.31 standard.
+It has support for sending out DMX data and receiving it. Multiple and multicast universes are supported.
+For full blown DMX support use [OLA](https://www.openlighting.org/ola/).
+
+Currently missing features:
+ * discovery messages (receiving)
+ * E1.31 sync feature (on the receiver side)
+ * custom ports (because this is not recommended)
+
+Features:
+ * out-of-order packet detection like the [E1.31][e1.31] 6.7.2
+ * multicast
+ * auto flow control (see [The Internals/Sending](#sending))
+ * E1.31 sync feature (see manual_flush)
+
+## Setup
+This Package is in the [pypi](https://pypi.org/project/sacn/). To install the package use `pip install sacn`. Python 3.6 or newer required!
+To use the library `import sacn`.
+If you want to install directly from source, download or clone the repository and execute `pip install .` where the setup.py is located.
+For more information on pip installation see: https://packaging.python.org/tutorials/installing-packages/#installing-from-a-local-src-tree
+
+## The Internals
+### Sending
+You can create a new `sACNsender` object and provide the necessary information. Then you have to use `start()`.
+This creates a new thread that is responsible for sending out the data. Do not forget to `stop()` the thread when
+finished! If the data is not changed, the same DMX data is sent out every second.
+
+The thread sends out the data every *1/fps* seconds. This reduces network traffic even if you give the sender new data
+more often than the *fps*.
+A simple description would be to say that the data that you give the sACNsender is subsampled by the *fps*.
+You can tweak this *fps* by simply change it when creating the `sACNsender` object.
+
+This function works according to the [E1.31][e1.31]. See 6.6.1 for more information.
+
+Note: Since Version 1.4 there is a manual flush feature available. See Usage/Sending for more info.
+This feature also uses the sync feature of the sACN protocol (see page 36 on [E1.31][e1.31]).
+Currently this is not implemented like the recommended way (this does not wait before sending out the sync packet), but
+it should work on a normal local network without too many latency differences.
+When the `flush()` function is called, all data is send out at the same time and immediately a sync packet is send out.
+
+### Receiving
+A very simple solution, as you just create a `sACNreceiver` object and use `start()` a new thread that is running in
+the background and calls the callbacks when new sACN data arrives.
+
+---
+## Usage
+### Sending
+To use the sending functionality you have to use the `sACNsender`.
+
+```python
+import sacn
+import time
+
+sender = sacn.sACNsender()  # provide an IP-Address to bind to if you want to send multicast packets from a specific interface
+sender.start()  # start the sending thread
+sender.activate_output(1)  # start sending out data in the 1st universe
+sender[1].multicast = True  # set multicast to True
+# sender[1].destination = "192.168.1.20"  # or provide unicast information.
+# Keep in mind that if multicast is on, unicast is not used
+sender[1].dmx_data = (1, 2, 3, 4)  # some test DMX data
+
+time.sleep(10)  # send the data for 10 seconds
+sender.stop()  # do not forget to stop the sender
+```
+
+You can activate an output universe via `activate_output(<universe>)` and then change the attributes of this universe
+via `sender[<universe>].<attribute>`. To deactivate an output use `deactivate_output(<universe>)`. The output is
+terminated like the [E1.31][e1.31] describes it on page 14.
+
+If you want to flush manually and the sender thread should not send out automatic, use the
+`sACNsender.manual_flush` option. This is useful when you want to use a fixture that is using more than one universe
+and all the data on multiple universes should send out at the same time.
+
+Tip: you can get the activated outputs with `get_active_outputs()` and you can move an output with all its settings
+from one universe to another with `move_universe(<from>, <to>)`.
+
+Available Attributes for `sender[<universe>].<attribute>` are:
+ * `destination: str`: the unicast destination as string. (eg "192.168.1.150") Default: "127.0.0.1"
+ * `multicast: bool`: set whether to send out via multicast or not. Default: False
+ If True the data is send out via multicast and not unicast.
+ * `ttl: int`: the time-to-live for the packets that are send out via multicast on this universe. Default: 8
+ * `priority: int`: (must be between 0-200) the priority for this universe that is send out. If multiple sources in a
+ network are sending to the same receiver the data with the highest priority wins. Default: 100
+ * `preview_data: bool`: Flag to mark the data as preview data for visualization purposes. Default: False
+ * `dmx_data: tuple`: the DMX data as a tuple. Max length is 512 and for legacy devices all data that is smaller than
+ 512 is merged to a 512 length tuple with 0 as filler value. The values in the tuple have to be [0-255]!
+
+`sACNsender` Creates a sender object. A sender is used to manage multiple sACN universes and handles their output.
+DMX data is send out every second, when no data changes. Some changes may be not send out, because the fps
+setting defines how often packets are send out to prevent network overuse. So if you change the DMX values too
+often in a second they may not all been send. Vary the fps parameter to your needs (Default=30).
+ * `bind_address: str`: the IP-Address to bind to.
+ Provide an IP-Address to bind to if you want to send multicast packets from a specific interface.
+ * `bind_port: int`: optionally bind to a specific port. Default=5568. It is not recommended to change the port.
+ Change the port number if you have trouble with another program or the sACNreceiver blocking the port
+ * `source_name: str`: the source name used in the sACN packets. See the [standard][e1.31] for more information.
+ * `cid: tuple`: the cid. If not given, a random CID will be generated. See the [standard][e1.31] for more information.
+ * `fps: int` the frames per second. See explanation above. Has to be >0. Default: 30
+ * `universeDiscovery: bool` if true, universe discovery messages are send out via broadcast every 10s. Default: True
+ * `sync_universe: int` set a specific universe used in the sync-packets. Default: 63999
+
+When manually flushed, the E1.31 sync feature is used. So all universe data is send out, and after all data was send out
+a sync packet is send to all receivers and then they are allowed to display the received data. Note that not all
+receiver implemented this feature of the sACN protocol.
+
+Example for the usage of the manual_flush:
+```python
+import sacn
+import time
+
+sender = sacn.sACNsender()
+sender.start()
+sender.activate_output(1)
+sender.activate_output(2)
+sender[1].multicast = True
+sender[2].multicast = True
+
+sender.manual_flush = True # turning off the automatic sending of packets
+sender[1].dmx_data = (1, 2, 3, 4)  # some test DMX data
+sender[2].dmx_data = (5, 6, 7, 8)  # by the time we are here, the above data would be already send out,
+# if manual_flush would be False. This could cause some jitter
+# so instead we are flushing manual
+time.sleep(1) # let the sender initialize itself
+sender.flush()
+sender.manual_flush = False # keep manual flush off as long as possible, because if it is on, the automatic
+# sending of packets is turned off and that is not recommended
+sender.stop() # stop sending out
+```
+
+### Receiving
+To use the receiving functionality you have to use the `sACNreceiver`.
+
+```python
+import sacn
+import time
+
+# provide an IP-Address to bind to if you want to receive multicast packets from a specific interface
+receiver = sacn.sACNreceiver()
+receiver.start()  # start the receiving thread
+
+# define a callback function
+@receiver.listen_on('universe', universe=1)  # listens on universe 1
+def callback(packet):  # packet type: sacn.DataPacket
+    if packet.dmxStartCode == 0x00:  # ignore non-DMX-data packets
+        print(packet.dmxData)  # print the received DMX data
+
+# optional: if multicast is desired, join with the universe number as parameter
+receiver.join_multicast(1)
+
+time.sleep(10)  # receive for 10 seconds
+
+# optional: if multicast was previously joined
+receiver.leave_multicast(1)
+
+receiver.stop()
+```
+
+The usage of the receiver is simpler than the sender.
+The `sACNreceiver` can be initialized with the following parameters:
+ * `bind_address: str`: Provide an IP-Address to bind to if you want to receive multicast packets from a specific interface.
+ * `bind_port: int`: Default: 5568. It is not recommended to change this value!
+ Only use when you are know what you are doing!
+
+Please keep in mind to not use the callbacks for time consuming tasks!
+If you do this, then the receiver can not react fast enough on incoming messages!
+
+Functions:
+ * `join_multicast(<universe>)`: joins the multicast group for the specific universe.
+ * `leave_multicast(<universe>)`: leave the multicast group specified by the universe.
+ * `get_possible_universes()`: Returns a tuple with all universes that have sources that are sending out data and this
+ data is received by this machine
+ * `register_listener(<trigger>, <callback>, **kwargs)`: register a listener for the given trigger.
+ You can also use the decorator `listen_on(<trigger>, **kwargs)`. Possible trigger so far:
+   * `availability`: gets called when there is no data for a universe anymore or there is now data
+   available. This gets also fired if a source terminates a stream via the stream_termination bit.
+   The callback should get two arguments: `callback(universe, changed)`
+     * `universe: int`: is the universe where the action happened
+     * `changed: str`: can be 'timeout' or 'available'
+   * `universe`: registers a listener for the given universe. The callback gets only one parameter, the DataPacket.
+   You can also use the decorator `@listen_on('universe', universe=<universe>)`.
+   The callback should have one argument: `callback(packet)`
+     * `packet: DataPacket`: the received DataPacket with all information
+ * `remove_listener(<callback>)`: removes a previously registered listener regardless of the trigger.
+ This means a listener can only be removed completely, even if it was listening to multiple universes.
+ If the function never was registered, nothing happens.
+ Note: if a function was registered multiple times, this remove function needs to be called only once.
+ * `remove_listener_from_universe(<universe>)`: removes all listeners from the given universe.
+ This does only have effect on the 'universe' listening trigger.
+ If no function was registered for this universe, nothing happens.
+
+### DataPacket
+This is an abstract representation of an sACN Data packet that carries the DMX data. This class is used internally by
+the module and is used in the callbacks of the receiver.
+
+The DataPacket provides following attributes:
+ * `sourceName: str`: a string that is used to identify the source. Only the first 64 bytes are used.
+ * `priority: int`: the priority used to manage multiple DMX data on one receiver. [1-200] Default: 100
+ * `universe: int`: the universe for the whole message and its DMX data. [1-63999]
+ * `sequence: int`: the sequence number. Should increment for every new message and can be used to check for wrong
+ order of arriving packets.
+ * `option_StreamTerminated: bool`: True if this packet is the last one of the stream for the given universe.
+ * `option_PreviewData: bool`: True if this data is for visualization purposes.
+ * `option_ForceSync: bool`: True if this should only function in a synchronized state.
+ * `dmxStartCode: int`: the start code for the data tuple. [1-255] Default: 0x00 for streaming level data. See
+ [Alternate START Codes](https://tsp.esta.org/tsp/working_groups/CP/DMXAlternateCodes.php) for more information.
+ * `dmxData: tuple`: the DMX data as tuple. Max length is 512 and shorter tuples getting normalized to a length of 512.
+ Filled with 0 for empty spaces.
+
+## Development
+Some tools are used to help with development of this library. These are [flake8](https://flake8.pycqa.org), [pytest](https://pytest.org) and [coverage.py](https://coverage.readthedocs.io).
+
+Install those tools with pip:
+
+```
+pip install flake8 pytest pytest-timeout coverage
+```
+
+`flake8` checks for formatting issues and can be run with `flake8` or `python -m flake8` in the root directory of this repository.
+
+`pytest` is used for unit testing and can be executed with `pytest` or `python -m pytest` in the root directory of this repository.
+By default, this skips the integration test, which uses real hardware I/O and might not run in every configuration.
+Use the flag `--run-integration-tests` to run the additional tests (e.g. `python -m pytest --run-integration-tests`)
+
+It is useful to check if the test coverage changed with `coverage run -m pytest` and then `coverage html`, which generates a `htmlcov/index.html` file with all the information.
+
+### Changelog
+ * 1.9.1: When a sACN packet could not be send out, the exception is raised instead of silently dropped. (Thanks to andrewyager! See #48 for more information)
+ * 1.9.0: The behavior of multicast sending and receiving is now unified across most operating systems. This means Windows no longer requires to set a `bind_address` to be able to use multicast or universe discovery. (Thanks to mthespian! See #42 for more information)
+ * 1.8.1: Calling `stop` on a sender or receiver now closes the underlying socket too. Note: after stopping a sender or receiver, it can not be started again with `start`. (See #39 for more information)
+ * 1.8.0: Added function for removing a listener on a receiver by universe. See `sACNreceiver.remove_listener_from_universe(<universe>)` for more information.
+ * 1.7.1: Small changes that might improve timing on the sender. (Thanks to mthespian! See #36 for more information)
+ * 1.7.0: Added function for removing a listener on a receiver. See `sACNreceiver.remove_listener(<callback>)` for more information.
+ * 1.6.4: Functionality related to sending of sACN data is now mostly covered by tests. Removed undocumented parameters for `sACNsender.start()`.
+ * 1.6.3: Functionality related to receiving sACN data is now mostly covered by tests. Fixed a bug, where an exception was thrown on the first `DataPacket` when the stream-termination option was set. (Additional thanks to mthespian! See #31 for more information)
+ * 1.6.2: Test coverage of sub-module `messages` is now 100%. Fixed a bug where a too long source name did not throw an exception.
+ Fixed a bug where invalid DMX data could be set on the `DataPacket`. (Thanks to mthespian! See #30 for more information)
+ * 1.6.1: Fixed a bug, where the DMX start code was not set on received packets (Thanks to mthespian! See #29 for more information)
+ * 1.6: Added dmxStartCode property to DataPacket (Thanks to mthespian! see #27 for more information)
+ * 1.5: Performance improvement: Deleted debugging statements in hot path of packet sending and receiving (Thanks to shauneccles! See #25 for more information)
+ * 1.4.6: Fix: When creating a DataPacket with invalid DMX start codes (i.e. not `0x00`) an exception is thrown (Thanks to niggiover9000! See #11 for more information)
+ * 1.4.5: When using a manual flush, only a specified list of universes can be flushed (Thanks to CrazyIvan359! See #22 for more information)
+ * 1.4.4: The universe used for the sACN-sync messages can now be set when creating a `sACNsender` (Thanks to CrazyIvan359! See #21 for more information)
+ * 1.4.3: The sequence number of the sync-packet when using manual flush was not increased (Thanks to @BlakeGarner ! See #19 for more information)
+ * 1.4.2: The internal logging of the receiver_thread and output_thread was using the root logger instead of its module-logger. (Thanks to @mje-nz ! See #18 for more information)
+ * 1.4: Added a manual flush feature for sending out all universes at the same time. Thanks to ahodges9 for the idea.
+
+
+[e1.31]: http://tsp.esta.org/tsp/documents/docs/E1-31-2016.pdf
```

### Comparing `sacn-1.9.0/PKG-INFO` & `sacn-1.9.1/sacn.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,265 +1,267 @@
 Metadata-Version: 2.1
 Name: sacn
-Version: 1.9.0
+Version: 1.9.1
 Summary: sACN / E1.31 module for easy handling of DMX data over ethernet
 Home-page: https://www.github.com/Hundemeier/sacn
 Author: Hundemeier
 Author-email: hundemeier99@gmail.com
 License: MIT License
-Description: # sACN / E1.31 module
-        
-        This module is a simple sACN library that support the standard DMX message of the protocol.
-        It is based on the [2016][e1.31] version of the official ANSI E1.31 standard.
-        It has support for sending out DMX data and receiving it. Multiple and multicast universes are supported.
-        For full blown DMX support use [OLA](https://www.openlighting.org/ola/).
-        
-        Currently missing features:
-         * discovery messages (receiving)
-         * E1.31 sync feature (on the receiver side)
-         * custom ports (because this is not recommended)
-        
-        Features:
-         * out-of-order packet detection like the [E1.31][e1.31] 6.7.2
-         * multicast
-         * auto flow control (see [The Internals/Sending](#sending))
-         * E1.31 sync feature (see manual_flush)
-        
-        ## Setup
-        This Package is in the [pypi](https://pypi.org/project/sacn/). To install the package use `pip install sacn`. Python 3.6 or newer required!
-        To use the library `import sacn`.
-        If you want to install directly from source, download or clone the repository and execute `pip install .` where the setup.py is located.
-        For more information on pip installation see: https://packaging.python.org/tutorials/installing-packages/#installing-from-a-local-src-tree
-        
-        ## The Internals
-        ### Sending
-        You can create a new `sACNsender` object and provide the necessary information. Then you have to use `start()`.
-        This creates a new thread that is responsible for sending out the data. Do not forget to `stop()` the thread when
-        finished! If the data is not changed, the same DMX data is sent out every second.
-        
-        The thread sends out the data every *1/fps* seconds. This reduces network traffic even if you give the sender new data
-        more often than the *fps*.
-        A simple description would be to say that the data that you give the sACNsender is subsampled by the *fps*.
-        You can tweak this *fps* by simply change it when creating the `sACNsender` object.
-        
-        This function works according to the [E1.31][e1.31]. See 6.6.1 for more information.
-        
-        Note: Since Version 1.4 there is a manual flush feature available. See Usage/Sending for more info.
-        This feature also uses the sync feature of the sACN protocol (see page 36 on [E1.31][e1.31]).
-        Currently this is not implemented like the recommended way (this does not wait before sending out the sync packet), but
-        it should work on a normal local network without too many latency differences.
-        When the `flush()` function is called, all data is send out at the same time and immediately a sync packet is send out.
-        
-        ### Receiving
-        A very simple solution, as you just create a `sACNreceiver` object and use `start()` a new thread that is running in
-        the background and calls the callbacks when new sACN data arrives.
-        
-        ---
-        ## Usage
-        ### Sending
-        To use the sending functionality you have to use the `sACNsender`.
-        
-        ```python
-        import sacn
-        import time
-        
-        sender = sacn.sACNsender()  # provide an IP-Address to bind to if you want to send multicast packets from a specific interface
-        sender.start()  # start the sending thread
-        sender.activate_output(1)  # start sending out data in the 1st universe
-        sender[1].multicast = True  # set multicast to True
-        # sender[1].destination = "192.168.1.20"  # or provide unicast information.
-        # Keep in mind that if multicast is on, unicast is not used
-        sender[1].dmx_data = (1, 2, 3, 4)  # some test DMX data
-        
-        time.sleep(10)  # send the data for 10 seconds
-        sender.stop()  # do not forget to stop the sender
-        ```
-        
-        You can activate an output universe via `activate_output(<universe>)` and then change the attributes of this universe
-        via `sender[<universe>].<attribute>`. To deactivate an output use `deactivate_output(<universe>)`. The output is
-        terminated like the [E1.31][e1.31] describes it on page 14.
-        
-        If you want to flush manually and the sender thread should not send out automatic, use the
-        `sACNsender.manual_flush` option. This is useful when you want to use a fixture that is using more than one universe
-        and all the data on multiple universes should send out at the same time.
-        
-        Tip: you can get the activated outputs with `get_active_outputs()` and you can move an output with all its settings
-        from one universe to another with `move_universe(<from>, <to>)`.
-        
-        Available Attributes for `sender[<universe>].<attribute>` are:
-         * `destination: str`: the unicast destination as string. (eg "192.168.1.150") Default: "127.0.0.1"
-         * `multicast: bool`: set whether to send out via multicast or not. Default: False
-         If True the data is send out via multicast and not unicast.
-         * `ttl: int`: the time-to-live for the packets that are send out via multicast on this universe. Default: 8
-         * `priority: int`: (must be between 0-200) the priority for this universe that is send out. If multiple sources in a
-         network are sending to the same receiver the data with the highest priority wins. Default: 100
-         * `preview_data: bool`: Flag to mark the data as preview data for visualization purposes. Default: False
-         * `dmx_data: tuple`: the DMX data as a tuple. Max length is 512 and for legacy devices all data that is smaller than
-         512 is merged to a 512 length tuple with 0 as filler value. The values in the tuple have to be [0-255]!
-        
-        `sACNsender` Creates a sender object. A sender is used to manage multiple sACN universes and handles their output.
-        DMX data is send out every second, when no data changes. Some changes may be not send out, because the fps
-        setting defines how often packets are send out to prevent network overuse. So if you change the DMX values too
-        often in a second they may not all been send. Vary the fps parameter to your needs (Default=30).
-         * `bind_address: str`: the IP-Address to bind to.
-         Provide an IP-Address to bind to if you want to send multicast packets from a specific interface.
-         * `bind_port: int`: optionally bind to a specific port. Default=5568. It is not recommended to change the port.
-         Change the port number if you have trouble with another program or the sACNreceiver blocking the port
-         * `source_name: str`: the source name used in the sACN packets. See the [standard][e1.31] for more information.
-         * `cid: tuple`: the cid. If not given, a random CID will be generated. See the [standard][e1.31] for more information.
-         * `fps: int` the frames per second. See explanation above. Has to be >0. Default: 30
-         * `universeDiscovery: bool` if true, universe discovery messages are send out via broadcast every 10s. Default: True
-         * `sync_universe: int` set a specific universe used in the sync-packets. Default: 63999
-        
-        When manually flushed, the E1.31 sync feature is used. So all universe data is send out, and after all data was send out
-        a sync packet is send to all receivers and then they are allowed to display the received data. Note that not all
-        receiver implemented this feature of the sACN protocol.
-        
-        Example for the usage of the manual_flush:
-        ```python
-        import sacn
-        import time
-        
-        sender = sacn.sACNsender()
-        sender.start()
-        sender.activate_output(1)
-        sender.activate_output(2)
-        sender[1].multicast = True
-        sender[2].multicast = True
-        
-        sender.manual_flush = True # turning off the automatic sending of packets
-        sender[1].dmx_data = (1, 2, 3, 4)  # some test DMX data
-        sender[2].dmx_data = (5, 6, 7, 8)  # by the time we are here, the above data would be already send out,
-        # if manual_flush would be False. This could cause some jitter
-        # so instead we are flushing manual
-        time.sleep(1) # let the sender initialize itself
-        sender.flush()
-        sender.manual_flush = False # keep manual flush off as long as possible, because if it is on, the automatic
-        # sending of packets is turned off and that is not recommended
-        sender.stop() # stop sending out
-        ```
-        
-        ### Receiving
-        To use the receiving functionality you have to use the `sACNreceiver`.
-        
-        ```python
-        import sacn
-        import time
-        
-        # provide an IP-Address to bind to if you want to send multicast packets from a specific interface
-        receiver = sacn.sACNreceiver()
-        receiver.start()  # start the receiving thread
-        
-        # define a callback function
-        @receiver.listen_on('universe', universe=1)  # listens on universe 1
-        def callback(packet):  # packet type: sacn.DataPacket
-            print(packet.dmxData)  # print the received DMX data
-        
-        # optional: if multicast is desired, join with the universe number as parameter
-        receiver.join_multicast(1)
-        
-        time.sleep(10)  # receive for 10 seconds
-        
-        # optional: if multicast was previously joined
-        receiver.leave_multicast(1)
-        
-        receiver.stop()
-        ```
-        
-        The usage of the receiver is way more simple than the sender.
-        The `sACNreceiver` can be initialized with the following parameters:
-         * `bind_address: str`: Provide an IP-Address to bind to if you want to receive multicast packets from a specific interface.
-         * `bind_port: int`: Default: 5568. It is not recommended to change this value!
-         Only use when you are know what you are doing!
-        
-        Please keep in mind to not use the callbacks for time consuming tasks!
-        If you do this, then the receiver can not react fast enough on incoming messages!
-        
-        Functions:
-         * `join_multicast(<universe>)`: joins the multicast group for the specific universe.
-         * `leave_multicast(<universe>)`: leave the multicast group specified by the universe.
-         * `get_possible_universes()`: Returns a tuple with all universes that have sources that are sending out data and this
-         data is received by this machine
-         * `register_listener(<trigger>, <callback>, **kwargs)`: register a listener for the given trigger.
-         You can also use the decorator `listen_on(<trigger>, **kwargs)`. Possible trigger so far:
-           * `availability`: gets called when there is no data for a universe anymore or there is now data
-           available. This gets also fired if a source terminates a stream via the stream_termination bit.
-           The callback should get two arguments: `callback(universe, changed)`
-             * `universe: int`: is the universe where the action happened
-             * `changed: str`: can be 'timeout' or 'available'
-           * `universe`: registers a listener for the given universe. The callback gets only one parameter, the DataPacket.
-           You can also use the decorator `@listen_on('universe', universe=<universe>)`.
-           The callback should have one argument: `callback(packet)`
-             * `packet: DataPacket`: the received DataPacket with all information
-         * `remove_listener(<callback>)`: removes a previously registered listener regardless of the trigger.
-         This means a listener can only be removed completely, even if it was listening to multiple universes.
-         If the function never was registered, nothing happens.
-         Note: if a function was registered multiple times, this remove function needs to be called only once.
-         * `remove_listener_from_universe(<universe>)`: removes all listeners from the given universe.
-         This does only have effect on the 'universe' listening trigger.
-         If no function was registered for this universe, nothing happens.
-        
-        ### DataPacket
-        This is an abstract representation of an sACN Data packet that carries the DMX data. This class is used internally by
-        the module and is used in the callbacks of the receiver.
-        
-        The DataPacket provides following attributes:
-         * `sourceName: str`: a string that is used to identify the source. Only the first 64 bytes are used.
-         * `priority: int`: the priority used to manage multiple DMX data on one receiver. [1-200] Default: 100
-         * `universe: int`: the universe for the whole message and its DMX data. [1-63999]
-         * `sequence: int`: the sequence number. Should increment for every new message and can be used to check for wrong
-         order of arriving packets.
-         * `option_StreamTerminated: bool`: True if this packet is the last one of the stream for the given universe.
-         * `option_PreviewData: bool`: True if this data is for visualization purposes.
-         * `option_ForceSync: bool`: True if this should only function in a synchronized state.
-         * `dmxStartCode: int`: the start code for the data tuple. [1-255] Default: 0x00 for streaming level data. See
-         [Alternate START Codes](https://tsp.esta.org/tsp/working_groups/CP/DMXAlternateCodes.php) for more information.
-         * `dmxData: tuple`: the DMX data as tuple. Max length is 512 and shorter tuples getting normalized to a length of 512.
-         Filled with 0 for empty spaces.
-        
-        ## Development
-        Some tools are used to help with development of this library. These are [flake8](https://flake8.pycqa.org), [pytest](https://pytest.org) and [coverage.py](https://coverage.readthedocs.io).
-        
-        Install those tools with pip:
-        
-        ```
-        pip install flake8 pytest pytest-timeout coverage
-        ```
-        
-        `flake8` checks for formatting issues and can be run with `flake8` or `python -m flake8` in the root directory of this repository.
-        
-        `pytest` is used for unit testing and can be executed with `pytest` or `python -m pytest` in the root directory of this repository.
-        By default, this skips the integration test, which uses real hardware I/O and might not run in every configuration.
-        Use the flag `--run-integration-tests` to run the additional tests (e.g. `python -m pytest --run-integration-tests`)
-        
-        It is useful to check if the test coverage changed with `coverage run -m pytest` and then `coverage html`, which generates a `htmlcov/index.html` file with all the information.
-        
-        ### Changelog
-         * 1.9.0: The behavior of multicast sending and receiving is now unified across most operating systems. This means Windows no longer requires to set a `bind_address` to be able to use multicast or universe discovery. (Thanks to mthespian! See #42 for more information)
-         * 1.8.1: Calling `stop` on a sender or receiver now closes the underlying socket too. Note: after stopping a sender or receiver, it can not be started again with `start`. (See #39 for more information)
-         * 1.8.0: Added function for removing a listener on a receiver by universe. See `sACNreceiver.remove_listener_from_universe(<universe>)` for more information.
-         * 1.7.1: Small changes that might improve timing on the sender. (Thanks to mthespian! See #36 for more information)
-         * 1.7.0: Added function for removing a listener on a receiver. See `sACNreceiver.remove_listener(<callback>)` for more information.
-         * 1.6.4: Functionality related to sending of sACN data is now mostly covered by tests. Removed undocumented parameters for `sACNsender.start()`.
-         * 1.6.3: Functionality related to receiving sACN data is now mostly covered by tests. Fixed a bug, where an exception was thrown on the first `DataPacket` when the stream-termination option was set. (Additional thanks to mthespian! See #31 for more information)
-         * 1.6.2: Test coverage of sub-module `messages` is now 100%. Fixed a bug where a too long source name did not throw an exception.
-         Fixed a bug where invalid DMX data could be set on the `DataPacket`. (Thanks to mthespian! See #30 for more information)
-         * 1.6.1: Fixed a bug, where the DMX start code was not set on received packets (Thanks to mthespian! See #29 for more information)
-         * 1.6: Added dmxStartCode property to DataPacket (Thanks to mthespian! see #27 for more information)
-         * 1.5: Performance improvement: Deleted debugging statements in hot path of packet sending and receiving (Thanks to shauneccles! See #25 for more information)
-         * 1.4.6: Fix: When creating a DataPacket with invalid DMX start codes (i.e. not `0x00`) an exception is thrown (Thanks to niggiover9000! See #11 for more information)
-         * 1.4.5: When using a manual flush, only a specified list of universes can be flushed (Thanks to CrazyIvan359! See #22 for more information)
-         * 1.4.4: The universe used for the sACN-sync messages can now be set when creating a `sACNsender` (Thanks to CrazyIvan359! See #21 for more information)
-         * 1.4.3: The sequence number of the sync-packet when using manual flush was not increased (Thanks to @BlakeGarner ! See #19 for more information)
-         * 1.4.2: The internal logging of the receiver_thread and output_thread was using the root logger instead of its module-logger. (Thanks to @mje-nz ! See #18 for more information)
-         * 1.4: Added a manual flush feature for sending out all universes at the same time. Thanks to ahodges9 for the idea.
-        
-        
-        [e1.31]: http://tsp.esta.org/tsp/documents/docs/E1-31-2016.pdf
-        
 Keywords: sacn e131 e1.31 dmx
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# sACN / E1.31 module
+
+This module is a simple sACN library that support the standard DMX message of the protocol.
+It is based on the [2016][e1.31] version of the official ANSI E1.31 standard.
+It has support for sending out DMX data and receiving it. Multiple and multicast universes are supported.
+For full blown DMX support use [OLA](https://www.openlighting.org/ola/).
+
+Currently missing features:
+ * discovery messages (receiving)
+ * E1.31 sync feature (on the receiver side)
+ * custom ports (because this is not recommended)
+
+Features:
+ * out-of-order packet detection like the [E1.31][e1.31] 6.7.2
+ * multicast
+ * auto flow control (see [The Internals/Sending](#sending))
+ * E1.31 sync feature (see manual_flush)
+
+## Setup
+This Package is in the [pypi](https://pypi.org/project/sacn/). To install the package use `pip install sacn`. Python 3.6 or newer required!
+To use the library `import sacn`.
+If you want to install directly from source, download or clone the repository and execute `pip install .` where the setup.py is located.
+For more information on pip installation see: https://packaging.python.org/tutorials/installing-packages/#installing-from-a-local-src-tree
+
+## The Internals
+### Sending
+You can create a new `sACNsender` object and provide the necessary information. Then you have to use `start()`.
+This creates a new thread that is responsible for sending out the data. Do not forget to `stop()` the thread when
+finished! If the data is not changed, the same DMX data is sent out every second.
+
+The thread sends out the data every *1/fps* seconds. This reduces network traffic even if you give the sender new data
+more often than the *fps*.
+A simple description would be to say that the data that you give the sACNsender is subsampled by the *fps*.
+You can tweak this *fps* by simply change it when creating the `sACNsender` object.
+
+This function works according to the [E1.31][e1.31]. See 6.6.1 for more information.
+
+Note: Since Version 1.4 there is a manual flush feature available. See Usage/Sending for more info.
+This feature also uses the sync feature of the sACN protocol (see page 36 on [E1.31][e1.31]).
+Currently this is not implemented like the recommended way (this does not wait before sending out the sync packet), but
+it should work on a normal local network without too many latency differences.
+When the `flush()` function is called, all data is send out at the same time and immediately a sync packet is send out.
+
+### Receiving
+A very simple solution, as you just create a `sACNreceiver` object and use `start()` a new thread that is running in
+the background and calls the callbacks when new sACN data arrives.
+
+---
+## Usage
+### Sending
+To use the sending functionality you have to use the `sACNsender`.
+
+```python
+import sacn
+import time
+
+sender = sacn.sACNsender()  # provide an IP-Address to bind to if you want to send multicast packets from a specific interface
+sender.start()  # start the sending thread
+sender.activate_output(1)  # start sending out data in the 1st universe
+sender[1].multicast = True  # set multicast to True
+# sender[1].destination = "192.168.1.20"  # or provide unicast information.
+# Keep in mind that if multicast is on, unicast is not used
+sender[1].dmx_data = (1, 2, 3, 4)  # some test DMX data
+
+time.sleep(10)  # send the data for 10 seconds
+sender.stop()  # do not forget to stop the sender
+```
+
+You can activate an output universe via `activate_output(<universe>)` and then change the attributes of this universe
+via `sender[<universe>].<attribute>`. To deactivate an output use `deactivate_output(<universe>)`. The output is
+terminated like the [E1.31][e1.31] describes it on page 14.
+
+If you want to flush manually and the sender thread should not send out automatic, use the
+`sACNsender.manual_flush` option. This is useful when you want to use a fixture that is using more than one universe
+and all the data on multiple universes should send out at the same time.
+
+Tip: you can get the activated outputs with `get_active_outputs()` and you can move an output with all its settings
+from one universe to another with `move_universe(<from>, <to>)`.
+
+Available Attributes for `sender[<universe>].<attribute>` are:
+ * `destination: str`: the unicast destination as string. (eg "192.168.1.150") Default: "127.0.0.1"
+ * `multicast: bool`: set whether to send out via multicast or not. Default: False
+ If True the data is send out via multicast and not unicast.
+ * `ttl: int`: the time-to-live for the packets that are send out via multicast on this universe. Default: 8
+ * `priority: int`: (must be between 0-200) the priority for this universe that is send out. If multiple sources in a
+ network are sending to the same receiver the data with the highest priority wins. Default: 100
+ * `preview_data: bool`: Flag to mark the data as preview data for visualization purposes. Default: False
+ * `dmx_data: tuple`: the DMX data as a tuple. Max length is 512 and for legacy devices all data that is smaller than
+ 512 is merged to a 512 length tuple with 0 as filler value. The values in the tuple have to be [0-255]!
+
+`sACNsender` Creates a sender object. A sender is used to manage multiple sACN universes and handles their output.
+DMX data is send out every second, when no data changes. Some changes may be not send out, because the fps
+setting defines how often packets are send out to prevent network overuse. So if you change the DMX values too
+often in a second they may not all been send. Vary the fps parameter to your needs (Default=30).
+ * `bind_address: str`: the IP-Address to bind to.
+ Provide an IP-Address to bind to if you want to send multicast packets from a specific interface.
+ * `bind_port: int`: optionally bind to a specific port. Default=5568. It is not recommended to change the port.
+ Change the port number if you have trouble with another program or the sACNreceiver blocking the port
+ * `source_name: str`: the source name used in the sACN packets. See the [standard][e1.31] for more information.
+ * `cid: tuple`: the cid. If not given, a random CID will be generated. See the [standard][e1.31] for more information.
+ * `fps: int` the frames per second. See explanation above. Has to be >0. Default: 30
+ * `universeDiscovery: bool` if true, universe discovery messages are send out via broadcast every 10s. Default: True
+ * `sync_universe: int` set a specific universe used in the sync-packets. Default: 63999
+
+When manually flushed, the E1.31 sync feature is used. So all universe data is send out, and after all data was send out
+a sync packet is send to all receivers and then they are allowed to display the received data. Note that not all
+receiver implemented this feature of the sACN protocol.
+
+Example for the usage of the manual_flush:
+```python
+import sacn
+import time
+
+sender = sacn.sACNsender()
+sender.start()
+sender.activate_output(1)
+sender.activate_output(2)
+sender[1].multicast = True
+sender[2].multicast = True
+
+sender.manual_flush = True # turning off the automatic sending of packets
+sender[1].dmx_data = (1, 2, 3, 4)  # some test DMX data
+sender[2].dmx_data = (5, 6, 7, 8)  # by the time we are here, the above data would be already send out,
+# if manual_flush would be False. This could cause some jitter
+# so instead we are flushing manual
+time.sleep(1) # let the sender initialize itself
+sender.flush()
+sender.manual_flush = False # keep manual flush off as long as possible, because if it is on, the automatic
+# sending of packets is turned off and that is not recommended
+sender.stop() # stop sending out
+```
+
+### Receiving
+To use the receiving functionality you have to use the `sACNreceiver`.
+
+```python
+import sacn
+import time
+
+# provide an IP-Address to bind to if you want to receive multicast packets from a specific interface
+receiver = sacn.sACNreceiver()
+receiver.start()  # start the receiving thread
+
+# define a callback function
+@receiver.listen_on('universe', universe=1)  # listens on universe 1
+def callback(packet):  # packet type: sacn.DataPacket
+    if packet.dmxStartCode == 0x00:  # ignore non-DMX-data packets
+        print(packet.dmxData)  # print the received DMX data
+
+# optional: if multicast is desired, join with the universe number as parameter
+receiver.join_multicast(1)
+
+time.sleep(10)  # receive for 10 seconds
+
+# optional: if multicast was previously joined
+receiver.leave_multicast(1)
+
+receiver.stop()
+```
+
+The usage of the receiver is simpler than the sender.
+The `sACNreceiver` can be initialized with the following parameters:
+ * `bind_address: str`: Provide an IP-Address to bind to if you want to receive multicast packets from a specific interface.
+ * `bind_port: int`: Default: 5568. It is not recommended to change this value!
+ Only use when you are know what you are doing!
+
+Please keep in mind to not use the callbacks for time consuming tasks!
+If you do this, then the receiver can not react fast enough on incoming messages!
+
+Functions:
+ * `join_multicast(<universe>)`: joins the multicast group for the specific universe.
+ * `leave_multicast(<universe>)`: leave the multicast group specified by the universe.
+ * `get_possible_universes()`: Returns a tuple with all universes that have sources that are sending out data and this
+ data is received by this machine
+ * `register_listener(<trigger>, <callback>, **kwargs)`: register a listener for the given trigger.
+ You can also use the decorator `listen_on(<trigger>, **kwargs)`. Possible trigger so far:
+   * `availability`: gets called when there is no data for a universe anymore or there is now data
+   available. This gets also fired if a source terminates a stream via the stream_termination bit.
+   The callback should get two arguments: `callback(universe, changed)`
+     * `universe: int`: is the universe where the action happened
+     * `changed: str`: can be 'timeout' or 'available'
+   * `universe`: registers a listener for the given universe. The callback gets only one parameter, the DataPacket.
+   You can also use the decorator `@listen_on('universe', universe=<universe>)`.
+   The callback should have one argument: `callback(packet)`
+     * `packet: DataPacket`: the received DataPacket with all information
+ * `remove_listener(<callback>)`: removes a previously registered listener regardless of the trigger.
+ This means a listener can only be removed completely, even if it was listening to multiple universes.
+ If the function never was registered, nothing happens.
+ Note: if a function was registered multiple times, this remove function needs to be called only once.
+ * `remove_listener_from_universe(<universe>)`: removes all listeners from the given universe.
+ This does only have effect on the 'universe' listening trigger.
+ If no function was registered for this universe, nothing happens.
+
+### DataPacket
+This is an abstract representation of an sACN Data packet that carries the DMX data. This class is used internally by
+the module and is used in the callbacks of the receiver.
+
+The DataPacket provides following attributes:
+ * `sourceName: str`: a string that is used to identify the source. Only the first 64 bytes are used.
+ * `priority: int`: the priority used to manage multiple DMX data on one receiver. [1-200] Default: 100
+ * `universe: int`: the universe for the whole message and its DMX data. [1-63999]
+ * `sequence: int`: the sequence number. Should increment for every new message and can be used to check for wrong
+ order of arriving packets.
+ * `option_StreamTerminated: bool`: True if this packet is the last one of the stream for the given universe.
+ * `option_PreviewData: bool`: True if this data is for visualization purposes.
+ * `option_ForceSync: bool`: True if this should only function in a synchronized state.
+ * `dmxStartCode: int`: the start code for the data tuple. [1-255] Default: 0x00 for streaming level data. See
+ [Alternate START Codes](https://tsp.esta.org/tsp/working_groups/CP/DMXAlternateCodes.php) for more information.
+ * `dmxData: tuple`: the DMX data as tuple. Max length is 512 and shorter tuples getting normalized to a length of 512.
+ Filled with 0 for empty spaces.
+
+## Development
+Some tools are used to help with development of this library. These are [flake8](https://flake8.pycqa.org), [pytest](https://pytest.org) and [coverage.py](https://coverage.readthedocs.io).
+
+Install those tools with pip:
+
+```
+pip install flake8 pytest pytest-timeout coverage
+```
+
+`flake8` checks for formatting issues and can be run with `flake8` or `python -m flake8` in the root directory of this repository.
+
+`pytest` is used for unit testing and can be executed with `pytest` or `python -m pytest` in the root directory of this repository.
+By default, this skips the integration test, which uses real hardware I/O and might not run in every configuration.
+Use the flag `--run-integration-tests` to run the additional tests (e.g. `python -m pytest --run-integration-tests`)
+
+It is useful to check if the test coverage changed with `coverage run -m pytest` and then `coverage html`, which generates a `htmlcov/index.html` file with all the information.
+
+### Changelog
+ * 1.9.1: When a sACN packet could not be send out, the exception is raised instead of silently dropped. (Thanks to andrewyager! See #48 for more information)
+ * 1.9.0: The behavior of multicast sending and receiving is now unified across most operating systems. This means Windows no longer requires to set a `bind_address` to be able to use multicast or universe discovery. (Thanks to mthespian! See #42 for more information)
+ * 1.8.1: Calling `stop` on a sender or receiver now closes the underlying socket too. Note: after stopping a sender or receiver, it can not be started again with `start`. (See #39 for more information)
+ * 1.8.0: Added function for removing a listener on a receiver by universe. See `sACNreceiver.remove_listener_from_universe(<universe>)` for more information.
+ * 1.7.1: Small changes that might improve timing on the sender. (Thanks to mthespian! See #36 for more information)
+ * 1.7.0: Added function for removing a listener on a receiver. See `sACNreceiver.remove_listener(<callback>)` for more information.
+ * 1.6.4: Functionality related to sending of sACN data is now mostly covered by tests. Removed undocumented parameters for `sACNsender.start()`.
+ * 1.6.3: Functionality related to receiving sACN data is now mostly covered by tests. Fixed a bug, where an exception was thrown on the first `DataPacket` when the stream-termination option was set. (Additional thanks to mthespian! See #31 for more information)
+ * 1.6.2: Test coverage of sub-module `messages` is now 100%. Fixed a bug where a too long source name did not throw an exception.
+ Fixed a bug where invalid DMX data could be set on the `DataPacket`. (Thanks to mthespian! See #30 for more information)
+ * 1.6.1: Fixed a bug, where the DMX start code was not set on received packets (Thanks to mthespian! See #29 for more information)
+ * 1.6: Added dmxStartCode property to DataPacket (Thanks to mthespian! see #27 for more information)
+ * 1.5: Performance improvement: Deleted debugging statements in hot path of packet sending and receiving (Thanks to shauneccles! See #25 for more information)
+ * 1.4.6: Fix: When creating a DataPacket with invalid DMX start codes (i.e. not `0x00`) an exception is thrown (Thanks to niggiover9000! See #11 for more information)
+ * 1.4.5: When using a manual flush, only a specified list of universes can be flushed (Thanks to CrazyIvan359! See #22 for more information)
+ * 1.4.4: The universe used for the sACN-sync messages can now be set when creating a `sACNsender` (Thanks to CrazyIvan359! See #21 for more information)
+ * 1.4.3: The sequence number of the sync-packet when using manual flush was not increased (Thanks to @BlakeGarner ! See #19 for more information)
+ * 1.4.2: The internal logging of the receiver_thread and output_thread was using the root logger instead of its module-logger. (Thanks to @mje-nz ! See #18 for more information)
+ * 1.4: Added a manual flush feature for sending out all universes at the same time. Thanks to ahodges9 for the idea.
+
+
+[e1.31]: http://tsp.esta.org/tsp/documents/docs/E1-31-2016.pdf
```

### Comparing `sacn-1.9.0/sacn/sending/sender_handler.py` & `sacn-1.9.1/sacn/sending/sender_handler.py`

 * *Files identical despite different names*

### Comparing `sacn-1.9.0/sacn/sending/output.py` & `sacn-1.9.1/sacn/sending/output.py`

 * *Files identical despite different names*

### Comparing `sacn-1.9.0/sacn/sending/sender_socket_test.py` & `sacn-1.9.1/sacn/sending/sender_socket_test.py`

 * *Files identical despite different names*

### Comparing `sacn-1.9.0/sacn/sending/sender_socket_udp.py` & `sacn-1.9.1/sacn/sending/sender_socket_udp.py`

 * *Files 1% similar despite different names*

```diff
@@ -89,8 +89,9 @@
         self.send_packet(data.getBytes(), destination='<broadcast>')
 
     def send_packet(self, data: bytearray, destination: str) -> None:
         data_raw = bytearray(data)
         try:
             self._socket.sendto(data_raw, (destination, DEFAULT_PORT))
         except OSError as e:
-            self._logger.warning('Failed to send packet', exc_info=e)
+            self._logger.exception('Failed to send packet', exc_info=e)
+            raise
```

### Comparing `sacn-1.9.0/sacn/sending/sender_socket_base.py` & `sacn-1.9.1/sacn/sending/sender_socket_base.py`

 * *Files identical despite different names*

### Comparing `sacn-1.9.0/sacn/sending/sender_handler_test.py` & `sacn-1.9.1/sacn/sending/sender_handler_test.py`

 * *Files identical despite different names*

### Comparing `sacn-1.9.0/sacn/sending/sender_socket_base_test.py` & `sacn-1.9.1/sacn/sending/sender_socket_base_test.py`

 * *Files identical despite different names*

### Comparing `sacn-1.9.0/sacn/sender.py` & `sacn-1.9.1/sacn/sender.py`

 * *Files identical despite different names*

### Comparing `sacn-1.9.0/sacn/receiver.py` & `sacn-1.9.1/sacn/receiver.py`

 * *Files identical despite different names*

### Comparing `sacn-1.9.0/sacn/messages/universe_discovery_test.py` & `sacn-1.9.1/sacn/messages/universe_discovery_test.py`

 * *Files identical despite different names*

### Comparing `sacn-1.9.0/sacn/messages/data_packet_test.py` & `sacn-1.9.1/sacn/messages/data_packet_test.py`

 * *Files identical despite different names*

### Comparing `sacn-1.9.0/sacn/messages/sync_packet.py` & `sacn-1.9.1/sacn/messages/sync_packet.py`

 * *Files identical despite different names*

### Comparing `sacn-1.9.0/sacn/messages/root_layer.py` & `sacn-1.9.1/sacn/messages/root_layer.py`

 * *Files identical despite different names*

### Comparing `sacn-1.9.0/sacn/messages/root_layer_test.py` & `sacn-1.9.1/sacn/messages/root_layer_test.py`

 * *Files identical despite different names*

### Comparing `sacn-1.9.0/sacn/messages/data_types.py` & `sacn-1.9.1/sacn/messages/data_types.py`

 * *Files identical despite different names*

### Comparing `sacn-1.9.0/sacn/messages/sync_packet_test.py` & `sacn-1.9.1/sacn/messages/sync_packet_test.py`

 * *Files identical despite different names*

### Comparing `sacn-1.9.0/sacn/messages/universe_discovery.py` & `sacn-1.9.1/sacn/messages/universe_discovery.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 This class represents an universe discovery packet of the E1.31 Standard.
 """
 from typing import List
 
 from sacn.messages.root_layer import \
     VECTOR_ROOT_E131_EXTENDED, \
     VECTOR_E131_EXTENDED_DISCOVERY, \
-    VECTOR_UNIVERSE_DISCOVERY_UNIVERSE_LIST,\
+    VECTOR_UNIVERSE_DISCOVERY_UNIVERSE_LIST, \
     RootLayer, \
     int_to_bytes, \
     byte_tuple_to_int, \
     make_flagsandlength
 
 
 class UniverseDiscoveryPacket(RootLayer):
```

### Comparing `sacn-1.9.0/sacn/messages/general_test.py` & `sacn-1.9.1/sacn/messages/general_test.py`

 * *Files identical despite different names*

### Comparing `sacn-1.9.0/sacn/messages/data_types_test.py` & `sacn-1.9.1/sacn/messages/data_types_test.py`

 * *Files identical despite different names*

### Comparing `sacn-1.9.0/sacn/messages/data_packet.py` & `sacn-1.9.1/sacn/messages/data_packet.py`

 * *Files identical despite different names*

### Comparing `sacn-1.9.0/sacn/receiver_test.py` & `sacn-1.9.1/sacn/receiver_test.py`

 * *Files identical despite different names*

### Comparing `sacn-1.9.0/sacn/receiving/receiver_handler_test.py` & `sacn-1.9.1/sacn/receiving/receiver_handler_test.py`

 * *Files identical despite different names*

### Comparing `sacn-1.9.0/sacn/receiving/receiver_socket_base_test.py` & `sacn-1.9.1/sacn/receiving/receiver_socket_base_test.py`

 * *Files identical despite different names*

### Comparing `sacn-1.9.0/sacn/receiving/receiver_socket_base.py` & `sacn-1.9.1/sacn/receiving/receiver_socket_base.py`

 * *Files identical despite different names*

### Comparing `sacn-1.9.0/sacn/receiving/receiver_socket_udp.py` & `sacn-1.9.1/sacn/receiving/receiver_socket_udp.py`

 * *Files identical despite different names*

### Comparing `sacn-1.9.0/sacn/receiving/receiver_handler.py` & `sacn-1.9.1/sacn/receiving/receiver_handler.py`

 * *Files identical despite different names*

### Comparing `sacn-1.9.0/sacn/receiving/receiver_socket_test.py` & `sacn-1.9.1/sacn/receiving/receiver_socket_test.py`

 * *Files identical despite different names*

### Comparing `sacn-1.9.0/sacn/sender_test.py` & `sacn-1.9.1/sacn/sender_test.py`

 * *Files identical despite different names*

