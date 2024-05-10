# Comparing `tmp/mb_netmgmt-0.0.82.tar.gz` & `tmp/mb_netmgmt-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mb_netmgmt-0.0.82.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "mb_netmgmt-0.0.9.tar", last modified: Mon Jun 13 07:34:10 2022, max compression
```

## Comparing `mb_netmgmt-0.0.82.tar` & `mb_netmgmt-0.0.9.tar`

### file list

```diff
@@ -1,20 +1,18 @@
--rw-r--r--   0        0        0       37 2023-07-25 10:19:17.807600 mb_netmgmt-0.0.82/.gitignore
--rw-r--r--   0        0        0      183 2023-08-02 11:03:06.613486 mb_netmgmt-0.0.82/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1063 2023-07-25 10:19:17.807600 mb_netmgmt-0.0.82/AUTHORS
--rw-r--r--   0        0        0      528 2023-07-25 10:19:17.807600 mb_netmgmt-0.0.82/CODEOWNERS
--rw-r--r--   0        0        0     5489 2023-07-25 10:19:17.810933 mb_netmgmt-0.0.82/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     4530 2023-07-25 10:19:17.810933 mb_netmgmt-0.0.82/CONTRIBUTING.md
--rw-r--r--   0        0        0    18092 2023-07-25 10:19:17.810933 mb_netmgmt-0.0.82/COPYING
--rw-r--r--   0        0        0      502 2024-05-10 09:01:33.920939 mb_netmgmt-0.0.82/Dockerfile
--rw-r--r--   0        0        0     6488 2023-07-25 10:19:17.810933 mb_netmgmt-0.0.82/README.md
--rw-r--r--   0        0        0        0 2023-07-25 10:19:17.810933 mb_netmgmt-0.0.82/conftest.py
--rw-r--r--   0        0        0     3864 2024-05-10 09:01:33.920939 mb_netmgmt-0.0.82/mb_netmgmt/__init__.py
--rwxr-xr-x   0        0        0     5480 2024-02-07 12:49:37.640869 mb_netmgmt-0.0.82/mb_netmgmt/__main__.py
--rwxr-xr-x   0        0        0     4916 2024-01-05 15:27:45.474985 mb_netmgmt-0.0.82/mb_netmgmt/netconf.py
--rw-r--r--   0        0        0      279 2024-01-05 15:11:48.921279 mb_netmgmt-0.0.82/mb_netmgmt/protocols.json
--rw-r--r--   0        0        0     4852 2023-08-02 11:03:06.613486 mb_netmgmt-0.0.82/mb_netmgmt/snmp.py
--rw-r--r--   0        0        0     4569 2023-07-25 10:19:17.810933 mb_netmgmt-0.0.82/mb_netmgmt/ssh.py
--rw-r--r--   0        0        0     3511 2024-05-10 09:01:33.920939 mb_netmgmt-0.0.82/mb_netmgmt/telnet.py
--rw-r--r--   0        0        0      271 2024-01-05 15:18:59.159915 mb_netmgmt-0.0.82/pyproject.toml
--rw-r--r--   0        0        0     8976 2024-02-07 21:03:32.347334 mb_netmgmt-0.0.82/test/test_mb_netmgmt.py
--rw-r--r--   0        0        0      268 1970-01-01 00:00:00.000000 mb_netmgmt-0.0.82/PKG-INFO
+-rw-r--r--   0        0        0       29 2022-06-10 12:37:21.272670 mb_netmgmt-0.0.9/.gitignore
+-rw-r--r--   0        0        0     1063 2022-05-12 07:55:21.636265 mb_netmgmt-0.0.9/AUTHORS
+-rw-r--r--   0        0        0      528 2022-05-12 07:42:27.646338 mb_netmgmt-0.0.9/CODEOWNERS
+-rw-r--r--   0        0        0     5489 2022-05-12 07:42:27.646338 mb_netmgmt-0.0.9/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     4530 2022-05-12 07:42:27.646338 mb_netmgmt-0.0.9/CONTRIBUTING.md
+-rw-r--r--   0        0        0    18092 2022-05-12 07:42:27.649671 mb_netmgmt-0.0.9/COPYING
+-rw-r--r--   0        0        0      173 2022-05-16 14:19:22.315290 mb_netmgmt-0.0.9/Dockerfile
+-rw-r--r--   0        0        0     4248 2022-05-12 15:16:00.210932 mb_netmgmt-0.0.9/README.md
+-rw-r--r--   0        0        0     2083 2022-06-13 07:33:52.801133 mb_netmgmt-0.0.9/mb_netmgmt/__init__.py
+-rwxr-xr-x   0        0        0     3560 2022-06-12 18:57:24.622529 mb_netmgmt-0.0.9/mb_netmgmt/__main__.py
+-rwxr-xr-x   0        0        0     1044 2022-06-10 12:50:34.479268 mb_netmgmt-0.0.9/mb_netmgmt/netconf.py
+-rw-r--r--   0        0        0      279 2022-05-12 15:45:50.527927 mb_netmgmt-0.0.9/mb_netmgmt/protocols.json
+-rw-r--r--   0        0        0     4262 2022-05-18 12:23:11.443961 mb_netmgmt-0.0.9/mb_netmgmt/snmp.py
+-rw-r--r--   0        0        0     3828 2022-06-12 19:40:04.468538 mb_netmgmt-0.0.9/mb_netmgmt/ssh.py
+-rw-r--r--   0        0        0     2949 2022-06-12 18:57:48.395872 mb_netmgmt-0.0.9/mb_netmgmt/telnet.py
+-rw-r--r--   0        0        0      140 2022-05-12 11:32:43.680335 mb_netmgmt-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     1628 2022-06-12 19:46:42.858320 mb_netmgmt-0.0.9/test/test_mb_netmgmt.py
+-rw-r--r--   0        0        0      107 1970-01-01 00:00:00.000000 mb_netmgmt-0.0.9/PKG-INFO
```

### Comparing `mb_netmgmt-0.0.82/AUTHORS` & `mb_netmgmt-0.0.9/AUTHORS`

 * *Files identical despite different names*

### Comparing `mb_netmgmt-0.0.82/CODEOWNERS` & `mb_netmgmt-0.0.9/CODEOWNERS`

 * *Files identical despite different names*

### Comparing `mb_netmgmt-0.0.82/CODE_OF_CONDUCT.md` & `mb_netmgmt-0.0.9/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `mb_netmgmt-0.0.82/CONTRIBUTING.md` & `mb_netmgmt-0.0.9/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `mb_netmgmt-0.0.82/COPYING` & `mb_netmgmt-0.0.9/COPYING`

 * *Files identical despite different names*

### Comparing `mb_netmgmt-0.0.82/mb_netmgmt/snmp.py` & `mb_netmgmt-0.0.9/mb_netmgmt/snmp.py`

 * *Files 16% similar despite different names*

```diff
@@ -14,21 +14,19 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with mb-netmgmt. If not, see <https://www.gnu.org/licenses/
 
 import binascii
-import logging
 from base64 import b64decode, b64encode
 from socket import SOCK_DGRAM, socket
 from socketserver import DatagramRequestHandler, ThreadingUDPServer, UDPServer
 
 from scapy.asn1.asn1 import ASN1_Class_UNIVERSAL
-from scapy.asn1.ber import BER_Decoding_Error
 from scapy.layers.snmp import SNMP, SNMPbulk, SNMPresponse, SNMPvarbind
 
 from mb_netmgmt.__main__ import Protocol
 
 Server = ThreadingUDPServer
 
 
@@ -58,22 +56,21 @@
 
     def open_upstream(self, to):
         self.upstream_socket = socket(type=SOCK_DGRAM)
         self.upstream_socket.connect((to, 161))
 
     def read_proxy_response(self):
         bytes_response = self.upstream_socket.recv(UDPServer.max_packet_size)
-        try:
-            snmp_response = SNMP(bytes_response)
-        except BER_Decoding_Error:
-            logging.error(bytes_response)
-            raise
+        snmp_response = SNMP(bytes_response)
         result = dict()
         for varbind in snmp_response.PDU.varbindlist:
-            result[varbind.oid.val] = to_dict(varbind)
+            result[varbind.oid.val] = {
+                "val": decode(varbind.value.val),
+                "tag": str(varbind.value.tag),
+            }
 
         return result
 
     def send_upstream(self, request, request_id):
         oids = request["oids"]
         pdu_type = type(self.snmp_request.PDU)
         kwargs = dict()
@@ -102,47 +99,24 @@
         return {"oid": varbind.oid.val}
 
     def translate_json_to_network_response(self, json):
         result = list()
         for oid, response in json.items():
             if oid.startswith("_"):
                 continue
-            result += to_varbind(oid, response)
+            value = response["val"]
+            try:
+                value = b64decode(value, validate=True)
+            except (binascii.Error, TypeError):
+                pass
+            asn1_class = ASN1_Class_UNIVERSAL.__dict__[response["tag"]]
+            result += SNMPvarbind(oid=oid, value=asn1_class.asn1_object(value))
         return result
 
 
 def decode(value):
     try:
         return value.decode()
     except AttributeError:
         return value
     except UnicodeDecodeError:
         return b64encode(value).decode()
-
-
-def to_dict(varbind):
-    val = None
-    tag = None
-    if varbind.value:
-        val = decode(varbind.value.val)
-        tag = str(varbind.value.tag)
-    result = {"val": val, "tag": tag}
-    if varbind.noSuchObject:
-        result["noSuchObject"] = 0
-    if varbind.noSuchInstance:
-        result["noSuchInstance"] = 0
-    if varbind.endOfMibView:
-        result["endOfMibView"] = 0
-    return result
-
-
-def to_varbind(oid, response):
-    value = response["val"]
-    try:
-        value = b64decode(value, validate=True)
-        asn1_class = ASN1_Class_UNIVERSAL.__dict__[response["tag"]]
-        value = asn1_class.asn1_object(value)
-    except (binascii.Error, TypeError):
-        pass
-    del response["val"]
-    del response["tag"]
-    return SNMPvarbind(oid=oid, value=value, **response)
```

### Comparing `mb_netmgmt-0.0.82/mb_netmgmt/ssh.py` & `mb_netmgmt-0.0.9/mb_netmgmt/ssh.py`

 * *Files 16% similar despite different names*

```diff
@@ -13,23 +13,25 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with mb-netmgmt. If not, see <https://www.gnu.org/licenses/
 
+import os
 import re
-from socketserver import BaseRequestHandler
-from socketserver import ThreadingTCPServer as Server
+from socketserver import BaseRequestHandler, TCPServer
 
 import paramiko
 
-from mb_netmgmt.__main__ import Protocol, get_cli_patterns
+from mb_netmgmt.__main__ import Protocol
 
+Server = TCPServer
 stopped = False
+message_id_regex = ' message-id="([^"]*)"'
 
 
 class ParamikoServer(paramiko.ServerInterface):
     def get_allowed_auths(*args):
         return "password,publickey"
 
     def check_auth_password(*args):
@@ -37,106 +39,85 @@
 
     def check_auth_publickey(*args):
         return paramiko.AUTH_SUCCESSFUL
 
     def check_channel_request(*args):
         return paramiko.OPEN_SUCCEEDED
 
-    def check_channel_pty_request(
-        self, channel, term, width, height, pixelwidth, pixelheight, modes
-    ):
-        transport = channel.transport
-        channel.upstream = open_upstream(
-            transport.to,
-            transport.key_filename,
-            term,
-            width,
-            height,
-            pixelwidth,
-            pixelheight,
-        )
-        channel.command_prompt = b"#"
-        channel.command_prompt = handle_prompt(self.handle_request)
+    def check_channel_pty_request(*args):
         return True
 
     def check_channel_shell_request(*args):
         return True
 
     def check_channel_subsystem_request(*args):
         return True
 
 
 class Handler(BaseRequestHandler, Protocol):
+    message_terminator = b"\n"
+    default_port = 22
+
     def handle(self):
         self.callback_url = self.server.callback_url
-        transport = start_server(
-            self.request, self.get_to(), self.key_filename, self.handle_request
-        )
-        self.channel = transport.accept()
+        t = paramiko.Transport(self.request)
+        t.add_server_key(paramiko.DSSKey.generate())
+        t.add_server_key(paramiko.ECDSAKey.generate())
+        t.add_server_key(paramiko.RSAKey.generate(4096))
+        t.start_server(server=ParamikoServer())
+        self.channel = t.accept()
+        self.open_upstream()
+        self.handle_request({"command": ""}, "")
         while not stopped:
             request, request_id = self.read_request()
             self.handle_request(request, request_id)
 
     def send_upstream(self, request, request_id):
-        self.channel.upstream.sendall(request["command"])
+        self.upstream_channel.sendall(
+            replace_message_id(request["command"], request_id)
+        )
 
     def read_request(self):
-        request = self.read_message(self.channel, [b"\n", b"\r"])
-        return {"command": request.decode()}, None
+        request = self.read_message(self.channel)
+        return (
+            {"command": replace_message_id(request.decode(), "")},
+            get_message_id(request.decode()),
+        )
 
     def respond(self, response, request_id):
-        response = response["response"]
+        response = replace_message_id(response["response"], request_id)
         self.channel.sendall(response)
-        return response
 
+    def open_upstream(self):
+        to = self.get_to()
+        if not to:
+            return
+        client = paramiko.SSHClient()
+        client.set_missing_host_key_policy(paramiko.AutoAddPolicy)
+        client.connect(
+            to,
+            os.environ.get("NETCONF_PORT", self.default_port),
+            os.environ["NETCONF_USERNAME"],
+            os.environ["NETCONF_PASSWORD"],
+        )
+        transport: paramiko.Transport = client._transport
+        self.upstream_channel = transport.open_session()
+ 
     def read_proxy_response(self):
-        prompt_patterns = [self.channel.command_prompt]
-        prompt_patterns += get_cli_patterns()
-        message = self.read_message(self.channel.upstream, prompt_patterns)
-        return {"response": message.decode()}
+        return {"response": self.read_message(self.upstream_channel).decode()}
 
-    def read_message(self, channel, patterns):
+    def read_message(self, channel):
         message = b""
-        end_of_message = False
-        while not end_of_message and not stopped:
+        while self.message_terminator not in message and not stopped:
             message += channel.recv(1024)
-            for pattern in patterns:
-                if re.findall(pattern, message):
-                    end_of_message = True
-                    break
         return message
 
 
-def open_upstream(to, key_filename, term, width, height, pixelwidth, pixelheight):
-    if not to:
-        return
-    client = paramiko.SSHClient()
-    client.set_missing_host_key_policy(paramiko.AutoAddPolicy)
-    client.connect(
-        to.hostname,
-        to.port or paramiko.config.SSH_PORT,
-        to.username,
-        to.password,
-        key_filename=key_filename,
-        transport_factory=paramiko.Transport,
-        look_for_keys=False,
-    )
-    return client.invoke_shell(term, width, height, pixelwidth, pixelheight)
-
-
-def handle_prompt(handle_request):
-    response = handle_request({"command": ""}, "")
-    command_prompt = response.split("\n")[-1].encode()
-    return command_prompt
-
-
-def start_server(request, to, key_filename, handle_request):
-    t = paramiko.Transport(request)
-    t.add_server_key(paramiko.DSSKey.generate())
-    t.add_server_key(paramiko.ECDSAKey.generate())
-    t.add_server_key(paramiko.RSAKey.generate(4096))
-    t.to = to
-    t.key_filename = key_filename
-    paramiko_server = ParamikoServer()
-    paramiko_server.handle_request = handle_request
-    t.start_server(server=paramiko_server)
-    return t
+def get_message_id(rpc):
+    try:
+        return re.findall(message_id_regex, rpc)[0]
+    except IndexError:
+        return None
+
+
+def replace_message_id(rpc, message_id):
+    return re.sub(message_id_regex, f' message-id="{message_id}"', rpc)
```

### Comparing `mb_netmgmt-0.0.82/mb_netmgmt/telnet.py` & `mb_netmgmt-0.0.9/mb_netmgmt/telnet.py`

 * *Files 24% similar despite different names*

```diff
@@ -14,87 +14,73 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with mb-netmgmt. If not, see <https://www.gnu.org/licenses/
 
 import re
+import telnetlib
 import time
-from socketserver import StreamRequestHandler
-from socketserver import ThreadingTCPServer as Server
-
-from Exscript.protocols import Telnet
+from socketserver import StreamRequestHandler, TCPServer
 
 from mb_netmgmt.__main__ import Protocol
 
+Server = TCPServer
+
 
 class Handler(StreamRequestHandler, Protocol):
     def handle(self):
         self.callback_url = self.server.callback_url
         self.handle_username_prompt()
         self.username = extract_username(self.rfile.readline())
         self.handle_username()
         self.read_password()
         self.command_prompt = b"#"
         try:
-            self.telnet.send(self.password)
-            self.command_prompt = self.telnet.expect_prompt()[1].string.encode()
-            self.telnet.app_authenticated = True
+            self.telnet.write(self.password)
+            self.command_prompt = self.telnet.read_until(b"#").split(b"\n")[-1]
         except AttributeError:
             pass
         self.wfile.write(self.command_prompt)
         request = None
-        self.stopped = False
-        while not self.stopped:
+        while request != b"exit\r\n":
             request, request_id = self.read_request()
             if not request:
                 return
             self.handle_command(request, request_id)
 
     def handle_command(self, command, request_id):
         return self.handle_request({"command": command.decode()}, request_id)
 
     def send_upstream(self, request, request_id):
-        self.telnet.send(request["command"])
+        self.telnet.write(request["command"].encode())
 
     def read_request(self):
         return self.rfile.readline(), None
 
     def respond(self, response, request_id):
         self.wfile.write(response["response"].encode())
-        if response["response"].encode() in [b"exit\r\n\r", b"quit\r\n\r"]:
-            self.stopped = True
 
     def read_proxy_response(self):
-        _, match = self.telnet.expect_prompt()
-        return {"response": match.string}
+        return {"response": self.telnet.read_until(self.command_prompt).decode()}
 
     def handle_username_prompt(self):
         username_prompt = b"Username: "
         to = self.get_to()
         if to:
-            t = Telnet(debug=4)
-            t.connect(to.hostname)
-            result = t.expect(t.get_username_prompt())
-            username_prompt = (t.response[:-1] + result[1].string).encode()
-            self.telnet = t
+            self.telnet = telnetlib.Telnet(to)
+            username_prompt = self.telnet.read_until(username_prompt)
         self.wfile.write(username_prompt)
 
     def read_password(self):
         self.password = self.rfile.readline()
         while not self.password:
             time.sleep(1)
             self.password = self.rfile.readline()
 
     def handle_username(self):
-        try:
-            t = self.telnet
-            t.send(self.username)
-            result = t.expect(t.get_password_prompt())
-            password_prompt = result[1].string.encode()
-            self.wfile.write(password_prompt)
-        except AttributeError:
-            self.handle_request({"command": self.username.decode()}, None)        
+        self.command_prompt = b"Password: "
+        self.handle_request({"command": self.username.decode()}, None)
 
 
 def extract_username(byte_string):
     return re.match(b".*?([-0-9a-zA-Z_].*\n)", byte_string).group(1)
```

