# Comparing `tmp/czo-0.1.8.tar.gz` & `tmp/czo-0.1.9.tar.gz`

## Comparing `czo-0.1.8.tar` & `czo-0.1.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 czo-0.1.8/czo/__init__.py
--rw-r--r--   0        0        0     8617 2020-02-02 00:00:00.000000 czo-0.1.8/czo/_date.py
--rw-r--r--   0        0        0    12058 2020-02-02 00:00:00.000000 czo-0.1.8/czo/_faker.py
--rw-r--r--   0        0        0     8377 2020-02-02 00:00:00.000000 czo-0.1.8/czo/_net.py
--rw-r--r--   0        0        0     5943 2020-02-02 00:00:00.000000 czo-0.1.8/czo/_path.py
--rw-r--r--   0        0        0     4976 2020-02-02 00:00:00.000000 czo-0.1.8/czo/_rand.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 czo-0.1.8/czo/data/__init__.py
--rw-r--r--   0        0        0    14519 2020-02-02 00:00:00.000000 czo-0.1.8/czo/data/_country.py
--rw-r--r--   0        0        0    16493 2020-02-02 00:00:00.000000 czo-0.1.8/czo/data/_housing.py
--rw-r--r--   0        0        0   154755 2020-02-02 00:00:00.000000 czo-0.1.8/czo/data/_internal_utils.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 czo-0.1.8/czo/utils/__init__.py
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 czo-0.1.8/czo/utils/__meta.py
--rw-r--r--   0        0        0     3176 2020-02-02 00:00:00.000000 czo-0.1.8/.gitignore
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 czo-0.1.8/LICENSE
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 czo-0.1.8/README.md
--rw-r--r--   0        0        0      840 2020-02-02 00:00:00.000000 czo-0.1.8/pyproject.toml
--rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 czo-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 czo-0.1.9/czo/__init__.py
+-rw-r--r--   0        0        0     8919 2020-02-02 00:00:00.000000 czo-0.1.9/czo/_date.py
+-rw-r--r--   0        0        0    12058 2020-02-02 00:00:00.000000 czo-0.1.9/czo/_faker.py
+-rw-r--r--   0        0        0     8419 2020-02-02 00:00:00.000000 czo-0.1.9/czo/_net.py
+-rw-r--r--   0        0        0     6339 2020-02-02 00:00:00.000000 czo-0.1.9/czo/_path.py
+-rw-r--r--   0        0        0     8119 2020-02-02 00:00:00.000000 czo-0.1.9/czo/_rand.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 czo-0.1.9/czo/data/__init__.py
+-rw-r--r--   0        0        0    14519 2020-02-02 00:00:00.000000 czo-0.1.9/czo/data/_country.py
+-rw-r--r--   0        0        0    16493 2020-02-02 00:00:00.000000 czo-0.1.9/czo/data/_housing.py
+-rw-r--r--   0        0        0   154755 2020-02-02 00:00:00.000000 czo-0.1.9/czo/data/_internal_utils.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 czo-0.1.9/czo/utils/__init__.py
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 czo-0.1.9/czo/utils/__meta.py
+-rw-r--r--   0        0        0     3176 2020-02-02 00:00:00.000000 czo-0.1.9/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 czo-0.1.9/LICENSE
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 czo-0.1.9/README.md
+-rw-r--r--   0        0        0      942 2020-02-02 00:00:00.000000 czo-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 czo-0.1.9/PKG-INFO
```

### Comparing `czo-0.1.8/czo/_date.py` & `czo-0.1.9/czo/_date.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,30 @@
 import datetime
 import time
 
 
-class FastDate:
+class DateLib:
     """
-   提供了一组静态方法，用于处理日期和时间的常见操作。
-   """
+    提供了一组静态方法，用于处理日期和时间的常见操作。
+    """
+
+    @staticmethod
+    def timestamp() -> int:
+        """
+        返回当前时间的时间戳。
+        """
+        return int(time.time())
+
+    @staticmethod
+    def timestamp_ms() -> int:
+        """
+        返回当前时间的时间戳。
+        """
+        return int(time.time() * 1000)
+
     @staticmethod
     def now_date() -> str:
         """
         返回当前日期和时间的格式化字符串。
 
         Returns:
             当前日期和时间的格式化字符串，格式为"%Y-%m-%d %H:%M:%S"。
```

### Comparing `czo-0.1.8/czo/_faker.py` & `czo-0.1.9/czo/_faker.py`

 * *Files identical despite different names*

### Comparing `czo-0.1.8/czo/_net.py` & `czo-0.1.9/czo/_net.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from time import sleep
 from typing import Any, Generator
 
 
 class NetLib:
 
     @staticmethod
-    def cidr(address, netmask_or_prefix) -> dict[str, Any] | ValueError:
+    def cidr(address: str, netmask_or_prefix: int | str) -> dict[str, Any] | ValueError:
         """
         根据指定的网络和前缀长度计算CIDR信息。
 
         参数:
         - network: 字符串，指定的网络地址，可以是IPv4或IPv6格式。
         - prefix: 整数，网络的前缀长度。
 
@@ -22,16 +22,16 @@
         Examples:
         >>> print(Net.cidr('192.168.1.0', 24))
 
         >>> print(Net.cidr('240e::0', 64))
         """
 
         try:
-            ipType: ipaddress.IPv6Network | ipaddress.IPv4Network = ipaddress.IPv6Network if ':' in address else ipaddress.IPv4Network
-            cidr = ipType(f'{address}/{netmask_or_prefix}')
+            ip_type: ipaddress.IPv6Network | ipaddress.IPv4Network = ipaddress.IPv6Network if ':' in address else ipaddress.IPv4Network
+            cidr = ip_type(f'{address}/{netmask_or_prefix}')
 
             # 输出网络地址、子网掩码、广播地址等信息
             host_count = cidr.num_addresses - 2
             range = str(cidr.network_address + 1) + '-' + \
                 str(cidr.broadcast_address - 1)
             network_address = str(cidr.network_address)
             broadcast_address = str(cidr.broadcast_address)
@@ -40,15 +40,15 @@
 
             return {'host_count': host_count, 'range': range, 'network_address': network_address, 'broadcast_address': broadcast_address, 'prefixlen': prefixlen, 'netmask': netmask}
 
         except ValueError as e:
             return e
 
     @staticmethod
-    def ipaddress_generator(number: int, isIpv6: bool = False, max: int = 254, **kwargs) -> Generator[IPv4Address, IPv6Address, None]:
+    def ipaddress_generator(number: int, max: int = 254, is_ipv6: bool = False,  **kwargs) -> Generator[IPv4Address, IPv6Address, None]:
         """
         生成指定数量的IP地址序列。
 
         Args:
         - number: 每次生成的IP地址数量。
         - isIpv6: 是否生成IPv6地址，默认为False，即生成IPv4地址。
         - max: 生成IP地址的最大数量。
@@ -67,23 +67,23 @@
         c: int = kwargs.get("c", 1)
         d: int = kwargs.get("d", 1)
         e: int = kwargs.get("e", 1)
         f: int = kwargs.get("f", 1)
         g: int = kwargs.get("g", 1)
         h: int = kwargs.get("h", 1)
 
-        if isIpv6 is False:
+        if is_ipv6 is False:
             a_range: int = 256
             b_range: int = 256
             c_range: int = 256
             d_range: int = 255
-            ipList: list = []
+            ip_list: list = []
             count: int = 0
             for _ in range(1, max+1):
-                ipList.append(ipaddress.IPv4Address(f"{a}.{b}.{c}.{d}"))
+                ip_list.append(ipaddress.IPv4Address(f"{a}.{b}.{c}.{d}"))
                 count += 1
                 d += 1
 
                 if d == d_range:
                     d = 1
                     c = c+1
                     if c == c_range:
@@ -91,32 +91,32 @@
                         b = b+1
                         if b == b_range:
                             b = 1
                             a = a+1
                             if a == a_range:
                                 a = 1
 
-                if len(ipList) % number == 0:
-                    yield ipList
-                    ipList = []
-                if max == count and len(ipList) != 0:
-                    yield ipList
+                if len(ip_list) % number == 0:
+                    yield ip_list
+                    ip_list = []
+                if max == count and len(ip_list) != 0:
+                    yield ip_list
         else:
             a_range: int = 65536
             b_range: int = 65536
             c_range: int = 65536
             d_range: int = 65536
             e_range: int = 65536
             f_range: int = 65536
             g_range: int = 65536
             h_range: int = 65536
-            ipList: list = []
+            ip_list: list = []
             count: int = 0
             for _ in range(1, max+1):
-                ipList.append(ipaddress.IPv6Address(
+                ip_list.append(ipaddress.IPv6Address(
                     f"{a:04x}:{b:04x}:{c:04x}:{d:04x}:{e:04x}:{f:04x}:{g:04x}:{h:04x}"))
                 count += 1
                 h += 1
 
                 if h == h_range:
                     h = 1
                     g = g+1
@@ -137,19 +137,19 @@
                                         b = b+1
                                         if b == b_range:
                                             b = 1
                                             a = a+1
                                             if a == a_range:
                                                 a = 1
 
-                if len(ipList) % number == 0:
-                    yield ipList
-                    ipList = []
-                if max == count and len(ipList) != 0:
-                    yield ipList
+                if len(ip_list) % number == 0:
+                    yield ip_list
+                    ip_list = []
+                if max == count and len(ip_list) != 0:
+                    yield ip_list
 
     @staticmethod
     def ip_in_subnet(ip_str, subnet_str):
         """
 
         Example:
         ip = '2a00::110:133'
@@ -208,17 +208,17 @@
         a_range: int = 256
         b_range: int = 256
         c_range: int = 256
         d_range: int = 256
         e_range: int = 256
         f_range: int = 256
         count = 0
-        macList = []
+        mac_list = []
         for _ in range(1, max+1):
-            macList.append(f"{a:02x}:{b:02x}:{c:02x}:{d:02x}:{e:02x}:{f:02x}")
+            mac_list.append(f"{a:02x}:{b:02x}:{c:02x}:{d:02x}:{e:02x}:{f:02x}")
             count += 1
             f += 1
             if f == f_range:
                 f = 1
                 e = e+1
                 if e == e_range:
                     e = 1
@@ -230,12 +230,12 @@
                             c = 1
                             b = b+1
                             if b == b_range:
                                 b = 1
                                 a = a+1
                                 if a == a_range:
                                     a = 1
-            if len(macList) % number == 0:
-                yield macList
-                macList = []
-            if max == count and len(macList) != 0:
-                yield macList
+            if len(mac_list) % number == 0:
+                yield mac_list
+                mac_list = []
+            if max == count and len(mac_list) != 0:
+                yield mac_list
```

### Comparing `czo-0.1.8/czo/_path.py` & `czo-0.1.9/czo/_path.py`

 * *Files 6% similar despite different names*

```diff
@@ -173,7 +173,23 @@
             # 执行目录重命名操作
             self.directory.rename(new_directory_path)
 
             return new_directory_path
         else:
             # 目录为空，不进行重命名
             return False
+
+    @staticmethod
+    def delete_glob_file(dir_path: Path | str, file_name: str):
+        """
+        删除指定目录下匹配的文件
+
+        Example:
+            delete_glob_file(Path("./"), "*.json")
+        """
+        try:
+            for file in dir_path.glob("qemu_info_*.json"):
+                file.unlink()
+        except Exception as e:
+            return e
+
+        return True
```

### Comparing `czo-0.1.8/czo/_rand.py` & `czo-0.1.9/czo/_rand.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,19 @@
 import hashlib
 import ipaddress
 import random
 import secrets
 import shutil
 import string
 import uuid
+import warnings
+from typing import Literal
+
+# 设置警告过滤器
+warnings.filterwarnings("always")
 
 
 class Random:
     """
     随机生成一些测试数据
     """
     @staticmethod
@@ -48,44 +53,56 @@
         with open(temp_name, 'rb') as r:
             md5: str = hashlib.md5(r.read()).hexdigest()
         temp_path: str = f'./{md5}'
         shutil.move(temp_name, temp_path)
         return temp_path, md5
 
     @staticmethod
-    def str(length: int, is_zh: bool = False, mark: bool = False, is_int: bool = False) -> str:
+    def str(length: int = 1, is_zh: bool = False, mark: bool = False, is_int: bool = False, zh_code_is_unicode=False) -> str:
         """
-        生成指定长度的随机字符串。
+        生成指定长度的随机大小写字母、数字组成的字符串。
 
         Args:
             length (int): 字符串长度。
             is_zh (bool, optional): 是否包含中文字符，默认为 False。
-            mark (bool, optional): 是否包含标点符号，默认为 False。
+            mark (bool, optional): 默认生成的字符串是否包含标点符号，默认为 False。
             is_int (bool, optional): 是否生成随机整数字符串，默认为 False。
+            zh_code_is_unicode (bool, optional): 使用Unicode编码生成中文字符。默认使用GBK编码生成更常见的中文字符。
 
         Returns:
             str: 生成的随机字符串。
 
-        Example:
-            ```python
-            result = random_str(10)
-            print(result)  # 输出: "random_str"
-            ```
+        Examples:
+        >>> print(Random.str(1))   
+
         """
 
-        def generate_chinese():
-            result = ""
+        def Unicode() -> str:
+            result: Literal[''] = ""
             for _ in range(length):
-                # 生成随机的中文字符
                 char = chr(random.randint(0x4E00, 0x9FA5))
                 result += char
             return result
 
+        def GBK2312() -> str:
+            result: Literal[''] = ""
+            for _ in range(length):
+                head = random.randint(0xb0, 0xf7)
+                body = random.randint(0xa1, 0xfe)
+                val = f'{head:x} {body:x}'
+                str = bytes.fromhex(val).decode('gb2312')
+                result += str
+            return result
+
         if is_zh:
-            return generate_chinese()
+            if zh_code_is_unicode:
+                return Unicode()
+            else:
+                return GBK2312()
+
         if is_int:
             return ''.join(str(secrets.randbelow(10)) for _ in range(length))
 
         from random import SystemRandom
         sys_random = SystemRandom()
 
         if mark:
@@ -129,27 +146,90 @@
 
     @staticmethod
     def ipv4():
         """
         生成一个随机的IPv4地址。
 
         Returns:
-        - IPv4Address: 一个随机生成的IPv4地址对象。
+        - IPv4Address: 一个随机生成的IPv4地址。
         """
-        return ipaddress.IPv4Address(random.randint(0, 2**32-1))
+        warnings.warn(f"`{Random.ipv4.__name__}`已弃用即将删除，改用`Random.ip`",
+                      DeprecationWarning, stacklevel=2)
+        return ipaddress.IPv4Address(random.randint(0, 2**32-1)).__str__()
 
     @staticmethod
     def ipv6():
         """
         生成一个随机的IPv6地址。
 
         Returns:
-        - IPv6Address: 返回一个随机生成的IPv6地址对象。
+        - IPv6Address: 返回一个随机生成的IPv6地址。
         """
-        return ipaddress.IPv6Address(random.randint(0, 2**128-1))
+
+        warnings.warn(f"`{Random.ipv6.__name__}`已弃用即将删除，改用`Random.ip`",
+                      DeprecationWarning, stacklevel=2)
+        return ipaddress.IPv6Address(random.randint(0, 2**128-1)).__str__()
 
     @staticmethod
-    def mac():
+    def ip(is_ipv6: bool = False) -> str:
+        """
+        生成一个随机的IP地址。
+        """
+        if is_ipv6:
+            return ipaddress.IPv6Address(random.randint(0, 2**128-1)).__str__()
+        else:
+            return ipaddress.IPv4Address(random.randint(0, 2**32-1)).__str__()
+
+    @staticmethod
+    def ip_suffix_is_0(is_ipv6: bool = False, suffix: str = 0) -> str:
+        """
+        生成一个随机后缀为`0`|`suffix`的IP地址。
+        """
+        if is_ipv6:
+            return ":".join(
+                [f"{random.randint(0, 65535):x}" for _ in range(4)]) + f"::{suffix}"
+        else:
+            return ".".join(
+                [f"{random.randint(0, 255)}" for _ in range(3)]) + f".{suffix}"
+
+    @staticmethod
+    def ip_range(is_ipv6: bool = False):
+        """
+        生成一个IP地址范围，可以是IPv4或IPv6地址格式。
+
+        Args:
+        - is_ipv6: bool 值，用于指定生成IPv4还是IPv6地址范围。默认为False，表示生成IPv4地址范围。
+
+        Returns:
+        - 返回一个字符串，表示IP地址范围。如果is_ipv6为True，则返回IPv6地址范围，否则返回IPv4地址范围。
+        """
+        if is_ipv6:
+            ip = ":".join(
+                [f"{random.randint(0, 65535):x}" for _ in range(4)])
+            return f"{ip}::{random.randint(1, 10000):x}-{ip}::{random.randint(20000, 65500):x}"
+        else:
+            ip = ".".join(
+                [f"{random.randint(0, 255)}" for _ in range(3)])
+            return f"{ip}.{random.randint(1, 100)}-{ip}.{random.randint(110, 254)}"
 
+    @staticmethod
+    def ip_netmask(is_ipv6: bool = False, netmask: int | None = None):
+        """
+        生成一个随机的IP子网掩码格式。
+        """
+        if is_ipv6:
+            netmask = netmask if netmask is not None else random.randint(
+                64, 128)
+            return f"{Random.ip_suffix_is_0(True)}/{netmask}"
+        else:
+            netmask = netmask if netmask is not None else random.randint(8, 32)
+            return f"{Random.ip_suffix_is_0()}/{netmask}"
+
+    @staticmethod
+    @property
+    def mac():
+        """
+        生成一个随机的MAC。
+        """
         mac_address = ':'.join(['{:02x}'.format(
             (uuid.getnode() >> elements) & 0xff) for elements in range(0, 2*6, 2)])
         return mac_address
```

### Comparing `czo-0.1.8/czo/data/_country.py` & `czo-0.1.9/czo/data/_country.py`

 * *Files identical despite different names*

### Comparing `czo-0.1.8/czo/data/_housing.py` & `czo-0.1.9/czo/data/_housing.py`

 * *Files identical despite different names*

### Comparing `czo-0.1.8/czo/data/_internal_utils.py` & `czo-0.1.9/czo/data/_internal_utils.py`

 * *Files identical despite different names*

### Comparing `czo-0.1.8/.gitignore` & `czo-0.1.9/.gitignore`

 * *Files identical despite different names*

### Comparing `czo-0.1.8/LICENSE` & `czo-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `czo-0.1.8/pyproject.toml` & `czo-0.1.9/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,18 @@
+# https://packaging.python.org/en/latest/tutorials/packaging-projects/#uploading-your-project-to-pypi
 [build-system]
 requires = [
     "hatchling",
     "hatch-fancy-pypi-readme",
 ]
 build-backend = "hatchling.build"
 
 [project]
 name = "czo"
-version = "0.1.8"
+version = "0.1.9"
 authors = [
     { name = "sfwwslm", email = "sfwwslm@gmail.com" },
 ]
 description = "构建测试数据的工具包"
 readme = "README.md"
 requires-python = ">=3.10"
 license = "MIT"
```

### Comparing `czo-0.1.8/PKG-INFO` & `czo-0.1.9/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: czo
-Version: 0.1.8
+Version: 0.1.9
 Summary: 构建测试数据的工具包
 Project-URL: Homepage, https://github.com/sfwwslm/czo
 Project-URL: Issues, https://github.com/sfwwslm/czo/issues
 Author-email: sfwwslm <sfwwslm@gmail.com>
 License-Expression: MIT
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
```

